- [消息语法和路由](rfc7230/README.md)
    - [1. 介绍](rfc7230/Introduction/README.md)
        - [1.1 要求表示法](rfc7230/Introduction/Requirements_Notation.md)
        - [1.2 语法表示法](rfc7230/Introduction/Syntax_Notation.md)
    - [2. 结构](rfc7230/Architecture/README.md)
        - [2.1 客户端/服务器消息](rfc7230/Architecture/Client_Server_Messaging.md)
        - [2.2 实施多样性](rfc7230/Architecture/Implementation_Diversity.md)
        - [2.3 中介](rfc7230/Architecture/Intermediaries.md)
        - [2.4 缓存](rfc7230/Architecture/Caches.md)
        - [2.5 一致性和错误处理](rfc7230/Architecture/Conformance_and_Error_Handling.md)
        - [2.6 协议版本](rfc7230/Architecture/Protocol_Versioning.md)
        - [2.7 统一资源标识符](rfc7230/Architecture/Uniform_Resource_Identifiers/README.md)
            - [2.7.1 http URI格式](rfc7230/Architecture/Uniform_Resource_Identifiers/http_URI_Scheme.md)
            - [2.7.2 https URI格式](rfc7230/Architecture/Uniform_Resource_Identifiers/https_URI_Scheme.md)
            - [2.7.3 http和https URI规范化和比较](rfc7230/Architecture/Uniform_Resource_Identifiers/http_and_https_URI_Normalization_and_Comparison.md)
    - [3. 消息格式](rfc7230/Message_Format/README.md)
        - [3.1 开始行](rfc7230/Message_Format/Start_Line/README.md)
            - [3.1.1 请求行](rfc7230/Message_Format/Start_Line/Request_Line.md)
            - [3.1.2 状态行](rfc7230/Message_Format/Start_Line/Status_Line.md)
        - [3.2 头字段](rfc7230/Message_Format/Header_Fields/README.md)
            - [3.2.1 字段扩展性](rfc7230/Message_Format/Header_Fields/Field_Extensibility.md)
            - [3.2.2 字段顺序](rfc7230/Message_Format/Header_Fields/Field_Order.md)
            - [3.2.3 空白](rfc7230/Message_Format/Header_Fields/Whitespace.md)
            - [3.2.4 字段解析](rfc7230/Message_Format/Header_Fields/Field_Parsing.md)
            - [3.2.5 字段限制](rfc7230/Message_Format/Header_Fields/Field_Limits.md)
            - [3.2.6 字段值组件](rfc7230/Message_Format/Header_Fields/Field_Value_Components.md)
        - [3.3 消息体](rfc7230/Message_Format/Message_Body/README.md)
            - [3.3.1 传输编码](rfc7230/Message_Format/Message_Body/Transfer-Encoding.md)
            - [3.3.2 内容长度](rfc7230/Message_Format/Message_Body/Content-Length.md)
            - [3.3.3 消息体长度](rfc7230/Message_Format/Message_Body/Message_Body_Length.md)
        - [3.4 处理不完整消息](rfc7230/Message_Format/Handling_Incomplete_Messages.md)
        - [3.5 消息解析健壮性](rfc7230/Message_Format/Message_Parsing_Robustness.md)
    - [4. 传输编码](rfc7230/Transfer_Codings/README.md)
		- [4.1 分块传输编码](rfc7230/Transfer_Codings/Chunked_Transfer_Coding/README.md)
			- [4.1.1 分块扩展](rfc7230/Transfer_Codings/Chunked_Transfer_Coding/Chunk_Extensions.md)
			- [4.1.2 分块报尾部分](rfc7230/Transfer_Codings/Chunked_Transfer_Coding/Chunked_Trailer_Part.md)
			- [4.1.3 解码分块](rfc7230/Transfer_Codings/Chunked_Transfer_Coding/Decoding_Chunked.md)
		- [4.2 压缩编码](rfc7230/Transfer_Codings/Compression_Codings/README.md)
			- [4.2.1 Compress编码](rfc7230/Transfer_Codings/Compression_Codings/Compress_Coding.md)
			- [4.2.2 Deflate编码](rfc7230/Transfer_Codings/Compression_Codings/Deflate_Coding.md)
			- [4.2.3 Gzip编码](rfc7230/Transfer_Codings/Compression_Codings/Gzip_Coding.md)
		- [4.3 TE](rfc7230/Transfer_Codings/TE.md)
		- [4.4 Trailer](rfc7230/Transfer_Codings/Trailer.md)
    - [5. 消息路由](rfc7230/Message_Routing/README.md)
		- [5.1 识别目标资源](rfc7230/Message_Routing/Identifying_a_Target_Resource.md)
		- [5.2 连接入站](rfc7230/Message_Routing/Connecting_Inbound.md)
		- [5.3 请求目标](rfc7230/Message_Routing/Request_Target/README.md)
            - [5.3.1 原始形式](rfc7230/Message_Routing/Request_Target/origin-form.md)
			- [5.3.2 完整形式](rfc7230/Message_Routing/Request_Target/absolute-form.md)
			- [5.3.3 授权形式](rfc7230/Message_Routing/Request_Target/authority-form.md)
			- [5.3.4 星号形式](rfc7230/Message_Routing/Request_Target/asterisk-form.md)
		- [5.4 Host](rfc7230/Message_Routing/Host.md)
		- [5.5 有效的请求URI](rfc7230/Message_Routing/Effective_Request_URI.md)
		- [5.6 将响应与请求关联](rfc7230/Message_Routing/Associating_a_Response_to_a_Request.md)
		- [5.7 消息转发](rfc7230/Message_Routing/Message_Forwarding/README.md)
			- [5.7.1 Via](rfc7230/Message_Routing/Message_Forwarding/Via.md)
			- [5.7.2 转换](rfc7230/Message_Routing/Message_Forwarding/Transformations.md)
    - [6. 连接管理](rfc7230/Connection_Management/README.md)
		- [6.1 Connection](rfc7230/Connection_Management/Connection.md)
		- [6.2 建立](rfc7230/Connection_Management/Establishment.md)
	    - [6.3 保持](rfc7230/Connection_Management/Persistence/README.md)
            - [6.3.1 重试请求](rfc7230/Connection_Management/Persistence/Retrying_Requests.md)
            - [6.3.2 管道化](rfc7230/Connection_Management/Persistence/Pipelining.md)
        - [6.4 并发](rfc7230/Connection_Management/Concurrency.md)
        - [6.5 失败和超时](rfc7230/Connection_Management/Failures_and_Timeouts.md)
        - [6.6 销毁](rfc7230/Connection_Management/Tear-Down.md)
        - [6.7 Upgrade](rfc7230/Connection_Management/Upgrade.md)
    - [7. ABNF列表扩展：#规则](rfc7230/ABNF_List_Extension/README.md)
    - [8. IANA注意事项](rfc7230/IANA_Considerations/README.md)
        - [8.1 头字段注册](rfc7230/IANA_Considerations/Header_Field_Registration.md)
        - [8.2 URI方案注册](rfc7230/IANA_Considerations/URI_Scheme_Registration.md)
        - [8.3 互联网媒体类型注册](rfc7230/IANA_Considerations/Internet_Media_Type_Registration/README.md)
            - [8.3.1 互联网媒体类型message/http](rfc7230/IANA_Considerations/Internet_Media_Type_Registration/message_http.md)
            - [8.3.2 互联网媒体类型application/http](rfc7230/IANA_Considerations/Internet_Media_Type_Registration/application_http.md)
        - [8.4 传输编码注册](rfc7230/IANA_Considerations/Transfer_Coding_Registry/README.md)
            - [8.4.1 程序](rfc7230/IANA_Considerations/Transfer_Coding_Registry/Procedure.md)
            - [8.4.2 注册](rfc7230/IANA_Considerations/Transfer_Coding_Registry/Registration.md)
        - [8.5 内容编码注册](rfc7230/IANA_Considerations/Content_Coding_Registration.md)
        - [8.6 Upgrade令牌注册](rfc7230/IANA_Considerations/Upgrade_Token_Registration/README.md)
            - [8.6.1 程序](rfc7230/IANA_Considerations/Upgrade_Token_Registration/Procedure.md)
            - [8.6.2 注册](rfc7230/IANA_Considerations/Upgrade_Token_Registration/Upgrade_Token_Registration.md)
    - [9. 安全注意事项](rfc7230/Security_Considerations/README.md)
        - [9.1 建立权威](rfc7230/Security_Considerations/Establishing_Authority.md)
        - [9.2 中介的风险](rfc7230/Security_Considerations/Risks_of_Intermediaries.md)
        - [9.3 通过协议元素长度的攻击](rfc7230/Security_Considerations/Attacks_via_Protocol_Element_Length.md)
        - [9.4 响应分裂](rfc7230/Security_Considerations/Response_Splitting.md)
        - [9.5 请求走私](rfc7230/Security_Considerations/Request_Smuggling.md)
        - [9.6 信息完整性](rfc7230/Security_Considerations/Message_Integrity.md)
        - [9.7 消息机密性](rfc7230/Security_Considerations/Message_Confidentiality.md)
        - [9.8 服务器日志信息的隐私](rfc7230/Security_Considerations/Privacy_of_Server_Log_Information.md)
    - [10. 致谢](rfc7230/Acknowledgments/README.md)
    - [11. 引用](rfc7230/References/README.md)
        - [11.1 规范性参考](rfc7230/References/Normative_References.md)
        - [11.2 信息参考](rfc7230/References/Informative_References.md)
    - [附录A. HTTP版本历史](rfc7230/Appendix_A/README.md)
        - [A.1 从HTTP/1.0的改变](rfc7230/Appendix_A/Changes_from_http10/README.md)
            - [A.1.1 多宿主Web服务器](rfc7230/Appendix_A/Changes_from_http10/Multihomed_Web_Servers.md)
            - [A.1.2 Keep-Alive连接](rfc7230/Appendix_A/Changes_from_http10/Keep-Alive_Connections.md)
            - [A.1.3 Transfer-Encoding介绍](rfc7230/Appendix_A/Changes_from_http10/Introduction_of_Transfer-Encoding.md)
        - [A.2 从RFC2612的改变](rfc7230/Appendix_A/Changes_from_RFC_2612.md)
    - [附录B. 收集的ABNF](rfc7230/Appendix_B/README.md)
- [语义和内容](rfc7231/README.md)
    - [1. 介绍](rfc7231/Introduction/README.md)
        - [1.1 一致性和错误处理](rfc7231/Introduction/Conformance_and_Error_Handling.md)
        - [1.2 语法表示法](rfc7231/Introduction/Syntax_Notation.md)
    - [2. 资源](rfc7231/Resources/README.md)
    - [3. 表示](rfc7231/Representations/README.md)
        - [3.1 元数据表示](rfc7231/Representations/Representations_Metadata/README.md)
            - [3.1.1 处理表示数据](rfc7231/Representations/Representations_Metadata/Processing_Representation_Data.md)
            - [3.1.2 为压缩或完整性进行压缩](rfc7231/Representations/Representations_Metadata/Encoding_for_Compression_or_Integrity.md)
            - [3.1.3 观众语言](rfc7231/Representations/Representations_Metadata/Audience_Language.md)
            - [3.1.4 鉴定](rfc7231/Representations/Representations_Metadata/Identification.md)
        - [3.2 数据表示](rfc7231/Representations/Representation_Data.md)
        - [3.3 有效载荷语义](rfc7231/Representations/Payload_Semantics.md)
        - [3.4 内容协商](rfc7231/Representations/Content_Negotiation/README.md)
            - [3.4.1 主动协商](rfc7231/Representations/Content_Negotiation/Proactive_Negotiation.md)
            - [3.4.2 响应式协商](rfc7231/Representations/Content_Negotiation/Reactive_Negotiation.md)
    - [4. 请求方法](rfc7231/Request_Methods/README.md)
        - [4.1 概述](rfc7231/Request_Methods/Overview.md)
        - [4.2 通用方法属性](rfc7231/Request_Methods/Common_Method_Properties/README.md)
            - [4.2.1 安全方法](rfc7231/Request_Methods/Common_Method_Properties/Safe_Method.md)
            - [4.2.2 幂等方法](rfc7231/Request_Methods/Common_Method_Properties/Idempotent_Methods.md)
            - [4.2.3 可缓存方法](rfc7231/Request_Methods/Common_Method_Properties/Cacheable_Methods.md)
        - [4.3 方法定义](rfc7231/Request_Methods/Method_Definitions/README.md)
            - [4.3.1 GET](rfc7231/Request_Methods/Method_Definitions/GET.md)
            - [4.3.1 HEAD](rfc7231/Request_Methods/Method_Definitions/HEAD.md)
            - [4.3.1 POST](rfc7231/Request_Methods/Method_Definitions/POST.md)
            - [4.3.1 PUT](rfc7231/Request_Methods/Method_Definitions/PUT.md)
            - [4.3.1 DELETE](rfc7231/Request_Methods/Method_Definitions/DELETE.md)
            - [4.3.1 CONNECT](rfc7231/Request_Methods/Method_Definitions/CONNECT.md)
            - [4.3.1 OPTIONS](rfc7231/Request_Methods/Method_Definitions/OPTIONS.md)
            - [4.3.1 TRACE](rfc7231/Request_Methods/Method_Definitions/TRACE.md)
    - [5. 请求头字段](rfc7231/Request_Header_Fields/README.md)
        - [5.1 控制](rfc7231/Request_Header_Fields/Controls/README.md)
            - [5.1.1 Expect](rfc7231/Request_Header_Fields/Controls/Expect.md)
            - [5.1.2 Max-Forwards](rfc7231/Request_Header_Fields/Controls/Max-Forwards.md)
        - [5.2 条件语句](rfc7231/Request_Header_Fields/Conditional.md)
        - [5.3 内容协商](rfc7231/Request_Header_Fields/Content_Negotiation/README.md)
            - [5.3.1 质量值](rfc7231/Request_Header_Fields/Content_Negotiation/Quality_Values.md)
            - [5.3.2 Accept](rfc7231/Request_Header_Fields/Content_Negotiation/Accept.md)
            - [5.3.3 Accept-Charset](rfc7231/Request_Header_Fields/Content_Negotiation/Accept-Charset.md)
            - [5.3.4 Accept-Encoding](rfc7231/Request_Header_Fields/Content_Negotiation/Accept-Encoding.md)
            - [5.3.5 Accept-Language](rfc7231/Request_Header_Fields/Content_Negotiation/Accept-Language.md)
        - [5.4 认证证书](rfc7231/Request_Header_Fields/Authentication_Credentials.md)
        - [5.5 请求上下文](rfc7231/Request_Header_Fields/Request_Context/README.md)
            - [5.5.1 From](rfc7231/Request_Header_Fields/Request_Context/From.md)
            - [5.5.2 Referer](rfc7231/Request_Header_Fields/Request_Context/Referer.md)
            - [5.5.3 User-Agent](rfc7231/Request_Header_Fields/Request_Context/User-Agent.md)           
    - [6 响应状态码](rfc7231/Response_Status_Codes/README.md)
        - [6.1 状态码概述](rfc7231/Response_Status_Codes/Overview_of_Status_Codes/README.md)
        - [6.2 信息1xx](rfc7231/Response_Status_Codes/Informational_1xx/README.md)
            - [6.2.1 100 Continue](rfc7231/Response_Status_Codes/Informational_1xx/100_Continue.md)
            - [6.2.2 101 Switching Protocols](rfc7231/Response_Status_Codes/Informational_1xx/101_Switching_Protocols.md)
        - [6.3 成功2xx](rfc7231/Response_Status_Codes/Successful_2xx/README.md)
            - [6.3.1 200 OK](rfc7231/Response_Status_Codes/Successful_2xx/200_OK.md)
            - [6.3.2 201 Created](rfc7231/Response_Status_Codes/Successful_2xx/201_Created.md)
            - [6.3.3 202 Accepted](rfc7231/Response_Status_Codes/Successful_2xx/202_Accepted.md)
            - [6.3.4 203 Non-Authoritative Information](rfc7231/Response_Status_Codes/Successful_2xx/203_Non-Authoritative_Information.md)
            - [6.3.5 204 No Content](rfc7231/Response_Status_Codes/Successful_2xx/204_No_Content.md)
            - [6.3.6 205 Reset Content](rfc7231/Response_Status_Codes/Successful_2xx/205_Reset_Content.md)
        - [6.4 重定向3xx](rfc7231/Response_Status_Codes/Redirection_3xx/README.md)
            - [6.4.1 300 Multiple Choices](rfc7231/Response_Status_Codes/Redirection_3xx/300_Multiple_Choices.md)
            - [6.4.2 301 Moved Permanently](rfc7231/Response_Status_Codes/Redirection_3xx/301_Moved_Permanently.md)
            - [6.4.3 302 Found](rfc7231/Response_Status_Codes/Redirection_3xx/302_Found.md)
            - [6.4.4 303 See Other](rfc7231/Response_Status_Codes/Redirection_3xx/303_See_Other.md)
            - [6.4.5 305 Use Proxy](rfc7231/Response_Status_Codes/Redirection_3xx/305_Use_Proxy.md)
            - [6.4.6 306 (Unused)](rfc7231/Response_Status_Codes/Redirection_3xx/306_Unused.md)
            - [6.4.7 307 Temporary Redirect](rfc7231/Response_Status_Codes/Redirection_3xx/307_Temporary_Redirect.md)
        - [6.5 客户端错误4xx](rfc7231/Response_Status_Codes/Client_Error_4xx/README.md)
            - [6.5.1 400 Bad_Request](rfc7231/Response_Status_Codes/Client_Error_4xx/400_Bad_Request.md)
            - [6.5.2 402 Payment Required](rfc7231/Response_Status_Codes/Client_Error_4xx/402_Payment_Required.md)
            - [6.5.3 403 Forbidden](rfc7231/Response_Status_Codes/Client_Error_4xx/403_Forbidden.md)
            - [6.5.4 404 Not Found](rfc7231/Response_Status_Codes/Client_Errorr_4xx/404_Not_Found.md)
            - [6.5.5 405 Method Not Allowed](rfc7231/Response_Status_Codes/Client_Errorr_4xx/405_Method_Not_Allowed.md)
            - [6.5.6 406 Not Acceptable](rfc7231/Response_Status_Codes/Client_Errorr_4xx/406_Not_Acceptable.md)
            - [6.5.7 408 Request Timeout](rfc7231/Response_Status_Codes/Client_Errorr_4xx/408_Request_Timeout.md)
            - [6.5.8 409 Conflict](rfc7231/Response_Status_Codes/Client_Errorr_4xx/409_Conflict.md)
            - [6.5.9 410 Gone](rfc7231/Response_Status_Codes/Client_Errorr_4xx/410_Gone.md)
            - [6.5.10 411 Length Required](rfc7231/Response_Status_Codes/Client_Errorr_4xx/411_Length_Required.md)
            - [6.5.11 413 Payload Too Large](rfc7231/Response_Status_Codes/Client_Errorr_4xx/413_PayloadToo_Large.md)
            - [6.5.12 414 URI Too Long](rfc7231/Response_Status_Codes/Client_Errorr_4xx/414_URIToo_Long.md)
            - [6.5.13 415 Unsupported Media Type](rfc7231/Response_Status_Codes/Client_Errorr_4xx/415_Unsupported_Media_Type.md)
            - [6.5.14 417 Expectation Failed](rfc7231/Response_Status_Codes/Client_Errorr_4xx/417_Expectation_Failed.md)
            - [6.5.15 426 Upgrade Required](rfc7231/Response_Status_Codes/Client_Errorr_4xx/426_Upgrade_Required.md)
        - [6.6 服务器错误5xx](rfc7231/Response_Status_Codes/Server_Errorr_5xx/README.md)
            - [6.6.1 500 Internal Server Error](rfc7231/Response_Status_Codes/Server_Errorr_5xx/500_Internal_Server_Error.md)
            - [6.6.2 501 Not Implemented](rfc7231/Response_Status_Codes/Server_Errorr_5xx/501_Not_Implemented.md)
            - [6.6.3 502 BadGateway](rfc7231/Response_Status_Codes/Server_Errorr_5xx/502_Bad_Gateway.md)
            - [6.6.4 503 Service Unavailable](rfc7231/Response_Status_Codes/Server_Errorr_5xx/503_Service_Unavailable.md)
            - [6.6.5 504 Gateway Timeout](rfc7231/Response_Status_Codes/Server_Errorr_5xx/504_Gateway_Timeout.md)
            - [6.6.6 505 HTTP Version Not Supported](rfc7231/Response_Status_Codes/Server_Errorr_5xx/505_HTTP_Version_Not_Supported.md)
    - [7 响应头字段](rfc7231/Response_Header_Fields/README.md)
        - [7.1 控制数据](rfc7231/Response_Header_Fields/Control_Data/README.md)
            - [7.1.1 组织日期](rfc7231/Response_Header_Fields/Control_Data/Origination_Date.md)
            - [7.1.2 Location](rfc7231/Response_Header_Fields/Control_Data/Location.md)
            - [7.1.3 Retry-After](rfc7231/Response_Header_Fields/Control_Data/Retry-After.md)
            - [7.1.4 Vary](rfc7231/Response_Header_Fields/Control_Data/Vary.md)
        - [7.2 验证器头字段](rfc7231/Response_Header_Fields/Validator_Header_Fields.md)
        - [7.3 认证挑战](rfc7231/Response_Header_Fields/Authentication_Challenges.md)
        - [7.4 响应上下文](rfc7231/Response_Header_Fields/Response_Context/README.md)
            - [7.4.1 Allow](rfc7231/Response_Header_Fields/Response_Context/Allow.md)
            - [7.4.2 Server](rfc7231/Response_Header_Fields/Response_Context/Server.md)
    - [8 IANA注意事项](rfc7231/IANA_Considerations/README.md)
        - [8.1 方法注册](rfc7231/IANA_Considerations/Method_Registry/README.md)
            - [8.1.1 程序](rfc7231/IANA_Considerations/Method_Registry/Procedure.md)
            - [8.1.2 新方法注意事项](rfc7231/IANA_Considerations/Method_Registry/Considerations_for_New_Methods.md)
            - [8.1.3 注册](rfc7231/IANA_Considerations/Method_Registry/Registrations.md)
        - [8.2 状态码注册](rfc7231/IANA_Considerations/Status_Code_Registry/README.md)
            - [8.2.1 程序](rfc7231/IANA_Considerations/Status_CodeRegistry/Procedure.md)
            - [8.2.2 新状态码注册注意事项](rfc7231/IANA_Considerations/Status_Code_Registry/Considerations_for_New_Status_Codes.md)
            - [8.2.3 注册](rfc7231/IANA_Considerations/Status_Code_Registry/Registrations.md)
        - [8.3 头字段注册](rfc7231/IANA_Considerations/Header_Field_Registry/README.md)
            - [8.3.1 新头字段注册注意事项](rfc7231/IANA_Considerations/Header_FieldRegistry/Considerations_for_New_HeaderFields.md)
            - [8.3.2 注册](rfc7231/IANA_Considerations/Header_FieldRegistry/Registrations.md)
        - [8.4 内容编码注册](rfc7231/IANA_Considerations/Content_Coding_Registry/README.md)
            - [8.4.1 程序](rfc7231/IANA_Considerations/Content_Coding_Registry/Procedure.md)
            - [8.4.2 注册](rfc7231/IANA_Considerations/Content_Coding_Registry/Registrations.md)
    - [9 安全注意事项](rfc7231/Security_Considerations/README.md)
        - [9.1 基于文件和路径名的攻击](rfc7231/Security_Considerations/Attacks_Based_on_File_and_Path_Names.md)
        - [9.2 基于命令、代码或查询注入的攻击](rfc7231/Security_Considerations/Attacks_Based_on_Command_Code_or_Query_Injection.md)
        - [9.3 个人信息泄露](rfc7231/Security_Considerations/Disclosure_of_Personal_Information.md)
        - [9.4 敏感信息URI泄露](rfc7231/Security_Considerations/Disclosure_of_Sensitive_Information_in_URIs.md)
        - [9.5 重定向后片段泄露](rfc7231/Security_Considerations/Disclosure_of_Fragment_after_Redirects.md)
        - [9.6 产品信息泄露](rfc7231/Security_Considerations/Disclosure_of_Product_Information.md)
        - [9.7 浏览器指纹](rfc7231/Security_Considerations/Browser_Finger_printing.md)
    - [10 致谢](rfc7231/Acknowledgments/README.md)
    - [11 引用](rfc7231/References/README.md)
        - [11.1 规范引用](rfc7231/References/Normative_References.md)
        - [11.2 信息引用](rfc7231/References/Informative_References.md)
    - [附录A MIME与HTTP的区别)(rfc7231/Appendix_A/README.md)
        - [A.1 MIME版本](rfc7231/Appendix_A/MIME-Version.md)
        - [A.2 转换为规范形式](rfc7231/Appendix_A/Conversion_to_Canonical_Form.md)
        - [A.3 日期格式转换](rfc7231/Appendix_A/Conversion_of_Date_Formats.md)
        - [A.4 Content-Enconding的转换](rfc7231/Appendix_A/Conversion_of_Content-Encoding.md)
        - [A.5 Content-Transfer-Encoding的转换](rfc7231/Appendix_A/Conversion_of_Content-Transfer-Encoding.md)
        - [A.6 MHTML和行长度限制](rfc7231/Appendix_A/MHTML_and_Line_Length_Limitations.md)
    - [附录B 从RFC2616的改变](rfc7231/Appendix_B/README)
    - [附录C 导入的ABNF](rfc7231/Appendix_B/README.md)
    - [附录D 收集的ABNF](rfc7231/Appendix_B/README.md)

- [条件请求](rfc7232/README.md)
- [范围请求](rfc7233/README.md)
- [缓存](rfc7234/README.md)
- [认证](rfc7235/README.md)
