# Router

Router 的主体是 pathname 的管理和传递。

在单页应用中，一般所有 pathname 对应的逻辑全部由一个 HTML 页面完成。故：

- 在应用初始化的时候，应用程序可以第一时间获取当前的 pathname。
  - 若借由 SPA 路由不友好的静态托管（腾讯云云开发）搭建应用，可以通过 redirector.html 作为路由中转，此时，应用程序应该在初始化的时候对相关参数进行处理，并将处理的结果妥善地传递给应用主体。
- 初始化完成之后，在应用运行过程中，应用程序可以不间断获取最新的 pathname。

应用启动 -> 判断 mobius_redirect ->
