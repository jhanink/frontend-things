# HTML5

See [MDN - HTML5](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)

## `highlights`

* new elements, attributes, and behaviors
* a larger set of technologies -> _HTML5 & friends_ -> _HTML5_

### Semantics

Semantic HTML tags can indicate structure for document outlining or be typed elements that have specific meaning.

* Sections and outlines `<section> <article> <nav> <header> <footer>` 
* Audio and video `<audio> <video>` 
  * [video.js open source library](http://videojs.com/)
* Forms `<input> <output>`
* New elements `<figcaption> <data> <time> <output> <progress> <meter> <main>`
* MathML
* Misc..
  * `<datalist id="browsers"><option value="Chrome"></datalist><input type="text" list="browsers"/>`
  * `<iframe>` [See docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe#Attributes) 
    * `<iframe seamless="seamless"></iframe>`
    * `<iframe sandbox="allow-modals,allow-popups,allow-popups-to-escape-sandbox,allow-same-origin"></iframe>`


### Connectivity
* Web Sockets
* Server push
* WebRTC - realtime communication without plugins

### Offline and storage
* Offline resources - [Service Workers](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API/Using_Service_Workers) 
  * note: `application cache` has been deprecated
* Online, offline events - network connection detection
* client side session and persistent storage
* IndexedDB - store structured, indexed data in the browser
* File API - access local files

### Multimedia
* Audio, Video
* WebRTC
* Camera API

### 2D/3D graphics and effects
* Canvas
* Text API for `<canvas>`
* WebGL with `<canvas>`
* SVG - embed vector images in HTML

### Performance and integration
* Web Workers
* XMLHttpRequest - level 2
* History API - manipulate browser history
* `contentEditable` attribute

### Device access

### Styling

### Other
* `window.postMessage` - cross-frame/cross-domain messaging
* `offline/online events`
  * `window.addEventListener('offline', function(){console.log("you've gone offline")})`
  * `window.addEventListener('online', function(){console.log("you're back online")})`


