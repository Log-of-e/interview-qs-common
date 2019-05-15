


### Why/What is prototype.constructor re-defined/for? [ES5]

When setting the prototype, the prototype.constructor gets overwritten. This _CAN_ becomes an issue when using the `new` operatior as in:
 var O2 = new Foo();
 reference: exploringjs.com/es6/ch_classes.html, https://stackoverflow.com/questions/17886395/what-is-prototype-constructor-for
 


When must `super` be called?
 1. Almost always for subclass constructor, (ie when using  `extends`) 

When can a subclass skip calling `super` in its construction?
 1. When returning an Object : `return {}` or `return Object.create(null)`
 2. OR: if there is no explicitly defined `constructor` method
 
 
