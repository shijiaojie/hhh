获取字节码文件对象
	1:对象名.getClass()
	2:类名.class属性
	3:Class.forName("包名.类名")
获取构造方法
	Class的成员方法:
		getConstructor(Class...objs)	-> Constructor
		getConstructors()	-> Constructor[]
		
		getDeclaredConstructor(Class...objs)	-> Constructor
		getDeclaredConstructors()	-> Constructor[] 
		newInstance()	->	Object
		
	Constructor成员方法
		newInstance(Object...objs)	->	Object
获取成员变量
	Class的成员方法:
		getField(Object obj)	->	Field
		getFields()	->	Field[]
		
		getDeclaredField("age")	->	Field
		getDeclaredFields()	->	Field[]
	
	Field的成员方法
		set(Object obj,Object value)
		get(Object obj)		->	Object
		
获取成员方法
	Class的成员方法:
		getMethod()	-> Method
		getMethods() ->	Method[]	获取自己的以及从父类或父接口中继承/实现过来的public修饰的成员方法对象
		
		getDeclaredMethod()	-> Method 
		getDeclaredMethods() -> Method[]	获取的自己的任意修饰符修饰的成员方法对象
		
	Method的成员方法:
		invoke(Object obj,Object...params) ->	Object 
		
定义Javabean规范
BeanUtils工具类的使用
	setProperty(Object bean,String name,Object value)
	getProperty(Object bean,String name)
	populate(Object bean,Map m)

改写自定义BeanUtils工具类的set/get/populate方法
