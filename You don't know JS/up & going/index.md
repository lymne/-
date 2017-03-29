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