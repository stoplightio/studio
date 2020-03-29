# Request Maker

Stoplight Studio has a built in HTTP client which we call Request Maker. It appears in a few places throughout our ecosystem, and in Studio you will see it under the "Try it Now" button in **Preview**.

![](../../assets/images/request-maker.png)

The request maker is very much like many other HTTP clients out there, but it knows all about your APIs. It knows every endpoint defined in the API description, it knows what headers need are required or optional, what content type you should send, and if the API description has defined servers, it will let you pick from those. 

When you edit the API description, this Try it Now tab will update as you save. This lets you make requests to your development server whilst you work on it, without needing to jump between multiple applications and update things in multiple places.

## Design-First

If you are following the design-first workflow, you can make requests to a [mock server](./06-mock-servers.md). This helps you get a feel for how the API will work, before writing any code.

## Code-First

If you are following the code-first workflow, you can make requests to your existing servers to get an idea of how they look, and speed up the creation of your API descriptions.

## Contract Violations

When you've got both a running server, and an API description for an API, request maker will be able to report any discrepencies between the two.

![](../../assets/images/request-maker-results.png)

Sending it a parameter it doesn't know about, sending data of the wrong type, even getting a response from the server with properties not mentioned in the API description, will all trigger a little warning like the one above.
