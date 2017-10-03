# Header
The Header component is an Android mobile header. It may be set with a title, an icon, and an action to be performed when the icon is tapped.

Header is designed to work with the [App](#App) component, which will create a Header instance by default. When the App component changes pages, the Header is automatically set with information on its new current page. 

**Note:** If you've created an App component, you do not need to also create a Header.

## Creating a Header
```coffeescript
header = new md.Header
  title: 'Welcome to Framer-Md'
  icon: 'menu'
  action: -> print "menu icon tapped!"
```

When creating a new Header, you may set its initial properties using the `title`, `icon`, and `action` options. 

You can also use standard Layer options: `backgroundColor` will set the background for the header, while `color` will set the color of the title, icon, and statusBar.


## header.title
```coffeescript
header = new md.Header

header.title = 'Hello World!'
```

The `title` property sets the text shown on the header. 

The color of the title can be set with `header.color`.

#### Default: `'Header'`


## header.icon
```coffeescript
header = new md.Header

header.icon = 'star'
```
The `icon` property sets the icon shown at the header's left hand side. 

It works the same as a regular `md.Icon`. For more about that component, and what the valid icon names are, see the [Icon](#icon) section of these docs. 

The color of the icon can be set with `header.color`.

#### Default: `'menu'`


## header.action
```coffeescript
header = new md.Header

header.action = -> print 'Hello world!'
```
The `action` property sets the callback function that will run when a user taps the header's icon.

#### Default: `-> null`



## header.setHeader( <span style="color:#777">options</span> )
```coffeescript
header = new md.Header

Utils.delay 3, ->
	header.setHeader
		title: 'whaddup world'
		icon: 'arrow-back'
		action: -> print 'Should go back!'
		backgroundColor: '#FF0077'
```

To create a transition effect, use the `setHeader` method. The header's current icon and title will fade out, change to the new values, and fade back in.

In addition to the properties above, you can use the `setHeader` method to set any other properties, such as `visible` or `backgroundColor`.