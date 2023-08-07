<html><head>
    <meta charset="utf-8">
    <title>layuimini-iframe版 v2 - 基于Layui的后台管理系统前端模板</title>
    <meta name="keywords" content="layuimini,layui,layui模板,layui后台,后台模板,admin,admin模板,layui mini">
    <meta name="description" content="layuimini基于layui的轻量级前端后台管理框架，最简洁、易用的后台框架模板，面向所有层次的前后端程序,只需提供一个接口就直接初始化整个框架，无需复杂操作。">
    <meta name="renderer" content="webkit">
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
    <meta http-equiv="Access-Control-Allow-Origin" content="*">
    <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
    <meta name="apple-mobile-web-app-status-bar-style" content="black">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="format-detection" content="telephone=no">
    <link rel="icon" href="images/favicon.ico">
    <link rel="stylesheet" href="lib/layui-v2.5.5/css/layui.css" media="all">
    <link rel="stylesheet" href="css/layuimini.css?v=2.0.4.2" media="all">
    <link rel="stylesheet" href="css/themes/default.css" media="all">
    <link rel="stylesheet" href="lib/font-awesome-4.7.0/css/font-awesome.min.css" media="all">
    <!--[if lt IE 9]>
    <script src="https://cdn.staticfile.org/html5shiv/r29/html5.min.js"></script>
    <script src="https://cdn.staticfile.org/respond.js/1.4.2/respond.min.js"></script>
    <![endif]-->
    <style id="layuimini-bg-color">
    </style><style id="layuimini-page-anim">.layui-tab-item.layui-show {animation:moveTop 1s;-webkit-animation:moveTop 1s;animation-fill-mode:both;-webkit-animation-fill-mode:both;position:relative;height:100%;-webkit-overflow-scrolling:touch;}
@keyframes moveTop {0% {opacity:0;-webkit-transform:translateY(30px);-ms-transform:translateY(30px);transform:translateY(30px);}
    100% {opacity:1;-webkit-transform:translateY(0);-ms-transform:translateY(0);transform:translateY(0);}
}
@-o-keyframes moveTop {0% {opacity:0;-webkit-transform:translateY(30px);-ms-transform:translateY(30px);transform:translateY(30px);}
    100% {opacity:1;-webkit-transform:translateY(0);-ms-transform:translateY(0);transform:translateY(0);}
}
@-moz-keyframes moveTop {0% {opacity:0;-webkit-transform:translateY(30px);-ms-transform:translateY(30px);transform:translateY(30px);}
    100% {opacity:1;-webkit-transform:translateY(0);-ms-transform:translateY(0);transform:translateY(0);}
}
@-webkit-keyframes moveTop {0% {opacity:0;-webkit-transform:translateY(30px);-ms-transform:translateY(30px);transform:translateY(30px);}
    100% {opacity:1;-webkit-transform:translateY(0);-ms-transform:translateY(0);transform:translateY(0);}
}</style>
<link id="layuicss-layer" rel="stylesheet" href="http://layuimini.99php.cn/iframe/v2/lib/layui-v2.5.5/css/modules/layer/default/layer.css?v=3.1.1" media="all"></head>
<body class="layui-layout-body layuimini-all layuimini-multi-module">
<div class="layui-layout layui-layout-admin">

    <div class="layui-header header">
        <div class="layui-logo layuimini-logo"><a href=""><img src="images/logo.png" alt="logo"><h1>LAYUI MINI</h1></a></div>

        <div class="layuimini-header-content">
            <a>
                <div class="layuimini-tool"><i title="展开" class="fa fa-outdent" data-side-fold="1"></i></div>
            </a>

            <!--电脑端头部菜单-->
            <ul class="layui-nav layui-layout-left layuimini-header-menu layuimini-menu-header-pc layuimini-pc-show"><li data-menu="multi_module_0" class="layui-nav-item menu-li undefined layui-this" id="multi_module_0HeaderId"> <a href="javascript:;"> <span class="layui-left-nav">常规管理</span></a>  </li><li data-menu="multi_module_1" class="layui-nav-item menu-li undefined " id="multi_module_1HeaderId"> <a href="javascript:;"> <span class="layui-left-nav">组件管理</span></a>  </li><li data-menu="multi_module_2" class="layui-nav-item menu-li undefined " id="multi_module_2HeaderId"> <a href="javascript:;"> <span class="layui-left-nav">其它管理</span></a>  </li><span class="layui-nav-bar"></span></ul>

            <!--手机端头部菜单-->
            <ul class="layui-nav layui-layout-left layuimini-header-menu layuimini-mobile-show">
                <li class="layui-nav-item">
                    <a href="javascript:;"><i class="fa fa-list-ul"></i> 选择模块<span class="layui-nav-more"></span></a>
                    <dl class="layui-nav-child layuimini-menu-header-mobile"><dd class="menu-dd undefined undefined"> <a href="javascript:;" data-menu="multi_module_0" id="multi_module_0HeaderId">  <i class="fa fa-address-book"></i>  <span class="layui-left-nav"> 常规管理</span></a> </dd><dd class="menu-dd undefined undefined"> <a href="javascript:;" data-menu="multi_module_1" id="multi_module_1HeaderId">  <i class="fa fa-lemon-o"></i>  <span class="layui-left-nav"> 组件管理</span></a> </dd><dd class="menu-dd undefined undefined"> <a href="javascript:;" data-menu="multi_module_2" id="multi_module_2HeaderId">  <i class="fa fa-slideshare"></i>  <span class="layui-left-nav"> 其它管理</span></a> </dd></dl>
                </li>
            <span class="layui-nav-bar"></span></ul>

            <ul class="layui-nav layui-layout-right">

                <li class="layui-nav-item" lay-unselect="">
                    <a href="javascript:;" data-refresh="刷新"><i class="fa fa-refresh"></i></a>
                </li>
                <li class="layui-nav-item" lay-unselect="">
                    <a href="javascript:;" data-clear="清理" class="layuimini-clear" data-href="api/clear.json"><i class="fa fa-trash-o"></i></a>
                </li>
                <li class="layui-nav-item mobile layui-hide-xs" lay-unselect="">
                    <a href="javascript:;" data-check-screen="full"><i class="fa fa-arrows-alt"></i></a>
                </li>
                <li class="layui-nav-item layuimini-setting">
                    <a href="javascript:;">admin<span class="layui-nav-more"></span></a>
                    <dl class="layui-nav-child">
                        <dd>
                            <a href="javascript:;" layuimini-content-href="page/user-setting.html" data-title="基本资料" data-icon="fa fa-gears">基本资料<span class="layui-badge-dot"></span></a>
                        </dd>
                        <dd>
                            <a href="javascript:;" layuimini-content-href="page/user-password.html" data-title="修改密码" data-icon="fa fa-gears">修改密码</a>
                        </dd>
                        <dd>
                            <hr>
                        </dd>
                        <dd>
                            <a href="javascript:;" class="login-out">退出登录</a>
                        </dd>
                    </dl>
                </li>
                <li class="layui-nav-item layuimini-select-bgcolor" lay-unselect="">
                    <a href="javascript:;" data-bgcolor="配色方案"><i class="fa fa-ellipsis-v"></i></a>
                </li>
            <span class="layui-nav-bar" style="left: 233.125px; top: 60px; width: 0px; opacity: 0;"></span></ul>
        </div>
    </div>

    <!--无限极左侧菜单-->
    <div class="layui-side layui-bg-black layuimini-menu-left"><ul class="layui-nav layui-nav-tree layui-left-nav-tree layui-this" id="multi_module_0"><li class="layui-nav-item menu-li  "> <a target="_self" href="javascript:;"> <i class="fa fa-home"></i>  <span class="layui-left-nav">主页模板</span><span class="layui-nav-more"></span></a>  <dl class="layui-nav-child "><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/welcome-1.html" target="_self">  <i class="fa fa-tachometer"></i>  <span class="layui-left-nav"> 主页一</span></a> </dd><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/welcome-2.html" target="_self">  <i class="fa fa-tachometer"></i>  <span class="layui-left-nav"> 主页二</span></a> </dd><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/welcome-3.html" target="_self">  <i class="fa fa-tachometer"></i>  <span class="layui-left-nav"> 主页三</span></a> </dd></dl>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/menu.html" target="_self" href="javascript:;"> <i class="fa fa-window-maximize"></i>  <span class="layui-left-nav">菜单管理</span></a>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/setting.html" target="_self" href="javascript:;"> <i class="fa fa-gears"></i>  <span class="layui-left-nav">系统设置</span></a>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/table.html" target="_self" href="javascript:;"> <i class="fa fa-file-text"></i>  <span class="layui-left-nav">表格示例</span></a>  </li><li class="layui-nav-item menu-li  "> <a target="_self" href="javascript:;"> <i class="fa fa-calendar"></i>  <span class="layui-left-nav">表单示例</span><span class="layui-nav-more"></span></a>  <dl class="layui-nav-child "><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/form.html" target="_self">  <i class="fa fa-list-alt"></i>  <span class="layui-left-nav"> 普通表单</span></a> </dd><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/form-step.html" target="_self">  <i class="fa fa-navicon"></i>  <span class="layui-left-nav"> 分步表单</span></a> </dd></dl>  </li><li class="layui-nav-item menu-li  "> <a target="_self" href="javascript:;"> <i class="fa fa-flag-o"></i>  <span class="layui-left-nav">登录模板</span><span class="layui-nav-more"></span></a>  <dl class="layui-nav-child "><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/login-1.html" target="_blank">  <i class="fa fa-stumbleupon-circle"></i>  <span class="layui-left-nav"> 登录-1</span></a> </dd><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/login-2.html" target="_blank">  <i class="fa fa-viacoin"></i>  <span class="layui-left-nav"> 登录-2</span></a> </dd><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/login-3.html" target="_blank">  <i class="fa fa-tags"></i>  <span class="layui-left-nav"> 登录-3</span></a> </dd></dl>  </li><li class="layui-nav-item menu-li  "> <a target="_self" href="javascript:;"> <i class="fa fa-home"></i>  <span class="layui-left-nav">异常页面</span><span class="layui-nav-more"></span></a>  <dl class="layui-nav-child "><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/404.html" target="_self">  <i class="fa fa-hourglass-end"></i>  <span class="layui-left-nav"> 404页面</span></a> </dd></dl>  </li><li class="layui-nav-item menu-li  "> <a href="javascript:;"> <i class="fa fa-snowflake-o"></i>  <span class="layui-left-nav">其它界面</span><span class="layui-nav-more"></span></a>  <dl class="layui-nav-child "><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/button.html" target="_self">  <i class="fa fa-snowflake-o"></i>  <span class="layui-left-nav"> 按钮示例</span></a> </dd><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/layer.html" target="_self">  <i class="fa fa-shield"></i>  <span class="layui-left-nav"> 弹出层</span></a> </dd></dl>  </li><span class="layui-nav-bar"></span></ul><ul class="layui-nav layui-nav-tree layui-left-nav-tree layui-hide" id="multi_module_1"><li class="layui-nav-item menu-li  "> <a layuimini-href="page/icon.html" target="_self" href="javascript:;"> <i class="fa fa-dot-circle-o"></i>  <span class="layui-left-nav">图标列表</span></a>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/icon-picker.html" target="_self" href="javascript:;"> <i class="fa fa-adn"></i>  <span class="layui-left-nav">图标选择</span></a>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/color-select.html" target="_self" href="javascript:;"> <i class="fa fa-dashboard"></i>  <span class="layui-left-nav">颜色选择</span></a>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/table-select.html" target="_self" href="javascript:;"> <i class="fa fa-angle-double-down"></i>  <span class="layui-left-nav">下拉选择</span></a>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/upload.html" target="_self" href="javascript:;"> <i class="fa fa-arrow-up"></i>  <span class="layui-left-nav">文件上传</span></a>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/editor.html" target="_self" href="javascript:;"> <i class="fa fa-edit"></i>  <span class="layui-left-nav">富文本编辑器</span></a>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/area.html" target="_self" href="javascript:;"> <i class="fa fa-rocket"></i>  <span class="layui-left-nav">省市县区选择器</span></a>  </li><span class="layui-nav-bar"></span></ul><ul class="layui-nav layui-nav-tree layui-left-nav-tree layui-hide" id="multi_module_2"><li class="layui-nav-item menu-li  "> <a href="javascript:;"> <i class="fa fa-meetup"></i>  <span class="layui-left-nav">多级菜单</span><span class="layui-nav-more"></span></a>  <dl class="layui-nav-child "><dd class="menu-dd  "> <a href="javascript:;" target="_self">  <i class="fa fa-calendar"></i>  <span class="layui-left-nav"> 按钮1</span><span class="layui-nav-more"></span></a>  <dl class="layui-nav-child "><dd class="menu-dd  "> <a href="javascript:;" target="_self">  <i class="fa fa-snowflake-o"></i>  <span class="layui-left-nav"> 按钮2</span><span class="layui-nav-more"></span></a>  <dl class="layui-nav-child "><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/button.html?v=3" target="_self">  <i class="fa fa-snowflake-o"></i>  <span class="layui-left-nav"> 按钮3</span></a> </dd><dd class="menu-dd  "> <a href="javascript:;" layuimini-href="page/form.html?v=1" target="_self">  <i class="fa fa-calendar"></i>  <span class="layui-left-nav"> 表单4</span></a> </dd></dl> </dd></dl> </dd></dl>  </li><li class="layui-nav-item menu-li  "> <a layuimini-href="page/error.html" target="_self" href="javascript:;"> <i class="fa fa-superpowers"></i>  <span class="layui-left-nav">失效菜单</span></a>  </li><span class="layui-nav-bar"></span></ul></div>

    <!--初始化加载层-->
    <div class="layuimini-loader" style="display: none;">
        <div class="layuimini-loader-inner"></div>
    </div>

    <!--手机端遮罩层-->
    <div class="layuimini-make"></div>

    <!-- 移动导航 -->
    <div class="layuimini-site-mobile"><i class="layui-icon"></i></div>

    <div class="layui-body">

        <div class="layuimini-tab layui-tab-rollTool layui-tab" lay-filter="layuiminiTab" lay-allowclose="true">
            <ul class="layui-tab-title">
                <li class="layui-this" id="layuiminiHomeTabId" lay-id="page/welcome-1.html?t=1"><span class="layuimini-tab-active"></span><span class="disable-close">首页</span><i class="layui-icon layui-unselect layui-tab-close">ဆ</i></li>
            </ul>
            <div class="layui-tab-control">
                <li class="layuimini-tab-roll-left layui-icon layui-icon-left"></li>
                <li class="layuimini-tab-roll-right layui-icon layui-icon-right"></li>
                <li class="layui-tab-tool layui-icon layui-icon-down">
                    <ul class="layui-nav close-box">
                        <li class="layui-nav-item">
                            <a href="javascript:;"><span class="layui-nav-more"></span></a>
                            <dl class="layui-nav-child layui-anim layui-anim-upbit">
                                <dd><a href="javascript:;" layuimini-tab-close="current">关 闭 当 前</a></dd>
                                <dd><a href="javascript:;" layuimini-tab-close="other">关 闭 其 他</a></dd>
                                <dd><a href="javascript:;" layuimini-tab-close="all">关 闭 全 部</a></dd>
                            </dl>
                        </li>
                    <span class="layui-nav-bar" style="left: 0px; top: 35px; width: 0px; opacity: 0;"></span></ul>
                </li>
            </div>
            <div class="layui-tab-content">
                <div id="layuiminiHomeTabIframe" class="layui-tab-item layui-show"><iframe width="100%" height="100%" frameborder="no" border="0" marginwidth="0" marginheight="0" src="page/welcome-1.html?t=1"></iframe></div>
            </div>
        </div>

    </div>
</div>
<script src="https://hm.baidu.com/hm.js?d97abf6d61c21d773f97835defbdef4e"></script><script src="lib/layui-v2.5.5/layui.js" charset="utf-8"></script>
<script src="js/lay-config.js?v=2.0.0" charset="utf-8"></script>
<script>
    layui.use(['jquery', 'layer', 'miniAdmin','miniTongji'], function () {
        var $ = layui.jquery,
            layer = layui.layer,
            miniAdmin = layui.miniAdmin,
            miniTongji = layui.miniTongji;

        var options = {
            iniUrl: "api/init.json",    // 初始化接口
            clearUrl: "api/clear.json", // 缓存清理接口
            urlHashLocation: true,      // 是否打开hash定位
            bgColorDefault: false,      // 主题默认配置
            multiModule: true,          // 是否开启多模块
            menuChildOpen: false,       // 是否默认展开菜单
            loadingTime: 0,             // 初始化加载时间
            pageAnim: true,             // iframe窗口动画
            maxTabNum: 20,              // 最大的tab打开数量
        };
        miniAdmin.render(options);

        // 百度统计代码，只统计指定域名
        miniTongji.render({
            specific: true,
            domains: [
                '99php.cn',
                'layuimini.99php.cn',
                'layuimini-onepage.99php.cn',
            ],
        });

        $('.login-out').on("click", function () {
            layer.msg('退出登录成功', function () {
                window.location = 'page/login-3.html';
            });
        });
    });
</script>


</body></html>
