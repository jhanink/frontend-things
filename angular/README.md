# ANGULAR

## `digest cycle`
* See [Understanding the Angular Digest Loop](http://techiejs.com/Blog/Post/Understanding-The-AngularJS-Digest-Loop)
* angular starts at root scope and examines all model properties on the watch list
  * it dirty checks by comparing new value to previous value
  * it is triggered by `$scope.digest()`, which is invoked by `$scope.$apply()`
  * angular directives and `angular` methods will result in a `$scope.$apply()` call
  * it processes the watch functions and then repeats the dirty checks until there are no changes
  * the loop is limited to 10 cycles to avoid an infinite loop, after which the application is killed

## `change detection and digest`
  * angular 1
    * change detection model graph has cycles
    * digest cycle loops until no more changes (or 10 elapsed cycles)
  * angular 2
    * change detection model is a tree
    * 1 digest (single cycle) pass only

## `directives`
* attribute values on isolated scope
  * `<div my-directive a="a" b="{{b}}" c="add(n)"></div>`
  * `scope: {a: "=", b: "@", c: "&"}`
  * `=` pass a parent-scoped value (can be a reference)
  * `@` pass a literal value expression 
  * `&` pass a wrapped expression (expression binding)
  * [see plunkr](https://plnkr.co/edit/2H2ecgWleNjP2n76KXdW)
* transclusion
  * [example](http://plnkr.co/edit/yFLe7OXj2u8epHXe6a0s?p=preview)

## `modules`

## `router`

## `extras`
* [Angular styleguide - john papa](https://github.com/johnpapa/angular-styleguide)
