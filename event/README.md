# EVENTS

## `preventDefault`
* cancels an event's default behavior if it is cancelable
* does not stop propagation
* prevent a checkbox from being toggled on click
   `checkbox.addEventListener('click', function (e) {e.preventDefault();})`
* [jsbin - preventDefault](http://jsbin.com/zegipo/edit?html,js,console,output)

## `target`
* `event.target` is the element on which the event occurred
* `event.currentTarget` is the element on which the the handler was attached

