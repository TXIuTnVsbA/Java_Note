# Java基础

------
**Java 关键字**

|类别|关键字|说明|
|:---:|:---:|:---:|
|访问控制|	private	|私有的|
||protected	|受保护的|
||public|	公共的|
|类、方法和变量修饰符|	abstract|	声明抽象|
||class|	类|
||extends|	扩允,继承|
||final|	最终值,不可改变的|
||implements|	实现（接口）|
||interface|	接口|
||native	|本地，原生方法（非Java实现）|
||new|	新,创建|
||static|	静态|
||strictfp|	严格,精准|
||synchronized|	线程,同步|
||transient|	短暂|
||volatile|	易失|
|程序控制语句|	break|	跳出循环|
||case|	定义一个值以供switch选择|
||continue|	继续|
||default|	默认|
||do|	运行|
||else|	否则|
||for|	循环|
||if|	如果|
||instanceof|	实例|
||return|	返回|
||switch|	根据值选择执行|
||while|	循环|
|错误处理|	assert|	断言表达式是否为真|
||catch|	捕捉异常|
||finally|	有没有异常都执行|
||throw	|抛出一个异常对象|
||throws|	声明一个异常可能被抛出|
||try|	捕获异常|
|包相关|	import	|引入|
||package|	包|
|基本类型|	boolean	|布尔型|
||byte|	字节型|
||char|	字符型|
||double|	双精度浮点|
||float|	单精度浮点|
||int|	整型|
||long|	长整型|
||short|	短整型|
|变量引用|	super|	父类,超类|
||this|	本类|
||void|	无返回值|
|保留关键字|	goto|	是关键字，但不能使用|
||const|	是关键字，但不能使用|
||null|	空|

**Java注释**
类似于C/C++，Java也支持单行以及多行注释。注释中的字符将被Java编译器忽略。
```
public class HelloWorld {
   /* 这是第一个Java程序
    *它将打印Hello World
    * 这是一个多行注释的示例
    */
    public static void main(String []args){
       // 这是单行注释的示例
       /* 这个也是单行注释的示例 */
       System.out.println("Hello World"); 
    }
}
```

<br/>
<br/>

####原始数据类型

------

JAVA中有八种基本类型

> * 对于整数有4种类型：**byte**, **short**, **int**, **long**
> * 实数类型： **float**, **double**
> * 字符类型： **char**
> * 布尔： 返回 **true** 或 **false** 值 (**true** 或 **false**)


|类型|描述|bit|最小值|最大值|
|:----:|:----:|:----:|:----:|:----:|
|byte	|8位整数|8	 |-128 (-2^7)	|127 (2^7-1)|
|short	|16位整数|16	|-32,768 (-2^15)	|32,767 (2^15 -1)|
|int|32位整数|32|- 2,147,483,648<br/>(-2^31)|2,147,483,647<br/>(2^31 -1)|
|long|64位整数|64|-9,223,372,036,854,775,808<br/>(-2^63)|9,223,372,036,854,775,807<br/>(2^63 -1)|
|float|32位实数|32|-3.4028235 x 10^38|3.4028235 x 10^38|
|double|64位实数|64|-1.7976931348623157 x 10^308|1.7976931348623157 x 10^308|
|boolean|逻辑类型||false|true|
|char|字符|16|	'\u0000' (0)|'\uffff' (65,535).|


<br/>

####java命名约定的优点

通过使用标准的Java命名约定，您可以使自己和其他程序员更容易阅读代码。Java程序的可读性非常重要。 它能让程序开发者花费更少的时间来读懂代码的作用。

|名称|约定|
|:-:|:-:|
|类名称	|应以大写字母开头，并成为容易理解的名词或组合。如：**String**, **Color**, **Button**, **System**, **Thread**等。|
|接口名称|应以大写字母开头，并作为形容词。如： **Runnable**，**Remote**，**ActionListener**等。|
|方法名称|应以小写字母开头，并作为动词。如：**actionPerformed()**，**main()**，**print()**，**println()**等。|
|变量名称|应以小写字母开头。如：**firstName**，**orderNumber**等。|
|包名称|应使用小写字母。如： **java**，**lang**，**sql**，**util**等。|
|常量名称|应使用大写字母。 例如：**RED**, **YELLOW**, **MAX_PRIORITY**等|