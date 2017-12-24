如果一个请求方法的语义实质上是只读的，那么它被视为“安全的”；即，客户端不请求，不期望在源服务器上任何状态的改变作为对目标资源应用安全方法的结果。同样合理的使用安全方法不会造成任何伤害，财产损失或者对源服务器的异常负担。

安全方法的定义没有组织实现包含可能有害的行为，它并非完全只读的，或当调用安全方法时造成副作用。然而，重要的是客户端没有请求额外的行为并且不能因此被追责。例如，大多数服务器在每个请求的完成时附加请求消息到访问日志文件，而不管请求方法，虽然日志存储可能填满存储而损坏服务器，但这被认为是安全的。同样，通过选择WEB上的一个广告而发起的安全请求通常将会有向广告账户收费的副作用。

本规范定义的GET，HEAD，OPTIONS，和TRACE请求方法被定义为安全的。

区别安全方法与非安全方法的目的是为了允许自动取回程序（爬虫）和缓存执行机制（预取）得以工作而不用担心造成危害。此外，它允许用户代理在处理可能不受信任的内容时对自动使用的非安全方法应用适当的限制。

用户代理在向用户呈现潜在的动作时**应该**区分安全和不安全方法，这样用户可以在请求它之前意识到这是不安全的行为。

当一个资源被构建为使得有效请求URI内的参数具有选择动作的效果时，资源所有者的责任是保证其行为与请求方法语义一致。例如，对于基于WEB的内容编辑软件来说，在查询参数中使用行为是很常见的，如“`page?do=delete`”。如果这种资源的目的是执行一个不安全的动作，那么当它被使用一个安全方法访问的时候，资源的拥有者**必须**禁用或者不允许那样的行为。如果没有这样做，当自动化程序为了链接维护，预取已经构建搜索索引等，在每个URI引用上执行GET时，将会造成未预料的的副作用。
