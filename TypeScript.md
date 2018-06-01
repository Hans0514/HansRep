TypeScript

一、字符串新特性
  1、多行字符串

  	var content = "aaabb"+
  	  "bbccc"


  	  var content = `aaa
  	   bbb
  	   ccc`

  2、字符串模板

  	var myname="zhai liang";
  	var getName=function(){
  		return "zhai liang"
  	}

  	console.log(`hello ${myname}`);
  	console.log(`hello ${getName()}`);

  3、自动拆分字符串

    function test(template,name,age)
    {
    	console.log(template);
    	console.log(name);
    	console.log(age);
    }

    var myname = "zhai liang";

    var getAge = function(){return 18;}

    test`hello my name is ${name},I'm ${getAge()}`

二、参数新特性
	1、参数类型
		在参数名称后面使用冒号来指定了参数类型
		var myname : string = "zhai liang";

		var age :number =123;

		var man : boolen = true;

	    function test(name:string):void { }


	    class Person {
	    	name:string;
	    	age ：number;
	    }

	    var zhangsan:person = new Person()

	2、参数默认值
		在参数声明后面使用冒号来指定参数的默认值
		function test(a:string,b:string,d:string="jojo"):void{
		}

	3、可选参数
		在方法的参数声明后面用问号标明此参数为可选参数

三、函数新特性
	1、Rest and Spread 操作符：
		用来声明任意数量的方法参数

		function func1(...args){ }









