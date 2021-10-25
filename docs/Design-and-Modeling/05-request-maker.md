# Try It

Stoplight Studio enables you to preview and test your API operations as you work or as people read your documentation.

<!--
focus: false
-->
![](../../assets/images/request-maker.png)

For each request, you can:

- Provide authorization and parameters as part of each request.
- Automatically generate a request code snippet for your preferred language type.
- Choose to send the request from any server defined in the API description.
- Enable mocking and choose to generate static or dynamic URLs. See [Mock Servers](06-mock-servers.md).  

## Send Requests

1. Open Try It:
    - From published API documentation, select an operation. 
    - In Edit mode, select an operation, select **Preview**, and then select the **Try It** tab. 
<!--
focus: false
-->
  ![](../../assets/images/open_try_it.png)

2. Provide Auth and parameters as required by the operation. 

3. Select a server for the request, if multiple servers are defined in your API description.

<!--
focus: false
-->
![](../../assets/images/send-request.png)

4. Select **Send Request**.

The response is returned.

<!-- theme: info -->
> Try It requests from browsers will be blocked for APIs that do not have appropriate [CORS headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) set up for *.http://stoplight.io.


## Generate Code Snippets

In the Request Sample box, select a language, and then select the copy icon.

<!--
focus: false
-->
  ![](../../assets/images/request-type.png)

The default language is **Shell / cURL**.

### Supported Languages

> These code snippets come from the open-source package [httpsnippet](https://github.com/Kong/httpsnippet), so if you'd like to contribute more, first send them a pull request then open an issue on [our GitHub repository](https://github.com/stoplightio/studio/issues).

Language | Library
---------|----------
Shell | cURL
Shell | HTTPie
Shell | Wget
Java | AsyncHttp
Java | NetHttp
Java | Unirest
Java | OkHttp
JavaScript | Fetch
JavaScript | XMLHttpRequest
JavaScript | jQuery
JavaScript | Axios
Node | Native
Node | Request
Node | Unirest
Node | Fetch
Node | Axios
PHP | curl
PHP | pecl/http 1
PHP | pecl/http 2
Python | Python 3
Python | Requests
Powershell | WebRequest
Powershell | RestMethod
R | |
Ruby | |
Go | |
C | |
C# | HttpClient
C# | RestSharp
Obj-C | |
Swift | |
OCaml | |
Http | |
Clojure | |
Kotlin | |



