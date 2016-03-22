## Angular
### Controller

    <div ng-controller="dogController as ctrl">
      <ul>
        <li ng-repeat="dog in ctrl.dogs">{{dog.name}}</li>
      </ul>
    </div>
    <div>
    <span class="btn btn-default" ng-click="ctrl.update()">Update</span>
