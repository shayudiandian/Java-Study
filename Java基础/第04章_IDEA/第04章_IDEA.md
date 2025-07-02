# 第04章_IDEA

***

## 本章专题与脉络

<img src="images/第1阶段：Java基本语法-第04章.png" alt="第1阶段：Java基本语法-第04章" style="zoom:50%;" />

***





## 1. 认识IntelliJ IDEA（了解）

### 1.1 JetBrains  公司介绍

IDEA，是 JetBrains (https://www.jetbrains.com/)公司的产品，该公司成立于2000年，总部位于捷克的布拉格，致力于为开发者打造最高效智能的开发工具。

公司旗下还有其它产品，比如：

* WebStorm：用于开发 JavaScript、HTML5、CSS3 等前端技术
* PyCharm：用于开发 python
* PhpStorm：用于开发 PHP
* RubyMine：用于开发 Ruby/Rails
* AppCode：用于开发 Objective - C/Swift
* CLion：用于开发 C/C++
* DataGrip：用于开发数据库和 SQL
* Rider：用于开发.NET
* GoLand：用于开发 Go

用于开发 Android 的 Android Studio，也是 Google 基于 IDEA 社区版进行迭代的。



### 1.2 IntelliJ IDEA  介绍

IDEA，全称 `IntelliJ IDEA`，是 Java 语言的集成开发环境，目前已经（基本）`代替`了Eclipse的使用。IDEA 在业界被公认为是最好的 Java 开发工具（之一），因其`功能强悍`、`设置人性化`，而深受Java、大数据、移动端程序员的喜爱。

IntelliJ IDEA 在 2015 年的官网上这样介绍自己：

> Excel at enterprise, mobile and web development with Java, Scala and Groovy,with all the latest modern technologies and frameworks available out of thebox.
>

### 1.3 IDEA的主要优势：(vs Eclipse)

**功能强大：**

① 强大的整合能力。比如：Git、Maven、Spring等

<img src="images/内置的工具和支持的框架.png" alt="1576218068631" style="zoom: 67%;" />

② 开箱即用的体验（集成版本控制系统、多语言支持的框架随时可用，无需额外安装插件）

**符合人体工程学：**

① 高度智能（快速的智能代码补全、实时代码分析、可靠的重构工具）

![image-20221018104821144](images/image-20221018104821144.png)

② 提示功能的快速、便捷、范围广

![img](images/clip_imrage002.jpg)

![image-20221018104942633](images/image-20221018104942633.png)

③ 好用的快捷键和代码模板

④ 精准搜索

### 1.4 IDEA  的下载

- 下载网址： https://www.jetbrains.com/idea/download/#section=windows


- IDEA 分为两个版本： `旗舰版(Ultimate)`和 `社区版(Community)`。


- IDEA的大版本每年迭代一次，大版本下的小版本（如：2022.x）迭代时间不固定，一般每年3个小版本。



两个不同版本的详细对比，可以参照官网：
https://www.jetbrains.com/idea/features/editions_comparison_matrix.html

官网提供的详细使用文档：
https://www.jetbrains.com/help/idea/meet-intellij-idea.html

## 2. 卸载与安装（略）





## 3. HelloWorld的实现

### 3.1 新建Project - Class

选择"New Project"：

<img src="images/image-20221019174051967.png" alt="image-20221019174051967" style="zoom:80%;" />

指名工程名、使用的JDK版本等信息。如下所示：

![image-20221019174355370](images/image-20221019174355370.png)

接着创建Java类：

![image-20221019174505876](images/image-20221019174505876.png)

![image-20221019174551606](images/image-20221019174551606.png)

### 3.2 编写代码

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello,World!");
    }
}
```

### 3.3 运行

![image-20221019174716442](images/image-20221019174716442.png)

![image-20221019174801370](images/image-20221019174801370.png)

## 4. JDK相关设置

### 4.1 项目的JDK设置

`File-->Project Structure...-->Platform Settings -->SDKs`

![image-20221019174847921](images/image-20221019174847921.png)

![image-20221019175030852](images/image-20221019175030852.png)

- 注1：SDKs全称是Software Development Kit ，这里一定是选择JDK的安装根目录，不是JRE的目录。
- 注2：这里还可以从本地添加多个JDK。使用“+”即可实现。

### 4.2 out目录和编译版本

`File-->Project Structure...-->Project Settings -->Project`

![image-20221019175358200](images/image-20221019175358200.png)

## 5. 详细设置

### 5.1 如何打开详细配置界面

1、显示工具栏

![image-20221019175536721](images/image-20221019175536721.png)

2、选择详细配置菜单或按钮

![image-20221019175620422](images/image-20221019175620422.png)

![image-20221019175953767](images/image-20221019175953767.png)

### 5.2 系统设置

#### 1、默认启动项目配置

![image-20221019180050832](images/image-20221019180050832.png)

启动IDEA时，默认自动打开上次开发的项目？还是自己选择？

如果去掉Reopen projects on startup前面的对勾，每次启动IDEA就会出现如下界面：

![image-20221019180304644](images/image-20221019180304644.png)

#### 2、取消自动更新

Settings-->Appearance & Behavior->System Settings -> Updates

![image-20221019180428323](images/image-20221019180428323.png)

默认都打√了，建议检查IDE更新的√去掉，检查插件更新的√选上。

### 5.3 设置整体主题

#### 1、选择主题

![image-20221019180637822](images/image-20221019180637822.png)

#### 2、设置菜单和窗口字体和大小

![1655136527800](images/1655136527800.png)

#### 3、设置IDEA背景图

![image-20221018204241748](images/image-20221018204241748.png)

选择一张合适的图片作为背景，即可。

![image-20221018204305159](images/image-20221018204305159.png)

### 5.4 设置编辑器主题样式

#### 1、编辑器主题

![1655136655026](images/1655136655026.png)

#### 2、字体大小

![1655136907073](images/1655136907073.png)

更详细的字体与颜色如下：

![image-20221019182625234](images/image-20221019182625234.png)

> 温馨提示：如果选择某个font字体，中文乱码，可以在fallback font（备选字体）中选择一个支持中文的字体。
>

#### 3、注释的字体颜色

![image-20220616121435182](images/image-20220616121435182.png)

- Block comment：修改多行注释的字体颜色
- Doc Comment –> Text：修改文档注释的字体颜色
- Line comment：修改单行注释的字体颜色

### 5.5 显示行号与方法分隔符

![1655137441471](images/1655137441471.png)

### 5.6 代码智能提示功能

![1655137649491](images/1655137649491.png)

IntelliJ IDEA 的代码提示和补充功能有一个特性：`区分大小写`。 如果想不区分大小写的话，就把这个对勾去掉。`建议去掉勾选`。

### 5.7 自动导包配置（掌握）

* 默认需要自己手动导包，Alt+Enter 快捷键

![1655138308426](images/1655138308426.png)

* 自动导包设置
  * 动态导入明确的包：Add unambiguous imports on the fly，该设置具有全局性；
  * 优化动态导入的包：Optimize imports on the fly，该设置只对当前项目有效；

![1655138465774](images/1655138465774.png)

### 5.8 设置项目文件编码

![image-20220615190832482](images/image-20220615190832482.png)

说明： Transparent native-to-ascii conversion主要用于转换ascii，显式原生内容。一般都要勾选。

### 5.9 设置控制台的字符编码

![image-20221019003153265](images/image-20221019003153265.png)

### 5.10 修改类头的文档注释信息（掌握）

![image-20221018114632127](images/image-20221018114632127.png)

比如：

```java
/**
* ClassName: ${NAME}
* Package: ${PACKAGE_NAME}
* Description: 
* @Author XXX
* @Create ${DATE} ${TIME} 
* @Version 1.0   
*/
```

常用的预设的变量，这里直接贴出官网给的：

```java
${PACKAGE_NAME} - the name of the target package where the new class or interface will be created. 
${PROJECT_NAME} - the name of the current project. 
${FILE_NAME} - the name of the PHP file that will be created. 
${NAME} - the name of the new file which you specify in the New File dialog box during the file creation. 
${USER} - the login name of the current user. 
${DATE} - the current system date. 
${TIME} - the current system time. 
${YEAR} - the current year. 
${MONTH} - the current month. 
${DAY} - the current day of the month. 
${HOUR} - the current hour. 
${MINUTE} - the current minute. 
${PRODUCT_NAME} - the name of the IDE in which the file will be created. 
${MONTH_NAME_SHORT} - the first 3 letters of the month name. Example: Jan, Feb, etc. 
${MONTH_NAME_FULL} - full name of a month. Example: January, February, etc.
```

### 5.11 设置自动编译

`Settings-->Build,Execution,Deployment-->Compiler`

<img src="images/1655109415450.png" alt="1655109415450" style="zoom: 67%;" />

### 5.12 设置为省电模式

![image-20220616121851207](images/image-20220616121851207.png)

IntelliJ IDEA 有一种叫做`省电模式`的状态，开启这种模式之后 IntelliJ IDEA 会`关掉代码检查`和`代码提示`等功能。所以一般也可认为这是一种`阅读模式`，如果你在开发过程中遇到突然代码文件不能进行检查和提示，可以来看看这里是否有开启该功能。

### 5.13 取消双击shift搜索

因为我们按shift切换中英文输入方式，经常被按到，总是弹出搜索框，太麻烦了。可以取消它。

<img src="images/1659191272699.png" alt="1659191272699" style="zoom:80%;" />

- 方式1：适用于IDEA 2022.1.2版本

在2022.1版本中，采用如下方式消双击shift出现搜索框：搜索double即可，勾选Disable double modifier key shortcuts，禁用这个选项。

![1659190132458](images/1659190132458.png)

- 方式2：适用于IDEA 2022.1.2之前版本

双击shift 或 ctrl + shift + a，打开如下搜索窗口：

![1577243967254](images/1577243967254.png)

选择registry...，找到"ide.suppress.double.click.handler"，把复选框打上勾就可以取消双击shift出现搜索框了。

![1577244045320](images/1577244045320.png)

## 6. 工程与模块管理（理解）

### 6.1 IDEA项目结构

**层级关系：**

```
project(工程) - module(模块) - package(包) - class(类)
```

**具体的：**

```
一个project中可以创建多个module

一个module中可以创建多个package

一个package中可以创建多个class
```

> 这些结构的划分，是为了方便管理功能代码。

### 6.2 Project和Module的概念

在 IntelliJ IDEA 中，提出了Project和Module这两个概念。

<img src="images/image-20220523014358169.png" alt="image-20220523014358169" style="zoom:80%;" />

在 IntelliJ IDEA 中Project是`最顶级的结构单元`，然后就是Module。目前，主流的大型项目结构基本都是多Module的结构，这类项目一般是`按功能划分`的，比如：user-core-module、user-facade-module和user-hessian-module等等，模块之间彼此可以`相互依赖`，有着不可分割的业务关系。因此，对于一个Project来说：

- 当为单Module项目的时候，这个单独的Module实际上就是一个Project。
- 当为多Module项目的时候，多个模块处于同一个Project之中，此时彼此之间具有`互相依赖`的关联关系。
- 当然多个模块没有建立依赖关系的话，也可以作为单独一个“项目”运行。

### 6.3 Module和Package

在一个module下，可以声明多个包（package），一般命名规范如下：

```
1.不要有中文
2.不要以数字开头
3.给包取名时一般都是公司域名倒着写,而且都是小写
  比如：尚硅谷网址是www.atguigu.com
  那么我们的package包名应该写成：com.atguigu.子名字。
```

### 6.4 创建Module

建议创建“Empty空工程”，然后创建多模块，每一个模块可以独立运行，相当于一个小项目。JavaSE阶段不涉及到模块之间的依赖。后期再学习模块之间的依赖。

步骤：

（1）选择创建模块

![1655167625885](images/1655167625885.png)

（2）选择模块类型：这里选择创建Java模块，给模块命名，确定存放位置

![1659191966074](images/1659191966074.png)

（4）模块声明在工程下面

![1659192028623](images/1659192028623.png)

### 6.5 删除模块

（1）移除模块

![1659192150052](images/1659192150052.png)

![1659192180062](images/1659192180062.png)

（2）彻底删除模块

![1659192241224](images/1659192241224.png)

### 6.6 导入他人的模块

（1）将他人的模块`teacher_chapter04`整个的复制到自己IDEA项目的路径下

![1659192514219](images/1659192514219.png)

接着打开自己IDEA的项目，会在项目目录下看到拷贝过来的module，只不过不是以模块的方式呈现。

![1659192692658](images/1659192692658.png)

（2）查看Project Structure，选择import module

![image-20220615213827271](images/image-20220615213827271.png)

![image-20220615214746952](images/image-20220615214746952.png)

（3）选择要导入的module：

![1659192850055](images/1659192850055.png)

![image-20220615214916374](images/image-20220615214916374.png)

（4）接着可以一路Next下去，最后选择Overwrite

![1659192928140](images/1659192928140.png)

![1659192995900](images/1659192995900.png)

最后点击OK即可了。



### 6.7 同时打开两个IDEA项目工程

#### 1、两个IDEA项目工程效果

有些同学想要把上课练习代码和作业代码分开两个IDEA项目工程。

![image-20211229111753237](images/image-20211229111753237.png)

![image-20211229111906342](images/image-20211229111906342.png)

#### 2、新建一个IDEA项目

注意：第一次需要新建，之后直接打开项目工程即可

![1655170522054](images/1655170522054.png)

![1655170341953](images/1655170341953.png)

![1655170765902](images/1655170765902.png)

#### 3、打开两个IDEA项目

![image-20211229112314671](images/image-20211229112314671.png)

![image-20211229112343470](images/image-20211229112343470.png)

![1655173351720](images/1655173351720.png)

### 6.8 导入前几章非IDEA工程代码

**1、创建chapter01、chapter02、chapter03等章节的module**

将相应章节的源文件粘贴到module的src下。

![image-20220615220728669](images/image-20220615220728669.png)

![image-20220615220755529](images/image-20220615220755529.png)

打开其中各个源文件，会发现有乱码。比如：

![image-20220615220846097](images/image-20220615220846097.png)

**2、设置编码**

当前项目是UTF-8。如果原来的.java文件都是GBK的（如果原来.java文件有的是GBK，有的是UTF-8就比较麻烦了）。

可以单独把这两个模块设置为GBK编码的。

![image-20220615220544760](images/image-20220615220544760.png)

改为GBK，确认即可。如图：

![image-20220615220950214](images/image-20220615220950214.png)



## 7. 代码模板的使用（设置-编辑器-常规-后缀补全，查看使用自定义）

### 7.1 查看Postfix Completion模板(后缀补全)

![1655173712802](images/1655173712802.png)

### 7.2 查看Live Templates模板(实时模板)

![img](images/wps2.jpg)

### 7.3 常用代码模板

#### 1、非空判断

* 变量.null：if(变量 == null)
* 变量.nn：if(变量 != null) 
* 变量.notnull：if(变量 != null) 
* ifn：if(xx  == null)
* inn：if(xx  != null)

#### 2、遍历数组和集合

* 数组或集合变量.fori：for循环
* 数组或集合变量.for：增强for循环
* 数组或集合变量.forr：反向for循环
* 数组或集合变量.iter：增强for循环遍历数组或集合

#### 3、输出语句

- sout：相当于System.out.println
- soutm：打印当前方法的名称
- soutp：打印当前方法的形参及形参对应的实参值
- soutv：打印方法中声明的最近的变量的值
- 变量.sout：打印当前变量值
- 变量.soutv：打印当前变量名及变量值

#### 4、对象操作

- 创建对象
  - Xxx.new  .var ：创建Xxx类的对象，并赋给相应的变量
  - Xxx.new  .field：会将方法内刚创建的Xxx对象抽取为一个属性
- 强转
  - 对象.cast：将对象进行强转
  - 对象.castvar：将对象强转后，并赋给一个变量

#### 5、静态常量声明

* psf：public static final
* psfi：public static final int
* psfs：public static final String
* prsf：private static final

### 7.4 自定义代码模板

#### 7.4.1 自定义后缀补全模板

![image-20221018143204667](images/image-20221018143204667.png)

![image-20221018143606913](images/image-20221018143606913.png)

#### 7.4.2 自定义Live Templates

例如：定义sop代表System.out.print();语句

①在Live Templates中增加模板

![1576467339631](images/1576467339631.png)

②先定义一个模板的组，这样方便管理所有自定义的代码模板

![1576467395084](images/1576467395084.png)

③在模板组里新建模板

![1576467478993](images/1576467478993.png)

④定义模板（以输出语句为例）

![1576467712251](images/1576467712251.png)

- Abbreviation：模板的缩略名称
- Description：模板的描述
- Template text：模板的代码片段
- 模板应用范围。比如点击Define。选择如下：应用在java代码中。

![1576467768103](images/1576467768103.png)

**其它模板1：单元测试模板：**

```java
@Test
public void test$var1$(){
    $var2$
}
```

![image-20220612124137427](images/image-20220612124137427.png)

**其它模板2：创建多线程**

```java
new Thread(){
    public void run(){
        $var$
    }
};
```

![image-20220612124221967](images/image-20220612124221967.png)

**其它模板3：冒泡排序**

```java
for(int $INDEX$ = 1; $INDEX$ < $ARRAY$.length; $INDEX$++) {
    for(int $INDEX2$ = 0; $INDEX2$ < $ARRAY$.length-$INDEX$; $INDEX2$++) {
        if($ARRAY$[$INDEX2$] > $ARRAY$[$INDEX2$+1]){
            $ELEMENT_TYPE$ temp = $ARRAY$[$INDEX2$];
            $ARRAY$[$INDEX2$] = $ARRAY$[$INDEX2$+1];
            $ARRAY$[$INDEX2$+1] = temp;
        }
    }
}
```

![image-20220612124541378](images/image-20220612124541378.png)



## 8. 快捷键的使用（熟悉）

### 8.1 常用快捷键

#### 1、IDEA的日常快捷键

第1组：通用型

| 说明            | 快捷键           |
| --------------- | ---------------- |
| 复制代码-copy   | ctrl + c         |
| 粘贴-paste      | ctrl + v         |
| 剪切-cut        | ctrl + x         |
| 撤销-undo       | ctrl + z         |
| 反撤销-redo     | ctrl + shift + z |
| 保存-save all   | ctrl + s         |
| 全选-select all | ctrl + a         |

第2组：提高编写速度（上）

| 说明                                               | 快捷键           |
| -------------------------------------------------- | ---------------- |
| 智能提示-edit                                      | alt + enter      |
| 提示代码模板-insert live template                  | ctrl+j           |
| 使用xx块环绕-surround with ...                     | ctrl+alt+t       |
| 调出生成getter/setter/构造器等结构-generate ...    | alt+insert       |
| 自动生成返回值变量-introduce variable ...          | ctrl+alt+v       |
| 复制指定行的代码-duplicate line or selection       | ctrl+d           |
| 删除指定行的代码-delete line                       | ctrl+y           |
| 切换到下一行代码空位-start new line                | shift + enter    |
| 切换到上一行代码空位-start new line before current | ctrl +alt+ enter |
| 向上移动代码-move statement up                     | ctrl+shift+↑     |
| 向下移动代码-move statement down                   | ctrl+shift+↓     |
| 向上移动一行-move line up                          | alt+shift+↑      |
| 向下移动一行-move line down                        | alt+shift+↓      |
| 方法的形参列表提醒-parameter info                  | ctrl+p           |

第3组：提高编写速度（下）

| 说明                                        | 快捷键       |
| ------------------------------------------- | ------------ |
| 批量修改指定的变量名、方法名、类名等-rename | shift+f6     |
| 抽取代码重构方法-extract method ...         | ctrl+alt+m   |
| 重写父类的方法-override methods ...         | ctrl+o       |
| 实现接口的方法-implements methods ...       | ctrl+i       |
| 选中的结构的大小写的切换-toggle case        | ctrl+shift+u |
| 批量导包-optimize imports                   | ctrl+alt+o   |

第4组：类结构、查找和查看源码

| 说明                                                      | 快捷键                          |
| --------------------------------------------------------- | ------------------------------- |
| 如何查看源码-go to class...                               | ctrl + 选中指定的结构 或 ctrl+n |
| 显示当前类结构，支持搜索指定的方法、属性等-file structure | ctrl+f12                        |
| 退回到前一个编辑的页面-back                               | ctrl+alt+←                      |
| 进入到下一个编辑的页面-forward                            | ctrl+alt+→                      |
| 打开的类文件之间切换-select previous/next tab             | alt+←/→                         |
| 光标选中指定的类，查看继承树结构-Type Hierarchy           | ctrl+h                          |
| 查看方法文档-quick documentation                          | ctrl+q                          |
| 类的UML关系图-show uml popup                              | ctrl+alt+u                      |
| 定位某行-go to line/column                                | ctrl+g                          |
| 回溯变量或方法的来源-go to implementation(s)              | ctrl+alt+b                      |
| 折叠方法实现-collapse all                                 | ctrl+shift+ -                   |
| 展开方法实现-expand all                                   | ctrl+shift+ +                   |

第5组：查找、替换与关闭

| 说明                                               | 快捷键       |
| -------------------------------------------------- | ------------ |
| 查找指定的结构                                     | ctlr+f       |
| 快速查找：选中的Word快速定位到下一个-find next     | ctrl+l       |
| 查找与替换-replace                                 | ctrl+r       |
| 直接定位到当前行的首位-move caret to line start    | home         |
| 直接定位到当前行的末位 -move caret to line end     | end          |
| 查询当前元素在当前文件中的引用，然后按 F3 可以选择 | ctrl+f7      |
| 全项目搜索文本-find in path ...                    | ctrl+shift+f |
| 关闭当前窗口-close                                 | ctrl+f4      |

第6组：调整格式

| 说明                                         | 快捷键           |
| -------------------------------------------- | ---------------- |
| 格式化代码-reformat code                     | ctrl+alt+l       |
| 使用单行注释-comment with line comment       | ctrl + /         |
| 使用/取消多行注释-comment with block comment | ctrl + shift + / |
| 选中数行，整体往后移动-tab                   | tab              |
| 选中数行，整体往前移动-prev tab              | shift + tab      |

#### 2、Debug快捷键

| 说明                                                  | 快捷键        |
| ----------------------------------------------------- | ------------- |
| 单步调试（不进入函数内部）- step over                 | F8            |
| 单步调试（进入函数内部）- step into                   | F7            |
| 强制单步调试（进入函数内部） - force step into        | alt+shift+f7  |
| 选择要进入的函数 - smart step into                    | shift + F7    |
| 跳出函数 - step out                                   | shift + F8    |
| 运行到断点 - run to cursor                            | alt + F9      |
| 继续执行，进入下一个断点或执行完程序 - resume program | F9            |
| 停止 - stop                                           | Ctrl+F2       |
| 查看断点 - view breakpoints                           | Ctrl+Shift+F8 |
| 关闭 - close                                          | Ctrl+F4       |



### 8.2 查看快捷键

#### 1、已知快捷键操作名，未知快捷键

![1577246789281](images/1577246789281.png)

#### 2、已知快捷键，不知道对应的操作名

![1577246895469](images/1577246895469.png)

### 8.3 自定义快捷键

![1577247069135](images/1577247069135.png)

### 8.4 使用其它平台快捷键

苹果电脑或者是用惯Eclipse快捷的，可以选择其他快捷键插件。

![image-20221019205934099](images/image-20221019205934099.png)

## 9. IDEA断点调试(Debug)（掌握）

### 9.1 为什么需要Debug

编好的程序在执行过程中如果出现错误，该如何查找或定位错误呢？简单的代码直接就可以看出来，但如果代码比较复杂，就需要借助程序调试工具（Debug）来查找错误了。

```
运行编写好的程序时，可能出现的几种情况：
> 情况1：没有任何bug,程序执行正确！

====================如果出现如下的三种情况，都有必要使用debug=============================
> 情况2：运行以后，出现了错误或异常信息。但是通过日志文件或控制台，显示了异常信息的位置。
> 情况3：运行以后，得到了结果，但是结果不是我们想要的。
> 情况4：运行以后，得到了结果，结果大概率是我们想要的。但是多次运行的话，可能会出现不是我们想要的情况。
        比如：多线程情况下，处理线程安全问题。
        
```

### 9.2 Debug的步骤

Debug(调试)程序步骤如下：

1、添加断点

2、启动调试

3、单步执行

4、观察变量和执行流程，找到并解决问题

#### 1、添加断点

在源代码文件中，在想要设置断点的代码行的前面的标记行处，单击鼠标左键就可以设置断点，在相同位置再次单击即可取消断点。

![1576476225262](images/1576476225262.png)

#### 2、启动调试

IDEA提供多种方式来启动程序(Launch)的调试，分别是通过菜单(Run –> Debug)、图标(“绿色臭虫”![1576476267687](images/1576476267687.png)等等

![1576476841154](images/1576476841154.png)

#### 3、单步调试工具介绍

![1576477907469](images/1576477907469.png)

或

![1576477927994](images/1576477927994.png)

![1576476917169](images/1576476917169.png)：Step Over（F8）：进入下一步，如果当前行断点是调用一个方法，则不进入当前方法体内

![1576476984903](images/1576476984903.png)：Step Into（F7）：进入下一步，如果当前行断点是调用一个自定义方法，则进入该方法体内

![1576477028289](images/1576477028289.png)：Force Step Into（Alt +Shift  + F7）：进入下一步，如果当前行断点是调用一个核心类库方法，则进入该方法体内

![1576477117156](images/1576477117156.png)：Step Out（Shift  + F8）：跳出当前方法体

![1576477204366](images/1576477204366.png)：Run to Cursor（Alt + F9）：直接跳到光标处继续调试

![1576477448969](images/1576477448969.png)：Resume Program（F9）：恢复程序运行，但如果该断点下面代码还有断点则停在下一个断点上

![1576477293031](images/1576477293031.png)：Stop（Ctrl + F2）：结束调试

![1576477330355](images/1576477330355.png)：View Breakpoints（Ctrl + Shift  + F8）：查看所有断点

![1576477381767](images/1576477381767.png)：Mute Breakpoints：使得当前代码后面所有的断点失效， 一下执行到底 

> 说明：在Debug过程中，可以动态的下断点。

### 9.3 多种Debug情况介绍

#### 9.3.1 行断点

- 断点打在代码所在的行上。执行到此行时，会停下来。

```java
package com.atguigu.debug;

/**
 * ClassName: Debug01
 * Package: com.atguigu.debug
 * Description: 演示1：行断点  &  测试debug各个常见操作按钮
 *
 * @Author: XXX
 * @Create: 2022/10/20 18:44
 * @Version 1.0
 */
public class Debug01 {
    public static void main(String[] args) {
        //1.
        int m = 10;
        int n = 20;
        System.out.println("m = " + m + ",n = " + n);
        swap(m, n);
        System.out.println("m = " + m + ",n = " + n);

        //2.
        int[] arr = new int[] {1,2,3,4,5};
        System.out.println(arr);//地址值

        char[] arr1 = new char[] {'a','b','c'};
        System.out.println(arr1);//abc
    }

    public static void swap(int m,int n){
        int temp = m;
        m = n;
        n = temp;
    }

}

```

#### 9.3.2 方法断点

- 断点设置在方法的签名上，默认当进入时，断点可以被唤醒。
- 也可以设置在方法退出时，断点也被唤醒

![image-20221020213250606](images/image-20221020213250606.png)

- 在多态的场景下，在父类或接口的方法上打断点，会自动调入到子类或实现类的方法

```java
package com.atguigu.debug;

import java.util.HashMap;

/**
 * ClassName: Debug02
 * Package: com.atguigu.debug
 * Description: 演示2： 方法断点
 *
 * @Author: XXX
 * @Create: 2022/10/20 21:15
 * @Version 1.0
 */
public class Debug02 {
    public static void main(String[] args) {

        //1.
        Son instance = new Son();
        instance.test();
        //2.
        Father instance1 = new Son();
        instance1.test();

        //3.
        Consumer con = new ConsumerImpl();
        con.accept("atguigu");

        //4.
        HashMap map = new HashMap();
        map.put("Tom",12);
        map.put("Jerry",11);
        map.put("Tony",20);
    }
}

class Father{
    public void test(){
        System.out.println("Father : test");
    }
}

class Son extends Father{
    public void test(){
        System.out.println("Son : test");
    }
}

interface Consumer{
    void accept(String str);
}

class ConsumerImpl implements Consumer{

    @Override
    public void accept(String str) {
        System.out.println("ConsumerImple:" + str);
    }
}


```

#### 9.3.3 字段断点

- 在类的属性声明上打断点，默认对属性的修改操作进行监控

![image-20221020214905607](images/image-20221020214905607.png)

```java
package com.atguigu.debug;

/**
 * ClassName: Debug03
 * Package: com.atguigu.debug
 * Description: 演示3：字段断点
 *
 * @Author: XXX
 * @Create: 2022/10/20 21:34
 * @Version 1.0
 */
public class Debug03 {
    public static void main(String[] args) {
        Person p1 = new Person(3);

        System.out.println(p1);
    }
}

class Person{
    private int id = 1;
    private String name;
    private int age;

    public Person() {
    }
    {
        id = 2;
    }
    public Person(int id) {
        this.id = id;
    }



    public Person(int id, String name, int age) {
        this.id = id;
        this.name = name;
        this.age = age;
    }

    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }

    @Override
    public String toString() {
        return "Person{" +
                "id=" + id +
                ", name='" + name + '\'' +
                ", age=" + age +
                '}';
    }
}

```

#### 9.3.4 条件断点

```java
package com.atguigu.debug;

/**
 * ClassName: Debug04
 * Package: com.atguigu.debug
 * Description: 演示4：条件断点
 *
 * @Author: XXX
 * @Create: 2022/10/20 21:49
 * @Version 1.0
 */
public class Debug04 {
    public static void main(String[] args) {
        int[] arr = new int[]{1,2,3,4,5,6,7,8,9,10,11,12};

        for (int i = 0; i < arr.length; i++) {
            int target = arr[i];
            System.out.println(target);
        }
    }
}
```

针对上述代码，在满足arr[i] % 3 == 0的条件下，执行断点。

![image-20221020220043375](images/image-20221020220043375.png)

#### 9.3.5 异常断点

- 对异常进行跟踪。如果程序出现指定异常，程序就会执行断点，自动停住。

```java
package com.atguigu.debug;

import java.util.Date;

/**
 * ClassName: Debug05
 * Package: com.atguigu.debug
 * Description: 演示5：异常断点
 *
 * @Author: XXX
 * @Create: 2022/10/20 22:01
 * @Version 1.0
 */
public class Debug05 {
    public static void main(String[] args) {

        int m = 10;
        int n = 0;
        int result = m / n;
        System.out.println(result);


//        Person p1 = new Person(1001);
//        System.out.println(p1.getName().toUpperCase());


    }
}

```

通过下图的方式，对指定的异常进行监控：

![image-20221020220904864](images/image-20221020220904864.png)

#### 9.3.6 线程调试

```java
package com.atguigu.debug;

/**
 * ClassName: Debug06
 * Package: com.atguigu.debug
 * Description: 演示6：线程调试
 *
 * @Author: XXX
 * @Create: 2022/10/20 22:46
 * @Version 1.0
 */
public class Debug06 {

    public static void main(String[] args) {

        test("Thread1");
        test("Thread2");


    }

    public static void test(String threadName) {
        new Thread(
                () -> System.out.println(Thread.currentThread().getName()),
                threadName
        ).start();
    }

}

```

![image-20221020231542081](images/image-20221020231542081.png)

#### 9.3.7 强制结束

```java
package com.atguigu.debug;

/**
 * ClassName: Debug07
 * Package: com.atguigu.debug
 * Description: 演示7：强制结束
 *
 * @Author: XXX
 * @Create: 2022/10/20 23:15
 * @Version 1.0
 */
public class Debug07 {
    public static void main(String[] args) {
        System.out.println("获取请求的数据");
        System.out.println("调用写入数据库的方法");
        insert();
        System.out.println("程序结束");
    }

    private static void insert() {
        System.out.println("进入insert()方法");
        System.out.println("获取数据库连接");
        System.out.println("将数据写入数据表中");
        System.out.println("写出操作完成");
        System.out.println("断开连接");
    }
}

```

![image-20221020232038387](images/image-20221020232038387.png)

### 9.4 自定义调试数据视图

```java
package com.atguigu.debug;

import java.util.HashMap;

/**
 * ClassName: Debug08
 * Package: com.atguigu.debug
 * Description: 演示8：用户自定义数据视图
 *
 * @Author: XXX
 * @Create: 2022/10/20 23:21
 * @Version 1.0
 */
public class Debug08 {
    public static void main(String[] args) {
        HashMap<Integer,String> map = new HashMap<>();
        map.put(1,"高铁");
        map.put(2,"网购");
        map.put(3,"支付宝");
        map.put(4,"共享单车");

        System.out.println(map);
    }
}

```

设置如下：

![1576478352757](images/1576478352757.png)

![1576478431514](images/1576478431514.png)

### 9.5 常见问题

问题：使用Step Into时，会出现无法进入源码的情况。如何解决？

方案1：使用 force step into 即可

方案2：点击Setting -> Build,Execution,Deployment -> Debugger -> Stepping

把Do not step into the classess中的`java.*`、`javax.*` 取消勾选即可。

<img src="images/image-20220516200427750.png" alt="image-20220516200427750" style="zoom:75%;" />

小结：

> 经验：初学者对于在哪里加断点，缺乏经验，这也是调试程序最麻烦的地方，需要一定的经验。
>
> 简单来说，在可能发生错误的代码的前面加断点。如果不会判断，就在程序执行的起点处加断点。

## 10. IDEA常用插件（了解）

### 推荐1：Alibaba Java Coding Guidelines

 ![image-20221023224455751](images/image-20221023224455751.png)

阿里巴巴Java编码规范检查插件，检测代码是否存在问题，以及是否符合规范。

使用：在类中，右键，选择编码规约扫描，在下方显示扫描规约和提示。根据提示规范代码，提高代码质量。

### 推荐2：jclasslib bytecode viewer

 ![image-20221019223514412](images/image-20221019223514412.png)

可视化的字节码查看器。

使用：

1. 在 IDEA 打开想研究的类。
2. 编译该类或者直接编译整个项目（ 如果想研究的类在 jar 包中，此步可略过）。
3. 打开“view” 菜单，选择“Show Bytecode With jclasslib” 选项。
4. 选择上述菜单项后 IDEA 中会弹出 jclasslib 工具窗口。

![image-20221023225239838](images/image-20221023225239838.png)

英文设置：

在 Help -> Edit Custom VM Options …，加上

```
-Duser.language=en
```

### 推荐3：Translation

 ![image-20221019224727758](images/image-20221019224727758.png)

注册翻译服务（有道智云、百度翻译开放平台、阿里云机器翻译）帐号，开通翻译服务并获取其应用ID和密钥
绑定应用ID和密钥：偏好设置（设置） > 工具 > 翻译 > 常规 > 翻译引擎 > 配置…

使用：鼠标选中文本，点击右键即可自动翻译成多国语言。

注：请注意保管好你的应用密钥，防止其泄露。

### 推荐4：GenerateAllSetter

 ![image-20221019223238560](images/image-20221019223238560.png)

实际开发中还有一个非常常见的场景： 我们创建一个对象后，想依次调用 Setter 函数对属性赋值，如果属性较多很容易遗漏或者重复。

<img src="images/image-20221023230812560.png" alt="image-20221023230812560" style="zoom:80%;" />

可以使用这 GenerateAllSetter 提供的功能，快速生成对象的所有 Setter 函数（可填充默认值），然后自己再跟进实际需求设置属性值。

### 插件5：Rainbow Brackets

 ![image-20221019223340532](images/image-20221019223340532.png)

给括号添加彩虹色，使开发者通过颜色区分括号嵌套层级，便于阅读

![image-20221019222113604](images/image-20221019222113604.png)

### 推荐6：CodeGlance Pro

 ![image-20221019223219982](images/image-20221019223219982.png)

在编辑器右侧生成代码小地图，可以拖拽小地图光标快速定位代码，阅读行数很多的代码文件时非常实用。

<img src="images/image-20221023231842846.png" alt="image-20221023231842846" style="zoom:80%;" />

### 推荐7：Statistic

 ![image-20221019234545641](images/image-20221019234545641.png)

代码统计工具。

![image-20221023231801337](images/image-20221023231801337.png)

![image-20221023231741671](images/image-20221023231741671.png)

### 推荐8：Presentation Assistant

 ![image-20221019223426562](images/image-20221019223426562.png)

显示快捷键操作的按键

### 推荐9：Key Promoter X

 ![image-20221019223250943](images/image-20221019223250943.png)

快捷键提示插件。当你执行鼠标操作时，如果该操作可被快捷键代替，会给出提示，帮助你自然形成使用快捷键的习惯，告别死记硬背。

### 推荐10：JavaDoc

 ![image-20221019224820244](images/image-20221019224820244.png)

按`alt+insert`，执行操作：

![image-20221019225041655](images/image-20221019225041655.png)

### 推荐11： LeetCode Editor

 ![image-20221019225142011](images/image-20221019225142011.png)

![image-20221019225242331](images/image-20221019225242331.png)

在 IDEA 里刷力扣算法题

### 推荐12：GsonFormatPlus

 ![image-20221019233444272](images/image-20221019233444272.png)

根据 json 生成对象。

使用：使用alt + s 或 alt + insert调取。

![image-20221023235416317](images/image-20221023235416317.png)

举例：

```json
{
    "name": "tom",
    "age": "18",
    "gender": "man",
    "hometown": {
        "province": "河北省",
        "city": "石家庄市",
        "county": "正定县"
    }
}
```

### 插件13：Material Theme UI

 ![image-20221019223325480](images/image-20221019223325480.png)

对于很多人而言，写代码时略显枯燥的，如果能够安装自己喜欢的主题将为开发工作带来些许乐趣。

IDEA 支持各种主题插件，其中最出名的当属 Material Theme UI。

![image-20220810011348421](images/image-20220810011348421.png)

安装后，可以从该插件内置的各种风格个选择自己最喜欢的一种。

