# Publishing in Studio

Whenever changes are made to your API descriptions or Markdown documentation, whether that is done in Stoplight Studio or anywhere else, you want to get those changes reflected in Documentation, Mock Servers, Explorer, the Design Library, etc.

In Studio v1.x publishing was done by clicking the "Publish" button, but with the launch of Stoplight Platform publishing can be [automated using Webhooks, or Continuous Integration](https://meta.stoplight.io/docs/platform/2.-workspaces/g.automating-publishing.md). 

## Published Documentation URL

If you click the Publish button in Studio Desktop v1.x, your documentation will go here:

```
https://stoplight.io/p/docs/gh/{org}/{project}
```

If you have created a workspace on [Stoplight Platform](https://stoplight.io/welcome) then you no longer need to click that button (it'll be gone when you upgrade to Studio Desktop v2.0 anyway) and the documentation will instead be over here.

```
https://{workspace}.stoplight.io/docs/{project}
```

_If you need any help migrating from the old documentation to the new documentation, please [contact support](mailto:support@stoplight.io)._
