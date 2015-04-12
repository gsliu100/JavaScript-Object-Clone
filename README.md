# JavaScript-Object-Clone
Js中克隆对象的参考资料
*如何赋值一个对象a到另一个变量b，另一个变量b发生改变是原对象a不变。*

## 参考资料

   1. [what is the most efficient way to clone an object](http://stackoverflow.com/questions/122102/what-is-the-most-efficient-way-to-clone-an-object/5344074#534407)

   1. [cloning an object](http://web.archive.org/web/20140328224025/http://jsperf.com/cloning-an-object/2)

   1. [most elegant way to clone a javascript object](http://stackoverflow.com/questions/728360/most-elegant-way-to-clone-a-javascript-object)

   1. [how to copy javascript object to new variable not by reference](http://stackoverflow.com/questions/18359093/how-to-copy-javascript-object-to-new-variable-not-by-reference)

## 几种方法

  - 使用的方法.

    ```javascript
    //for  in
	for(var attr in oldObj){
		     var newOld={};
		     if(oldObj.hasOwlProprity(attr)){
		     newOld[attr]=oldObj[attr];
	     }
    }

	//JSON
	     var newObj=JSON.paser(JSON.stringify(oldObj));

	//jQuery
		浅拷贝
		var newObj=jQuery.extend({},old);
		深拷贝
		var newObj=jQuery.extend(true,{},old);
    ```

