当一个消息没有Transfer-Encoding头字段时，Content-Length头字段可以通过一个十进制数字为潜在的有效载荷体提供预期尺寸。对于的确包含有效载荷体的消息来说，Content-Length字段的值提供了确定结束正文（和消息）结束所需的构成消息。对于没有包含有效载荷体的消息，Content-Length表示所选表示的大小。

> ```
>  Content-Length = 1*DIGIT
> ```

例如：`Content-Length: 3495`

发送者**不得**在任何包含Transfer-Encoding头字段的消息中发送Content-Length头字段。

当请求的方法为封闭有效载荷体定义了一个含义并且Transfer-Encoding没有被发送，用户代理**应该**在请求消息中发送Content-Length。例如，Content-Length头字段一般应该在POST请求中发送，即使它的值是0（指示一个空的有效载荷体）。当请求消息不包含有效载荷体并且方法语义没有预期这样一个主体的时候，用户代理**不应该**发送Content-Length头字段。

服务器**可能**在对HEAD请求（RFC7231中4.3.2节）的响应中发送一个Content-Length头字段；在这样的响应中，除非它的值等于用GET方法的相同请求的响应中将要发送的有效载荷体的字节十进制数，否则服务器**不得**发送Content-Length。

服务器**可能**在对条件GET请求（RFC7232的4.1节）的304（未修改）响应中发送一个Content-Length      头字段；在这样的相应中，除非他的字段值等于将要子啊相同请求的200（正确）响应的有效载荷体中发送的字节十进制数，否则服务器**不得**发送Content-Length。

在状态码为1xx（信息）或204（无内容）的响应中，服务器**不得**发送Content-Length头字段。服务器**不得**在对CONNECT请求（RFC7231的4.3.6节）的任何2xx（成功）响应中发送任何Content-Length头字段。

除了上面定义的情况，在没有Transfer-Encoding的时，当有效载荷体尺寸在发送完整的头部份之前能够知道的话，源服务器**应该**发送Content-Length头字段。这将允许下游接收者度量传输进程，知道什么时候被接收的消息是完整的，并且可以为另外的请求重用连接。

任何大于等于零的Content-Length字段值都是有效的。应为没有对有效载荷体长度的预定义限制，接收者**必须**预期尽可能大的十进制数，防止因为整数转换溢出（9.3节）造成的解析错误。

如果一个消息接收到具有由相同十进制值组成的的字段值的多个Content-Length头字段，或者一个具有包含一串相同十进制数值的字段值（例如：“Content-Length: 42, 42”）的单独的Content-Length头字段，说明重复的Content-Length头字段已经被生成或者被上游消息处理者组合，那么接收者**必须**因无效而拒绝该消息或者以一个单独的有效的Content-Length字段取代重复的字段值，这个字段包含预先决定消息体长度的十进制数字，或转发这个消息。

*注意：对于消息的构成，HTTP使用Content-Length与MIME中使用相同字段有明显的不同，在MIME中它仅仅是在“message/external-body”媒体类型内使用的可选字段。*