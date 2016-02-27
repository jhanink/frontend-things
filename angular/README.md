# ANGULAR

## `digest cycle`
* See [Understanding the Angular Digest Loop](http://techiejs.com/Blog/Post/Understanding-The-AngularJS-Digest-Loop)
* angular starts at root scope and examines all model properties on the watch list
  * it dirty checks by comparing new value to previous value
  * it is triggered by `$scope.digest()`, which is invoked by `$scope.$apply()`
  * angular directives and `angular` methods will result in a `$scope.$apply()` call

## `modules`

## `directives`

## `router`
