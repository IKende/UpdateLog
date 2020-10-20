## Beetlex相关组件功能计划/更新日志
- **?** `BeetleX.Tracks.`
    - 用于定义代码执行跟踪链处理。

- **?** `BeetleX.FastHttpApi.EFCore.Extension`
    - 支持直接在WebApi方法中定义efcore dbcontext参数，并可标记方法是否使用事务。
- **?**`BeetleX.FastHttpApi.Cached`
    - 控制器缓存插件
- **?** `BeetleX.Bumblebee`
    - 增加总入口的RPS请求限制控制
---
- **2020-10-15** `BeetleX.FastHttpApi 1.8.8.4`
    - [bug]`BinaryResult`处理存在问题!
    - 支持返回`return (new ArraySegment<byte>(data, 0, data.Length), "image/jpeg");`
    - 控制器处理浏览器用websocket发大数据分帧问题
    - 增加会话的http请求并发限制
---
- **2020-10-4** `BeetleX 1.5.5.3`
    -  AwaiterClient对象添加`Task<T> Receive<T>`和`Task<T> ReceiveFrom<T>`方法。
    -  AsyncTcpClient对象增加索引器，用于自定义信息存储。
    -  增加`IMessageSubmitHandler`接口，用于描述消息写入到流后触发的行为
---

- **2020-9-28** `BeetleX 1.5.4.6`
    - IServer增加索引器用于保存服务全局信息。
    - AsyncClient增加awaiter receive pipestream功能。

---

- **2020-9-25** `BeetleX.FastHttpApi 1.8.7.2`
    - ParameterBinderAttribute限制了泛型扩展，改成非Attribute。
    - 添加控制器支持自定义后缀
---

- **2020-9-23** `BeetleX.EFCore.Extension 0.6`
    - 创建Command的时候添加DBContext的事务对象
---

- **2020-9-21** `BeetleX.FastHttpApi 1.8.6.7`
    - 增加总入口的RPS请求限制控制
---
- **2020-9-13** `BeetleX 1.5.4`
    - Listen添加标签属性
    - Session来源于那个Listen
---
- **2020-9-9** `BeetleX.FastHttpApi 1.8.6.5`
    - 添加`ActionContext`类型参数注入支持
    - `ActionContext`添加`HasError`属性,用于获取当前请求是否有未处理的异常
    - `IActionParameter`加入`ActionContext`属性和`Init`方法
---
- **2020-9-7** `BeetleX.FastHttpApi.VueExtend 0.8.0`
    - 支持单个`WebResource`资源来源于多个程序集
---
- **2020-9-6** `BeetleX.Bumblebee 1.4.2.2`
    - `Route`添加`ReplacePattern` 和`ReplacePath`用于转发时替换请求路径
---
-  **2020-9-5** `BeetleX.FastHttpApi v1.68`
    - 支持`Cookie`的`SameSite`配置
    - 加入`BinaryResult`用于定义输出二进制内容
    - `TextResult`加入`AutoGzip`支持,可以配置当内容大于1K的情况自动使用`Gzip`输出。
----------------

- **2020-9-3** `BeetleX.Http.Clients 1.2.7`
    - 更新`BeetleX v1.5.3.2`
----------------
- **2020-8-31**`BeetleX.Bumblebee.Configuration 1.4.3.9`
    - 添加进程管理模块
---
- **2020-8-30** `BeetleX.Bumblebee 1.4.1.2`
    - 支持进程管理，自动附加服务进程并添加到网关中
-----

- **2020-8-27** `BeetleX v1.5.3.2`
    -  `socket.accept `错误的时候进行一个重试
    - `client`移除`ReciveFrom`等方法




