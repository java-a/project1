# Project 1 地图读取、输出问题

## IntelliJ IDEA 入门视频

我们使用 IntelliJ 来编写代码，并使用 IntelliJ 解决地图读取问题。

IntelliJ 入门视频链接：http://www.bilibili.com/video/av6483923/

## 一、将文件放到工程目录下

 如图，将tile.txt文件放到Intellij工程目录下。![](https://cloud.githubusercontent.com/assets/6532225/19012588/ce597416-87ec-11e6-9517-0ba9299a2778.png)

## 二、创建Scanner准备读取文件

如 Project1 文档中所写，创建 Scanner 来准备读取文件

![](https://cloud.githubusercontent.com/assets/6532225/19012720/13def9cc-87f0-11e6-8c47-ae777944ca5f.png)

但是此时出现了一个错误：程序在运行前不能确定文件是不是不存在，我们要处理文件不存在的问题。

把光标移到出错的代码处，按下 `Alt + Enter` ，出现IntelliJ提示的错误解决办法。 ![](https://cloud.githubusercontent.com/assets/6532225/19012589/ce6f50ce-87ec-11e6-8f0c-e6f65536f026.png)

选择第一项，发现main函数后面多了 `throws FileNotFoundException` 。此时代码不再报错。

## 三、读取文件中的地图信息

我们可以使用 `scanner.nextLine()` 来获取文件文件信息并输出。 ![](https://cloud.githubusercontent.com/assets/6532225/19012590/cf1458a8-87ec-11e6-8bab-c2c27cc3d9ab.png)

最后，思考一下如何通过读取的文件来输出中文的地图？