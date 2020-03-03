## HelloWorld 程序

### 编写 HelloWorld.java 文件

在 VSCode 中打开一个工作区，在工作区根目录下创建 HelloWorld.java 文件。

内容如下：

```java
public class HelloWorld {
  public static void main(String[] args) {
    System.out.println("hello, world!");
  }
}
```

这是一个最基本的 Java 程序，作用是在控制台窗口输出`hello, world!`字样。

### 运行 HelloWorld 程序

现在运行这个文件的方式有两种。

1. 使用命令行运行。

首先将 HelloWorld.java 文件编译成 HelloWorld.class 文件。

执行命令`javac HelloWorld.java`，会在根目录下生成一个 HelloWorld.class 的文件。

我们编写的代码 HelloWorld.java 是供人阅读的文本，计器运行的代码 HelloWorld.class 是供计器阅读的文本。计算机只能识别二进制，所以.class 文件的内容是我们无法读懂的二进制文本。

接下来运行 HelloWorld.class 文件。

执行命令`java HelloWorld`，会在控制台窗口输出`hello, world!`字样。

注意：执行`java xx`命令时，不可以附带文件名后缀。

2. 使用 Java Test Runner 扩展包运行

鼠标焦点放在 main 方法上面，会看到 Run|Debug 两个按钮，点击 Run 按钮，即可运行 main 方法。这对新手而言是最简单的方式。但实际上仍然会执行第一步的那两个命令。

### HelloWorld 程序解析

如果您是一个对编程一无所知的纯新手，这一部分可能不适合您。

```java
public class HelloWorld {
  // ...
}
```

`public`是 Java 中一个关键字，也称为修饰符。Java 语言规范中明确要求，每个 java 都包含一个 public 修饰的类，类名要与文件名保持一致。

`class`同样是一个关键字，用于创建一个类。

`HelloWorld`是类的名字，只要您遵循 Java 命名规则，可以随便取，但是要和文件名保持一致。Java 的命名规则在后面会讲到。

`{}`两个大括号表示的是一个代码块，HelloWorld 类的内容都在这个大括号内。
