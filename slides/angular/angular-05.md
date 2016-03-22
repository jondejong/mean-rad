## Angular
### Controller

    angular.module('dogApp').controller('DogController', DogController);

    /** @ngInject */
    function DogController($http) {
      var ctrl = this;

      ctrl.dogs = [];

      ctrl.update = function() {
        $http.get('http://doglist.com/api/dogs').then(function(response) {
          ctrl.dogs = response.data;
        });
      }
    }
