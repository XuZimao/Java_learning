## Java程序基本结构和JDK文件夹的内容

### Java程序的基本结构
1. 类名(与文件名保持一致) `public class 文件名`
2. 主函数 `public static void main(String[] args){}`
3. 基本输出语句 `System.out.println()  //自动换行`或`System.out.print()  //不换行`
4. 基本输入语法(需要导入特定的包)  
		
		import java.util.*;  //全部导入
		Scanner inp = new Scanner(System.in);  //初步接收键盘输入的内容并定义为inp(自己取的名字)
		int num=inp.nextInt();  //将接收到的内容赋值给整型对象num，输入成功,可以对num对象进行操作
5. 输入操作中第二部(将接收到的内容进行格式赋值)

		格式: Boolean 变量名=初步接收名字.nextBoolean();  //对象类型必须和后面的类型(nextBoolean)相同

	* nextBoolean();  //布尔类型
	* nextBytete();  //byte(短短整数)类型
	3. nextShort();  //短整型类型
	4. nextInt();   //整型类型
	5. nextLong();  //长整型类型
	6. nextFloat();  //浮点数类型
	7. nextDouble();  //双精度浮点数类型

6. Java的格式化字符`printf("%d,%f",12,33.33);`注意输出语句是`printf`,与C语言保持一致
	*  %d,输出int类型
	2. %c,输出char类型
	3. %f,输出浮点数类型
	4. %s,输出字符串类型
	5. %md,输出的int类型数据占m列
	6. %m.nf,输出的浮点数类型占据m列，小数点后保留n位。


### JDK文件夹的内容
1. bin（最重要）：存放了各种工具命令，其中javac和java比较重要
2. conf:存放了相关的配置文件
3. include:存放了一些平台特定的头文件
4. jmods：存放了各种模块
5. legal:存放了各种模块的授权文件
6. lib:存放了工具的一些补充JAR包