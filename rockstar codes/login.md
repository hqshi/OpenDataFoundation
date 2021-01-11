# 重新认证权限
[app.js](https://s.rsg.sc/sc/js/20201212bfdb/build/app.js)
> 注： 逻辑大致为请求authcheck页面后检测是否为401代码，是则请求refreshaccess页面。还是无法刷新权限则尝试重新自动登录

```javascript
function y(e, t) {
        if (401 !== e.status)
            return Promise.resolve(e);
        var n,
            r,
            o = (0, u.getAuthHeader)();
        if (o !== t.headers.get("Authorization"))
            return t.headers.set("Authorization", o), fetch(t);
        y.sharedPromise || (y.sharedPromise = new Promise((function(e, t) {
            n = function() {
                e(),
                y.sharedPromise = null
            },
            r = function(e) {
                t(e),
                y.sharedPromise = null
            }
        })).catch((function(e) {
            throw console.error("Auth retry failed", e), e
        })));
        var a = y.sharedPromise.then((function() {
            var e = (0, u.getAuthHeader)();
            return t.headers.set("Authorization", e), fetch(t)
        })).then((function(e) {
            if (401 === e.status)
                throw e;
            return e
        }));
        return y.isRunning ? a : (y.isRunning = !0, y.request = fetch("/connect/refreshaccess", {
            body: "accessToken=" + encodeURIComponent((0, u.getAuthToken)()),
            credentials: "same-origin",
            headers: {
                "X-Requested-With": "XMLHttpRequest",
                "Content-type": "application/x-www-form-urlencoded; charset=utf-8"
            },
            method: "POST",
            mode: "same-origin"
        }).then((function(e) {
            if (e.ok)
                return y.isRunning = !1, n();
            throw e
        })).catch((function() {
            return function(e, t) {
                (new i.default).get((function(n, r) {
                    var i = {
                        headers: {
                            "X-Requested-With": "XMLHttpRequest",
                            "Content-type": "application/x-www-form-urlencoded; charset=utf-8"
                        },
                        method: "POST",
                        credentials: "include",
                        body: "fingerprint=" + encodeURIComponent(r)
                    };
                    return fetch(_ + "/connect/cors/check/" + b, i).then((function(e) {
                        if (e.ok)
                            return e.json();
                        throw e
                    })).then((function(t) {
                        var n = {
                            credentials: "same-origin",
                            headers: {
                                "X-Requested-With": "XMLHttpRequest",
                                "Content-type": "application/x-www-form-urlencoded; charset=utf-8"
                            },
                            method: "POST",
                            mode: "same-origin",
                            body: "code=" + encodeURIComponent(t)
                        };
                        return fetch("/connect/silentgateway", n).then((function(t) {
                            if (t.ok)
                                return e(), t;
                            throw t
                        })).catch((function(e) {
                            throw console.error("Failed to exchange code: ", e), e
                        }))
                    })).catch((function(e) {
                        return console.error("Failed to perform silent authorization: ", e), t(e), e
                    }))
                }))
            }(n, r)
        })).then((function() {
            return y.isRunning = !1, a
        })))
    }

```

