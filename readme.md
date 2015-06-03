# ng-shadowbox

Angular directive to triggger `window.onbeforeunload()` based on a specified condition passed as the value of an attribute


## Attributes

* ngWarnOnUnload - Value Required. Defines the scope property to be evaluated in order to determine whether the user should be warned on unload
* ngWarnOnUnloadMsg - Optional. Defines the message to be returned from `onbeforeunload`



## Usage

HTML:

    <div ng-app="app" mng-controller="demoCtrl" ng-warn-on-unload="{{ !productForm.$pristine }}" ng-warn-on-unload-msg="You have made unsaved changes to this product.">

      <h1>ngWarnOnUnload demo</h1>

      <form name="productForm">
          <input type="text" ng-model="product.name">
          <input type="submit">
      </form>

    </div>

