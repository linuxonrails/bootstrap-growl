bootstrap-growl
===============

Pretty simple jQuery plugin that turns standard Bootstrap alerts into hovering "Growl-like" notifications.

###Demo

I have a basic demo set up at jsfiddle for the time being which you can view here: http://jsfiddle.net/tkB69/

###Features

* Uses standard [Twitter Bootstrap alerts](http://twitter.github.com/bootstrap/components.html#alerts) which provides 'info', 'error', and 'success' styles.
* Multiple growls called consecutively are stacked up one after another in a list.
* Automatically fades growls away after a default of 4 seconds.

###Dependencies

1. Latest version of jQuery. (tested on 1.7.2)
2. [Twitter Bootstrap](http://twitter.github.com/bootstrap/index.html). (tested on 2.0.3)

###Usage

Include the dependencies and `jquery.bootstrap-growl.min.js` into your page and call the following:

```javascript
$.bootstrapGrowl("My message");
```

###Available Options

By default, growls use the Bootstrap 'info' style, are 250px wide, right aligned, and are positioned 20px from the top right of the page.

```javascript
$.bootstrapGrowl("another message, yay!", {
  type: 'info', // (null, 'info', 'error', 'success')
  top_offset: 20,
  align: 'right', // ('left', 'right', or 'center')
  width: 250, // (integer, or 'auto')
  delay: 4000,
  allow_dismiss: true,
  stackup_spacing: 10 // spacing between consecutive stacecked growls.
});
```
