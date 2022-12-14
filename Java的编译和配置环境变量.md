### Java的编译和配置环境变量
***
>步骤  

1. 用记事本编写程序
2. 编译文件（翻译文件）
3. 运行程序
***

>编译文件步骤  

1. Java代码在操作系统中不能直接运行
2. 编译的动作就是将代码翻译为操作系统可以看懂的内容
3. 编译后产生新文件
4. 具体步骤：
	1. 记事本写好代码后保存后缀为.java的格式
	2. 打开JDK目录(Java安装包文件夹)
	3. 打开bin文件夹
	4. 原理：用javac编译，用java运行
	5. 打开cmd，切换到代码所在文件夹的路径（桌面）
	6. 切换到当前路径后输入：  
	`javac HelloWorld.java`  
	`格式：javac空格+文件名.格式`
	7. 正常运行后在文件夹中会出现一个新文件（编译后的文件，class文件，即操作系统可以看懂的文件类型）
	8. 继续在cmd中输入：  
	`java HelloWorld`  
	`格式：java空格+文件名`
	9. 点击回车即可完美运行！！！
***
##### ！注意：在任何时候都可以使用javac 和java命令，因为在安装JDK时自动将javac和Java的路径配置到环境变量中！
***

### 手动配置环境变量
>JDK安装时默认配置了四个工具的环境变量（javac\java\javaw\jshell）,可以在cmd的任何路径下使用。但是在实际学习中还需要用到其他的Java工具，这是就需要手动配置其他的环境变量。步骤如下：  

1. 先删除已经配置好的环境变量
2. 在系统变量中直接新建（不进入path）
3. 新建变量名为： JAVA_HOME
4. 新建变量值为：bin文件夹路径（删掉\bin,只输入留下的部分）
5. 进入系统变量中的path
6. 新建名字为 %JAVA_HOME%\bin 的环境变量（引用了JAVA_HOME,系统将JAVA_HOME中的值拿来引用，与bin文件夹进行拼接形成完整的路径） ，移动到最上面。  
7. **后续的Java开发软件也会依赖JAVA_HOME这个变量，所以一劳永逸**

>注意：可能会出现重启后无法识别创建好的环境变量的bug（无法识别）。解决方法如下：  

1. 照样配置JAVA_HOME的系统变量
2. 在path中，不要引用JAVA_HOME,直接写完bin文件夹的完整路径。如`C:\Java\bin`

