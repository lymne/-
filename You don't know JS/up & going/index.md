<h1>up & going</h1>

<ul>
	<li><strong>1.什么值会判断为false？</strong>
		<p> 空字符串"", 0, NAN, null, undefined, false
		</p>	
	</li>
	<li><strong>new String("a") == new String("a")</strong>
		<p> false
		</p>	
	</li>
	<li><strong>什么情况下使用 == 或者 ===</strong>
		<p> If you can be certain about the values, and == is safe, use it! If you can't be certain about the values, use ===. It's that simple.
		</p>	
	</li>
	<li><strong>闭包简述</strong>
		<p> 当一个函数执行完毕仍然可以记住和继续获得该函数作用域内的变量，闭包的主要作用是模块化开发，隐藏变量和方法，只对外公布api
		</p>	
	</li>
	<li><strong>this 相关</strong>
		<p> 
			If a function has a this reference inside it, that this reference usually points to an object. But which object it points to depends on how the function was called.

			It's important to realize that this does not refer to the function itself, as is the most common misconception. （在函数里面的this，并不是指引用函数自身）			
		</p>	
		<p>
			Closely related to the this keyword is the object prototype mechanism, which is a look-up chain for properties, similar to how lexical scope variables are found. But wrapped up in the prototypes is the other huge miscue about JS: the idea of emulating (fake) classes and (so-called "prototypal") inheritance.

            Unfortunately, the desire to bring class and inheritance design pattern thinking to JavaScript is just about the worst thing you could try to do, because while the syntax may trick you into thinking there's something like classes present, in fact the prototype mechanism is fundamentally opposite in its behavior.
		</p>
	</li>
		
</ul>

<h1>types & grammar</h1>
<ul>
	<li><strong>值 & 引用</strong>
		<p>在 Javascript 中，值的类型决定了值是value-copy还是reference-copy </p>
		<p>Simple values (aka scalar primitives) are always assigned/passed by value-copy: null, undefined, string, number, boolean, and ES6's symbol</p>
		<p>But both c and d are separate references to the same shared value [1,2,3], which is a compound value. It's important to note that neither c nor d more "owns" the [1,2,3] value -- both are just equal peer references to the value. So, when using either reference to modify (.push(4)) the actual shared array value itself, it's affecting just the one shared value, and both references will reference the newly modified value [1,2,3,4].</p>
	</li>
	<li><strong>NAN</strong>
		<p>NAN的类型是Number </p>
	</li>
</ul>

<h1>this & Object Prototypes</h1>
<ul>
	<li><strong>CH1 this 初认识</strong>
		<p>首先，this 不是词法作用域,是运行时绑定的。与函数在哪里声明无关，而是取决于函数在哪里被调用</p>
		<p>
			We said earlier that this is not an author-time binding but a runtime binding. It is contextual based on the conditions of the function's invocation. this binding has nothing to do with where a function is declared, but has instead everything to do with the manner in which the function is called.
		</p>
		<p>
			this is actually a binding that is made when a function is invoked, and what it references is determined entirely by the call-site where the function is called.
		</p>
		<p>词法作用域（静态作用域）是在<b>书写代码</b>或者说定义时确定的，而动态作用域是在<b>运行时</b>确定的。<br>词法作用域关注函数在<b>何处声明</b>，而动态作用域关注函数从<b>何处调用</b>，其作用域链是基于运行时的调用栈的。</p>
		
	</li>
	<li><strong>NAN</strong>
		<p>NAN的类型是Number </p>
	</li>
</ul>