rhapsody
========

This is a "loosely coupled module dependency" framework. The idea is that you can create a module by doing:

rhapsody.define("moduleName", function () {
    return {
        someMethod: function () {
           //  ... do something
        }
    };
});


and then you can use the module as:

rhapsody.use("moduleName", function(m) {
  m.someMethod();
});

