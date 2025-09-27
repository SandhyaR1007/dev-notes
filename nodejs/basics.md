# basics of node js
- Node.js is a runtime environment built to use javascript outside the browser.
- It is nothing but a Javascript engine combined with C++ program.

- Modules in Node 
1. Built-in modules -> These are provided by node itself. e.g. fs, path, os etc.
2. External(3rd party) modules -> These are the ones we download. e.g. jsonwebtoken, axios etc.
3. Custom modules -> These are created by us.

- Module Wrapper
Before executing a module's code node js wraps the code in a anonymous function providing it a private scope.
-- definition--
(function(exports,require, module, __filename, __dirname ){ // module wrapper
    // module's code
})
- exports: object used to export value of the module.
- require: function used to import other modules.
- module: the module object itself.
- __filename: absolute path of current module file.
- __dirname: absolute path of directory containing module file.