Flex Widget: Perspective Modal Dialogs
=============

![Perspective Dialogs Preview](http://www.beatbrokerz.com/flex/widget/fwperspective/preview.png)

This widget adds a cool twist on the presentation of modal dialogs in your app. Instead of the standard modal dialog, if the browser supports 3d transitions, this widget will perform a 3d effect to 'unhide' modal dialogs. In the event that the screen size is too small or the browser doesn't support the effect, then the standard modal dialog will display as usual.

* [**LIVE DEMO** (jsfiddle.net)](http://jsfiddle.net/beatbrokerz/KSmPk/)

### Pre-requisites

This widget requires a [flex app](http://www.beatbrokerz.com/flex) to be installed to your webpage in order for it to do anything useful. Refer to the [flex installation guide](http://www.beatbrokerz.com/flex/start) for more information on how to set up your own music app.

Once you have a flex app installed on your page, follow these steps to use this widget:

### Autoload Usage

This widget can be auto-loaded from the Beat Brokerz CDN. Use the following url in your autoload settings:

```
//www.beatbrokerz.com/flex/widget/fwperspective/widget.js
```

> You can use the [widget autoloader](http://www.beatbrokerz.com/flex/start/settings#autoloader) feature in your flex app settings (on Beat Brokerz) to autoload this widget automatically on every page your flex app is installed to.
>
> Or you can autoload it selectively on your pages using javascript:
> ```javascript
> flexloader.autoload('//www.beatbrokerz.com/flex/widget/fwperspective/widget.js');
> ```


### Widget Files / Controlled Loading

If you want to load this widget from your own server or you want to explicitly control the resources that get loaded on your page, you'll need to do the following:

1. Download the widget package [.zip file](https://github.com/beatbrokerz/flex-fwperspective/archive/master.zip)
2. Extract the contents and upload the files/folders to a public location on your webserver.

* fwperspective/widget.js (autoload ready)
* fwperspective/widget.css

If you choose not to autoload, then you'll need to manually reference the required resources in your page like so:

> ```html
> <script type="text/javascript" src="/path/to/fwperspective/widget.js"></script>
> <link rel="stylesheet" type="text/css" href="/path/to/fwperspective/widget.css" />
> ```

### Usage Instructions

Once the widget is loaded on your page, it will transform modal dialogs automatically where it is able to. There is no need to embed anything in your page.

### Widget Settings

This widget does not have settings.


### Theme & Structure Reference

The widget wraps html around the body of your page to acheive the 3d effect. Once it is loaded, it restructures your page body based on the following structure and css classing:

```html
<div class="bbflex-page-body">
  <div id="fwperspective" class="fwperspective effect-airbnb">
    <div class="fwperspective-container">
      <div class="fwperspective-wrapper">
        <!-- page body ends up here -->
      </div>
    </div>
    <div class="fwperspective-modal-wrapper fwmodal left vertical">
      <!-- modal dialog content ends up here -->
    </div>
  </div>
</div>

```
