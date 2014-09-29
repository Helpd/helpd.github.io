###Notes on layouts.

Layouts can use inheritance, so to keep things clear (and avoid unexpected behaviour), please log how layouts work here.

- `box.html` - simple layout used for error pages and small pieces of text.
  - `redirect.html` - based on the `box` layout, used to provide the pretty redirection page.

- - -

####redirect.html
This layout doesn't parse any content, only populating the manual redirect link and the meta refresh tag. As such, redirected pages (doing a redirect to) need only be as follows:

```
---
layout: redirect
redirect: http://example.com/page-to-redirect-to
---
```
