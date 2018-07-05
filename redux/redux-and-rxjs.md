[Ben Lesh - Async Redux Actions With RxJS](https://www.youtube.com/watch?v=sF5-V-Szo0c)

> Redux reducers handle state transitions, but they must be handled **synchronously**.

Async events: (Most of those asyncs can be handled synchronously)
* User interactions (mouse, keyboard, etc)
* AJAX
* Web Sockets
* Animations
* Workers

Some of the asyncs is harder than others:
* AJAX cancellation
* Composed AJAX
* Debounced form submissions
* Drag and drop

In redux, we can use middleware to manage asyncs by **callbacks** and **promises**.

> Callback hell (aka "the flying V")

 Promises:
 * Guaranteed Future
 * Immutable
 * Single value
 * Caching

 **Promises can't be cancelled**

 Why cancellation is important
 * Auto-complete
 * Changing views/routes before data finishes loading
 * Tearing down resources

 Observables
 * A set of events
 * Any number of values
 * Over any amount of time
 * Cancellable
 * Lazy

 RxJS
 > Lodash for async