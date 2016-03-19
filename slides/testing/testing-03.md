## Testing
### Jasmmine

Everything in one package

    describe('directive:hello', function () {
      var $compile, $rootScope;
      beforeEach(module('myApp'));

      beforeEach(inject(function (_$compile_, _$rootScope_) {
        $compile = _$compile_;
        $rootScope = _$rootScope_;
      }));

      it('Replaces the HTML content correctly', function () {
        var html = '<hello name="Jonny"></hello-person>';
        var element = $compile(html)($rootScope);
        $rootScope.$digest();
        expect(element.html()).toContain("Hello Jonny!!!");
      });
    });
