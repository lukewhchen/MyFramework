# MyFramework

MyFramework is a lightweight MVC framework developed with Ruby and inspired by Rails. MVC stands for Model-View—Controller. It’s a paradigm, allowing developers to factor out the various components of an application and more easily update them.

## ControllerBase

- **render(template_name):** Render a template located in the app/views/<controller_name> directory.
![](https://github.com/lukewhchen/MyFramework/blob/master/docs/render.png)
![](https://github.com/lukewhchen/MyFramework/blob/17e72ed260b857cd9d3dcda59a9d62402559b9b2/lib/controller_base.rb#L45-L57)
- **render_content(content, content_type):** Render custom content with the specified content_type.

- **redirect_to(url):** Redirect to the passed URL.

- **session:** key/value pairs saved to this hash are saved as cookies.

- **flash and flash.now:** key/values pairs saved to this hash will persist through the next session and the current
session only, respectively.

- **protect_from_forgery:** MyFramework will check for an authenticity token in any submitted data. This token can be added to the forms in your views.

## Router

- The Router allows the mapping of routes to your custom controllers.

## Rack Middleware

- **Exceptions** provides a detailed error message for any errors, which is useful for development.

- **StaticAssets** allows the serving of static assets from the public folder. Supported extensions are .jpg, .txt, .zip, and .html.
