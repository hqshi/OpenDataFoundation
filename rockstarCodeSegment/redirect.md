# 跳转页面
```html
<!doctype html>
<html class="no-js " lang="zh-CN" >
<head data-template-set="html5-reset">
    <meta charset="utf-8">
    <meta http-equiv="x-ua-compatible" content="ie=edge">
    <title data-rh="">Rockstar Games Social Club</title>
    <meta name="title" content="Rockstar Games Social Club" data-rh="">
    <meta name="keywords" content="Rockstar Games, Social Club, Rockstar">
    <meta name="description" content="" data-rh="">
    <meta name="google-site-verification" content="">
    <meta name="author" content="Rockstar North">
    <meta name="copyright" content="Rockstar Games 2021. All Rights Reserved.">
    <meta name="msapplication-config" content="none">
    <meta name="DC.title" content="Rockstar Games Social Club">
    <meta name="DC.subject" content="Rockstar Games, Social Club, Rockstar">
    <meta name="DC.creator" content="Rockstar North">

    
    <meta http-equiv="cleartype" content="on">

    <meta name="viewport" content="width=device-width, initial-scale=1">

    
        <meta name="robots" content="all">
    
        <meta name="referrer" content="origin" />


    <meta name="mobile-web-app-capable" content="yes">
    <!-- Chrome, Firefox OS and Opera -->
    <meta name="theme-color" content="#000000" data-rh="">
    <!-- Windows Phone -->
    <meta name="msapplication-navbutton-color" content="#000000" data-rh="">
    <!-- iOS Safari -->
    <meta name="apple-mobile-web-app-status-bar-style" content="#000000" data-rh="">

    <link rel="apple-touch-icon-precomposed" sizes="152x152" href="https://s.rsg.sc/sc/images/react/icons/apple-touch-icon-152x152-precomposed.png">
    <link rel="apple-touch-icon-precomposed" sizes="144x144" href="https://s.rsg.sc/sc/images/react/icons/apple-touch-icon-144x144-precomposed.png">
    <link rel="apple-touch-icon-precomposed" sizes="120x120" href="https://s.rsg.sc/sc/images/react/icons/apple-touch-icon-120x120-precomposed.png">
    <link rel="apple-touch-icon-precomposed" sizes="114x114" href="https://s.rsg.sc/sc/images/react/icons/apple-touch-icon-114x114-precomposed.png">   
    <link rel="apple-touch-icon-precomposed" sizes="76x76"   href="https://s.rsg.sc/sc/images/react/icons/apple-touch-icon-76x76-precomposed.png">
    <link rel="apple-touch-icon-precomposed" sizes="72x72"   href="https://s.rsg.sc/sc/images/react/icons/apple-touch-icon-72x72-precomposed.png">     
    <link rel="apple-touch-icon-precomposed"                 href="https://s.rsg.sc/sc/images/react/icons/apple-touch-icon-57x57-precomposed.png">     
    <link rel="shortcut icon"                                href="https://s.rsg.sc/sc/images/react/icons/apple-touch-icon-precomposed.png">           
    <link rel="shortcut icon"                                href="https://s.rsg.sc/sc/rockstar.ico">                                             

    <link href="https://s.rsg.sc/sc/js/20201212bfdb/build/app.css" rel="stylesheet">

    <link id='coreCSS' href="https://s.rsg.sc/sc/css/20201212bfdb/core.manifest.css" rel="stylesheet">

    

    <!--[if IE 9]>
        <style type="text/css">
            html * { filter: none !important; }
        </style>
    <![endif]-->

    

    <link rel="prefetch" href="https://s.rsg.sc/sc/js/20201212bfdb/build/locale-zh-CN-json.js" />
<script>

        window.smallMobileSize = 568;
        //window.mobileSize = 768;
        window.desktopSize = 1024;

        //Setting agent to be used with SASS mixins
        //See: sass/util/_mixins.scss -> agent, consoles
        document.documentElement.setAttribute("data-agent", navigator.userAgent);
    </script>

    
<script>
        window.sl_tr_start = function(){}; window.sl_tr_end = function(){}; window.sl_notr_start = function(){}; window.sl_notr_end = function(){}; window.sl_tr_json_start = function(){}; window.sl_tr_json_end = function(){};

    var siteMaster = {
        gdpr: {"eu":false,"isEnabled":true,"cookieInfo":{"name":"RSGDPR2020","ttl":12},"cookies":{"mandatory":true,"convenience":true,"tracking":true},"cookiesValues":{"mandatory":0,"convenience":1,"tracking":2},"showBanner":false},
        ccpa: {"isEnabled":false,"cookieInfo":{"name":"PolicyUpdate1_2020","expiration":"2020-06-30T13:00:00.0000000+00:00"},"showBanner":false,"isLinkEnabled":true},
        browserSessionReturnUrlCookieName: 'BrowserSessionReturnUrl',

        scFacebookAppId: '386536538045446',


        scauth: {
            client: 'socialclub',
            linkBase: 'https://signin.rockstargames.com',
            linkFlag: 'scAuthLinkStatus',
            base: 'https://signin.rockstargames.com',

            signinRedirectUrl: 'https://signin.rockstargames.com/connect/authorize/socialclub?returnUrl=%2Fmember%2Fyougase%2Fgames%2Fgtav%2Fpc%2Fcareer%2Faccomplishments&lang=zh-CN',
            signupRedirectUrl: 'https://signin.rockstargames.com/create/?cid=socialclub&returnUrl=%2Fmember%2Fyougase%2Fgames%2Fgtav%2Fpc%2Fcareer%2Faccomplishments&lang=zh-CN',
            logoutUrl: 'https://signin.rockstargames.com/logout/socialclub?returnUrl=%2F&lang=zh-CN',
            tokenCookieName: 'BearerToken'

        },

        scApiBase: 'https://scapi.rockstargames.com/',
        tileServer: 'https://sctools.rockstar.t2.corp/sctiles/',
        reactCulture: 'zh-CN',

        cdnBase: 'https://s.rsg.sc/sc',
        cdnResizerPattern: '^https?://media.rockstargames.com/.*$',
        jsBase: 'https://s.rsg.sc/sc/js/20201212bfdb',
        cssBase: 'https://s.rsg.sc/sc/css/20201212bfdb',
        cloudBase: 'https://prod.cloud.rockstargames.com',
        ugcCloudBase: 'http://prod.ros.rockstargames.com/cloud/11/cloudservices',
        avatarBase: 'https://s.rsg.sc/sc/images/avatars/',
        avatarDefault: 'https://s.rsg.sc/sc/images/avatars/default.png',
        emblemBase: 'https://prod.cloud.rockstargames.com/crews/sc/{0}/{1}/publish/emblem/emblem_{2}.png',
        emblemGalleryBase: 'https://prod.cloud.rockstargames.com/crews/sc/{0}/{1}/publish/emblems/{2}',
        emblemDefault: 'https://s.rsg.sc/sc/images/emblems/128x128/rockstar1.png',
        thirdPartyV2: true, // can be removed?
        isLoggedIn: true,
        googleAuth: true,
        fbSharing: true,
        fbSharingAppId: '386536538045446',
        twitterSharing: true,
        act: false,
        actInt: 180,
        actCnt: undefined,
        liEnabled: true,
        liBaseUrl: 'https://www.lifeinvader.com',
        gtavEnabled: true,
        locale: 'en',
        legalCulture: 'cn',
        supportCulture: 'zh-cn',
        default4Culture: 'en-us',
        support4Culture: 'zh-cn',
        support4NewsCulture: 'zh-CN',
        fbSdkCulture: 'zh-CN',
        timeAgoLocale: 'zh-cn',

        captchaCulture: 'zh-CN',

        crewsCommunity: true,
        newsHost: 'https://www.rockstargames.com/',
        sslOnly: true,
        avatarCloudBase: 'https://a.rsg.sc/',

        loginTracker: false,


        destCookies: ["https://www.lifeinvader.com/auth/Home/DestroyCookie?","https://www.rockstarwarehouse.com/store/tk2rstar/DestroyCookie","https://www.rockstargames.com/auth/users/logout.json?"],
        ssoEnabled: true,
        stsChkNm: 'statuschk.v2',
        stsChkDm: '.socialclub.rockstargames.com',
        stsChkSc: true,

        loc: true,
        locSubdomain: false,

        authUserNickName: 'yougase',
        authRockstarId: yougase,
        authUserAvatar: 'n/yougase',
        authVerifiedEmail: true,
        isEnabledAnalytics: true,
        isEnabledAnalyticsCD: true,
        gaTimeout: 30,
        gcx:
        {
            userId: yougase,
            id: '',
            variation: null
        },
        //0: Basic alerts
        //1: Responsive alerts
        alertType: 0,
        gtavBannerData:
        {
            banner: '',
            display: false
        },
    
        mfaEnabled: true,
    
        showRecaptcha: false,
        aft: '<input name="__RequestVerificationToken" type="hidden" value="o52jyhuyzvhj2mQ7MCVP1hnOuusC3i1VV9i0-ouvTkvrgSXe36e12_6JNYS7tJII96287Iux1Um7D7SU2iVakQkgLkBkHyqsc6pp2DoQCK36IesGcHrPqAvZKglU9labOVAbKg2" />',
        blockerRedirectUrl: ''
    },
    require = {
        baseUrl: siteMaster.jsBase,
    };
</script>


    

<script>window.webpackPublicPath = "https://s.rsg.sc/sc/js/20201212bfdb/build/"</script>
<script src="https://s.rsg.sc/sc/js/20201212bfdb/build/shared.js"></script>
    <script src="https://s.rsg.sc/sc/js/20201212bfdb/build/jquery.js"></script>
    <script src="https://s.rsg.sc/sc/js/20201212bfdb/build/common.js"></script>

</head>

<body class="bg_home_landing   twoCol  react smartling-zh-cn">

    <div id="fb-root"></div> 

    <div id="app-root" class="notranslate"></div>

    <div id="wrapper" class="bgDefault bg_home_landing">

        <div id="pageWrapper">

            <div id="pageMask"></div>

            <div id="page" class="clearfix">

            

                <div class="clear"></div>

            </div>

        </div>

    </div>

    <input name="__RequestVerificationToken" type="hidden" value="tKN8_mCOp8whXLAXuFjT1mhOVAkq2S2LgE0nVrkvd1yFbLxBm5K6wEktqSg_oIK0zlRtxjJ_6EOFQIF-W5BfShAHt_lK06cuyLOLsnQPQrY8qt6wMBaXZkg1EtarW8oSH0uVbg2" />

    
    

    <script type="text/javascript" src="https://s.rsg.sc/sc/js/20201212bfdb/build/app.js" data-config="{&quot;sl_translate&quot;:&quot;sl_none&quot;,&quot;langCookieName&quot;:&quot;rockstarweb_lang.prod&quot;,&quot;websocketReconnectTime&quot;:60,&quot;websocketReconnectCount&quot;:3,&quot;baseUrls&quot;:{&quot;cloud&quot;:&quot;https://prod.cloud.rockstargames.com/&quot;,&quot;lifeInvader&quot;:&quot;https://www.lifeinvader.com&quot;,&quot;newswireHostName&quot;:&quot;https://www.rockstargames.com/&quot;,&quot;scHostName&quot;:&quot;socialclub.rockstargames.com&quot;},&quot;uiLib&quot;:{&quot;cdnBaseUrl&quot;:&quot;https://s.rsg.sc/sc/&quot;,&quot;avatarCloudBase&quot;:&quot;https://a.rsg.sc/&quot;,&quot;crewEmblemBaseUrl&quot;:null,&quot;defaultCrewEmblemUrl&quot;:&quot;https://s.rsg.sc/sc/images/emblems/128x128/rockstar1.png&quot;,&quot;crewEmblemUrl&quot;:&quot;https://prod.cloud.rockstargames.com/crews/sc/{0}/{1}/publish/emblem/emblem_{2}.png&quot;,&quot;muteConsole&quot;:false,&quot;rootId&quot;:null},&quot;preRender&quot;:null,&quot;errorState&quot;:null,&quot;ageGate&quot;:{&quot;uagcCookieName&quot;:&quot;UAGC&quot;,&quot;urgcCookieName&quot;:&quot;URGC&quot;,&quot;gatingAge&quot;:17,&quot;registrationGatingAge&quot;:13},&quot;feed&quot;:{&quot;infiniteScroll&quot;:true,&quot;readEnabled&quot;:true,&quot;writeEnabled&quot;:true},&quot;sharing&quot;:{&quot;facebook&quot;:true,&quot;twitter&quot;:true,&quot;reddit&quot;:true},&quot;rdr2&quot;:{&quot;pvcEnabled&quot;:true,&quot;pvcDisplayTotal&quot;:false,&quot;disableRoutesCssReloading&quot;:false,&quot;rdoMinHonorableReputation&quot;:800,&quot;couponRedemptionEnabled&quot;:true},&quot;ga&quot;:{&quot;propertyId&quot;:&quot;UA-15984839-29&quot;},&quot;rockstarGamesLauncher&quot;:{&quot;downloadUrl&quot;:&quot;https://gamedownloads.rockstargames.com/public/installer/Rockstar-Games-Launcher.exe&quot;},&quot;sentry&quot;:{&quot;dsn&quot;:&quot;https://9c63ab4e6cf94378a829ec7518e1eaf6@o432808.ingest.sentry.io/5403993&quot;,&quot;release&quot;:&quot;2020-12-14cjg_prod.sc&quot;,&quot;environment&quot;:&quot;prod&quot;,&quot;errorReporting&quot;:{&quot;enabled&quot;:true,&quot;sampleRate&quot;:1.0,&quot;ignoreErrors&quot;:[],&quot;denyUrls&quot;:[],&quot;allowUrls&quot;:[&quot;^https:\\/\\/((?!www|local).*)\\.rockstargames\\.com&quot;,&quot;^https:\\/\\/(signin-)?s\\.rsg\\.sc&quot;]},&quot;performanceTracing&quot;:{&quot;enabled&quot;:true,&quot;sampleRate&quot;:0.1,&quot;tracingOrigins&quot;:[&quot;^https://.*\\.scapi\\.rockstargames\\.com&quot;]}},&quot;webpack&quot;:{&quot;cdnOrigin&quot;:&quot;https://s.rsg.sc/sc&quot;,&quot;cdnPath&quot;:&quot;/js/20201212bfdb/build/&quot;},&quot;player&quot;:{&quot;sonyStoreRegion&quot;:&quot;SonyRegionAmerica&quot;}}"></script>

    
    

    

    

    

    
    <script type="text/javascript">
        var MTIProjectId='bb97f612-ac86-4ab1-9c29-80d577a6fc8a';
        (function() {
            var mtiTracking = document.createElement('script');
            mtiTracking.type='text/javascript';
            mtiTracking.async='true';
            mtiTracking.src=('https:'==document.location.protocol?'https:':'http:')+'//fast.fonts.net/t/trackingCode.js';
            (document.getElementsByTagName('head')[0]||document.getElementsByTagName('body')[0]).appendChild( mtiTracking );
        })();
    </script>

</body>
</html>
```