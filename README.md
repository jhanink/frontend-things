# Frontend Things

Ideas about frontend tech and design

## Instant Search

Display search results (10 at a time under the search box) as you type in a fast and efficient manner.

A basic strategy
* on keyup, send the query term to the search engine, get results, display results

Some potential issues
* Fast typing by many concurrent users will add load on the search server
* request roundtrips may be "slow"
* asynchronous requests may come back out of order

Some possible optimizations
* on page load, prefetch search results (data-size: 26 x 10)
* to reduce load, throttle requests (e.g. 100ms) to make request rate per client more predictable
* "ignore" async requests made earlier than the "last" request
* if not throttling, prefetch "next" results so that subsequent letters are ready and waiting
* on the server, store top results in a fast key/value LRU cache
* use socket.io for realtime push

domain specific optimizations
* for a general search engine, cache known/top/popular searches from other people

personalization
* for a logged in user, predictive search results can be ranked based on a user's search history

## UI design language

* use simple, clear, uncluttered, consistent, and pleasing design language
   * see material design
* create affordances for the user
* a design is not finished when there is nothing left to add but when there is nothing left to take away
* use indicators only when something needs to be indicated
   * small splashes of color or notifications to draw user attention where and when needed
* provide feedback, like progress indicators, result confirmations, validation/error messages, etc.
* offer simple single-step operations instead of complicated, multi-layered behaviors.
* remember user preferences

