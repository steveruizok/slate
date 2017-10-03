---
title: Framer-md Docs

language_tabs: # must be one of https://git.io/vQNgJ
  - coffeescript

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - app
  - header
  - type
  - button
  - notification

search: true
---

# Introduction

Welcome to Framer-md, a Material Design kit for [Framer](http://framer.com). Framer-md is made up of many smaller modules for components such as buttons, inputs and selectors. Some of these are designed to work together, but most can be dropped into your project as you need them.

Why use Framer-md? The kit is perfect for developing Android prototypes, of course, but the components are also handy for quickly knocking together interactions for usability testing, or placeholders for custom components, or even as templates for those custom components.

# Installation
```coffeescript
# create a button
myButton = new md.Button
```

Download the [Framer-md repository](http://github.com/steveruizok/framer-md). 

Copy the contents of the `framer-md/modules` folder into your project's `modules` folder.

Require the Framer-md kit into your project using `md = require 'md'`.

That's it! You now have access to all of the Framer-md components, all of which are available through the `md` object. For example, to create a new [Button](#button), type `myButton = new md.Button`.







