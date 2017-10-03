# App
```coffeescript
md = require 'md'
# --------------

app = new md.App

myPage = new md.Page

app.showNext(myPage)
```

The App component is a modified FlowComponent, and is used for mobile Android application prototypes. It manages the interaction between seval other components, such as the header, footer, and menu overlay.

You don't need an App instance to use Framer-md, and most of the components in the kit work fine without it. Some components do require an App to work, or work differently if an App exists.

You can use App the same way you would a regular FlowComponent, however unlike a FlowComponent, it only works with instances of [Page](#Page) and [View](#View).