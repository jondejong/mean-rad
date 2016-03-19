## Angular
### Directives

    angular.module('myApp').directive('hello', function () {
     return {
       restrict: 'E',
       templateUrl: 'hello.template.html',
       link: function (scope, el, attrs) {
         scope.name = attrs.name;
       }
      };
    });
