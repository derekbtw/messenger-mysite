# Struck Messenger
Facebook Messenger on your website

Demo: http://struck.io/messenger | [Getting Started]

### Version
3.2.7

This is a tiny package that lets you add Facebook Messenger to your website for chat functionality with almost zero installation. The chat icon opens a chat window with you from messenger.com (m.me). This can be done with Pages and personal accounts. It will also direct them to a chat with you in Messenger if they're on iOS as well. I haven't tested this with Android yet.


[![](http://i.imgur.com/6wYl59g.png)](http://struck.io/messenger)

[![](http://i.imgur.com/Gcw3B4P.png)](http://struck.io/messenger)

This is still in the early stages so contributing to the project is greatly appreciated! Maybe some more icon templates?

### Getting Started

* Upload all the things to the root of your site, or just the CSS and JS assuming your site is already built.
* Include this on your pages. [Balloon.css] is recommended so people know what the button does.

```html
<link href="css/balloon.min.css" rel="stylesheet"> <!-- optional tooltips -->
<link href="css/struck-messenger.css" rel="stylesheet">
```
```html
<script src="js/struck-messenger.min.js"></script>
```

* Paste this somewhere on your pages like the footer with your Facebook username included in the URL.

```html   
<!-- left messenger -->
<a class="popup" href="https://m.me/[your Facebook username]">
  <div id="m-ios">
    <div class="messenger-ios hvr-grow" data-balloon="Chat with us!" data-balloon-pos="right"></div>
  </div>
</a>

<!-- right messenger -->
<a class="popup" href="https://m.me/[your Facebook username]">
  <div id="m-android">
    <div class="messenger-android hvr-float" data-balloon="Chat with us!" data-balloon-pos="left"></div>
  </div>
</a>
```

* Lastly, initialize it with some settings. More settings can be found in /js/struck-messenger.js

```html
<script type="text/javascript"> 
  $('.popup').popupWindow({ 
    height:500, 
    width:640, 
    centerScreen:1
  }); 
</script>
```

* That's it!

PSD files are included in the /img directory (with a demo logo by [Freepik] from [Flaticon]) for your chat icons. Make sure you read the [Facebook Messenger Branding Guidelines] before you make one.

License
----

MIT


   [Getting Started]: <https://github.com/struck-io/messenger#getting-started>
   [Balloon.css]: <http://kazzkiq.github.io/balloon.css/>
   [Facebook Messenger Branding Guidelines]: <https://developers.facebook.com/docs/messenger/brand-guidelines>
   [Freepik]: <http://www.freepik.com/>
   [Flaticon]: <http://www.flaticon.com/>
