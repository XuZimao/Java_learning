## Java的注释、标识符、数据类型
### **注意：Java中类名必须和文件名保持一致！**

### 1.注释
>单行注释和多行注释与C语言相同　　

1. 单行注释
2. 多行注释
3. 文档注释（/**注释信息*/）
***
### 2.标识符和关键字
>标识符的命名规则  

1. 有字母、下划线、（美元）符号和数字组成、长度不受限制
2. 第一个字符不能是数字
3. 不能与关键字重名
4. 区分大小写
***
>关键字  

1. 在NotePad++中关键字有代码高亮
2. Java中有50个关键字
3. **Java中的关键字均为小写**
***
>部分数据类型总结  

1. class关键字:  
用于创建/定义一个类，（类）构成Java最基本的组成单元。class后面加类的名字，如：`public class HelloWorld{}`，其中`HelloWorld`就是类名，`{}`就是类的范围，所有的代码放到类的大括号中。
2. 字面量（常量）  
定义：告诉程序员数据在程序中的书写格式
包括六种字面量类型，如下：
	1. 整数类型（int）
	2. 小数类型（float）
	3. 字符串类型（str,双引号）
	4. 字符类型（char,用单引号括起来，**里面的内容有且只能有一个**）
	5. 布尔类型(boolean,只有两个值，ture和false)
	6. 空类型（null）
***
### 3.数据类型的练习
>在练习之前先把整体代码框架写好，如下：  

	public class pro1{
		public static void main(String[] args){
			System.out.println();  //括号内是输出的内容
		}
	}

>对所有数据类型逐个练习，如下：  

	public class pro1{  //类名必须和文件名相同
		public static void main(String[] args){  //main方法是程序的主入口，格式固定
			System.out.println(666);  //输出语句，将小括号内的语句打印
			System.out.println(-123);  // 负值类型
			System.out.println(3.14);   //浮点数类型
			System.out.println("我爱Java");  //字符串类型
			System.out.println('男');  //注意字符类型中，引号内只能有一个字符
			System.out.println(true);  //布尔类型
			System.out.println(false);  //布尔类型
			System.out.println("null");  //空类型，注意null类型不能直接打印，必须转换为字符串
		}
	}

***
### 4.特殊字符

>也叫转义字符，如'\t' '\r'  '\n'等等  

1.  \t制表符  
概念：在打印时候，把前面字符串的长度**补齐到8**，或者8的倍数。**至少补1个空格，最多补8个空格。**  
作用：将输出的内容整齐的打印出来，代码如下：     

		public class texe{
			public static void main(String[] arges){
				System.out.println("name"+'\t'+"age");  //将name的长度用空格补充至8（添加4个空格）
				System.out.println("Tom"+'\t'+"20");  //将Tom的长度用空格补充至8（添加5个空格）	
			}
		}
	输出如下：    ![](texe.png)    
	#### 注意：\t在补空格时只与它前面的字符串有关系，与后面的没有任何关系！
