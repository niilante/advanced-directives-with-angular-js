# Advanced Directives with Angular JS

This repository is the companion to two screencasts:

[Part One](https://www.youtube.com/watch?v=Ty8XcASK9js) examines some of the more advanced features in Angular, specifically Directives and how we can leverage the power of custom elements and attributes to map Domain Specific concepts through HTML, translate those into Value Objects in our Domain, and gain rendered simple HTML output. Also discussed: complexity, creating a DSL with directives, debugging techniques, tips and tricks. This screencast covers:

* html as a dsl
* abstractions in html
* [$compile](https://docs.angularjs.org/api/ng/service/$compile)
* [$templateRequest](https://docs.angularjs.org/api/ng/service/$templateRequest)
* [$templateCache](https://docs.angularjs.org/api/ng/service/$templateCache)
* [directive definition object](https://docs.angularjs.org/api/ng/service/$compile#directive-definition-object)
* [requiring other directives](https://docs.angularjs.org/api/ng/service/$compile#-require-)
* [directive communication ($scope.$broadcast, $scope.$on)](https://docs.angularjs.org/guide/scope#scope-events-propagation)

[Part Two](https://www.youtube.com/watch?v=4zG8SfucUzg) continues the examination of some of the advanced features in Part 1. This screencast covers:

* bugfixes for the inline editor
* auto toggling of editing state using CSS content generation and the angular $scope
* leveraging the DSL from the first screencast as an interface to a 3rd party JavaScript data grid component: js-grid

If you're interested in some more context prior to watching check out my other [angular screencasts](http://www.youtube.com/user/vidjadavemo/videos) and an earlier post on the [power of web components as abstractions](http://blog.testdouble.com/posts/2013-06-26-what-polymer-and-angular-tell-us-about-the-future-success-of-the-web-platform-and-javascript-frameworks.html); 


# Running the Code Locally

I like to use the npm module [serve](https://github.com/zeit/serve) for running a simple static webserver for projects like this:

```shell
npm i -g serve
git clone git@github.com:davemo/advanced-directives-with-angular-js.git
cd advanced-directives-with-angular-js
serve
```

# Extra Credit

~~Some things in the screencast aren't complete and some things could definitely done better. This section is a challenge to you, the reader/watcher to improve the code and level up your knowledge in the process! Try and tackle some of these challenges if you want:~~

* ~~Bugfix: the editor currently shows up multiple times, fix it so this doesn't happen (hint: maybe an 'edit' state that's tracked could help the directive know if it should execute `.insertAfter`)~~ [Fixed Here](https://github.com/davemo/advanced-directives-with-angular-js/commit/4efc9edfacc3cee791f155d52bf517a7ab251586)
* ~~Feature: make the expandy arrow thing point down when expanded and to the right when collapsed.~~ [Added Here](https://github.com/davemo/advanced-directives-with-angular-js/commit/2f046f51dda4b54891353b7ec047b3a6e381792d)

