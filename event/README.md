# EVENTS

## `preventDefault`
* cancels an event's default behavior if it is cancelable
* does not stop propagation
* prevent a checkbox from being toggled on click
   `checkbox.addEventListener('click', function (e) {e.preventDefault();})`
* [jsbin - preventDefault](http://jsbin.com/zegipo/edit?html,js,console,output)

## `stopPropagation`
* stops an event from bubbling up to its parent
* using `e.stopPropagation()` in a local handler will not later be handled via a higher delegation handler

## `target`
* `event.target` is the element on which the event occurred
* `event.currentTarget` is the element on which the the handler was attached

