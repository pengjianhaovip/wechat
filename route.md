#路由解析
入口脚本程序获取到到URL中相关的GET参数，解析后进行权限判断，然后调用相应的控制器处理这个请求。该过程就被称为URL路由（routing）。

约定及使用GET 参数中的 c、a、do为微擎系统的路由参数，应当避免与系统参数冲突，在程序中可以使用 $controller、$action、$do来获取对应的路由三个参数

地址URL地址路由
当传入的URL请求中包含一个名为 c、a、do(可选) 的 GET 参数，它即被视为一个路由，例如：

http://we7.cc/web/index.php?c=platform&a=menu&
则会路由至 /web/source/platform/menu.ctrl.php 文件中

http://we7.cc/app/index.php?c=mc&a=home&
则会路由至 /app/source/mc/home.ctrl.php 文件中







模块URL地址路由
当传入的 c 值为 “site”, a 值为 “entry”时则是一个模块路由，例如：

http://we7.cc/web/index.php?c=site&a=entry&do=themeset&m=we7_demo
则会路由至 /addons/we7_demo/site.php 文件中的 doWebThemeset() 方法。

http://we7.cc/app/index.php?i=1&j=2&c=entry&do=list&m=ewei_shopping
则会路由至 /addons/we7_demo/site.php 文件中的 doMobileList() 方法。





