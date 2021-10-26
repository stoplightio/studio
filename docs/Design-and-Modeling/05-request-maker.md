# Try It

Stoplight Studio enables you to preview and test your API operations as you work or as people read your documentation.

For each request, you can:

- Provide authorization and parameters as part of each request.
- Choose to send the request from any server defined in the API description.
- Get a [request sample](05a-generating-code-snippets.md) for your preferred language type.
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


