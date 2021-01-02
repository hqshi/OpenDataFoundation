# CODE
## 指定游戏页面
```javascript
function o() {
            var e;
            N(this, o);
            for (var t = arguments.length, n = new Array(t), i = 0; i < t; i++)
                n[i] = arguments[i];
            return x(M(e = u.call.apply(u, [this].concat(n))), "getAchievementRoutes", (function() {
                var e = ["gtaiv", "gtaiv_tlad", "gtaiv_bogt", "rdr", "mcla"].join("|");
                return [r.default.createElement(c.Redirect, {
                    key: "achievements-member-blocker",
                    from: "/member/:nickname/games/:game(".concat(e, ")/(index-signin|index)"),
                    to: "/member/:nickname/games/:game(".concat(e, ")"),
                    replace: !0
                }), r.default.createElement(c.Redirect, {
                    key: "achievements-blocker",
                    from: "/games/:game(".concat(e, ")/(index-signin|index)"),
                    to: "/games/:game(".concat(e, ")"),
                    replace: !0
                }), r.default.createElement(J, {
                    key: "achievements-member",
                    path: "/member/:nickname/games/:game(".concat(e, ")/:platform?"),
                    component: te,
                    exact: !0,
                    isAgeRestricted: !0
                }), r.default.createElement(J, {
                    key: "achievements",
                    path: "/games/:game(".concat(e, ")/:platform?"),
                    component: te,
                    exact: !0,
                    isAgeRestricted: !0
                }), r.default.createElement(J, {
                    key: "achievements-member-gtav",
                    path: "/member/:nickname/games/:game(gtav)/:platform?/:path(career/accomplishments)",
                    component: te,
                    exact: !0,
                    isAgeRestricted: !0
                }), r.default.createElement(J, {
                    key: "achievements-gtav",
                    path: "/games/:game(gtav)/:platform?/:path(career/accomplishments)",
                    component: te,
                    exact: !0,
                    isAgeRestricted: !0
                }), r.default.createElement(J, {
                    key: "achievements-member-lan-lanvr",
                    path: "/member/:nickname/games/:game(lan|lanvr)/:platform?/:path(achievements)",
                    component: te,
                    exact: !0,
                    isAgeRestricted: !0
                }), r.default.createElement(J, {
                    key: "achievements-lan-lanvr",
                    path: "/games/:game(lan|lanvr)/:platform?/:path(achievements)",
                    component: te,
                    exact: !0,
                    isAgeRestricted: !0
                }), r.default.createElement(J, {
                    key: "achievements-member-mp3",
                    path: "/member/:nickname/games/:game(maxpayne3)/:platform?/:path(accomplishments)",
                    component: te,
                    exact: !0,
                    isAgeRestricted: !0
                }), r.default.createElement(J, {
                    key: "achievements-mp3",
                    path: "/games/:game(maxpayne3)/:platform?/:path(accomplishments)",
                    component: te,
                    exact: !0,
                    isAgeRestricted: !0
                })]
            }
            )),
            e
        }
```