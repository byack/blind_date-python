# Love-python-APP
不是项目，就是一个简单的文件，通过给出的三个数据，对应的选项，用K-近邻算法预测剩余其它项的值。完成一个相亲配对。

# 说明
不是项目，就是一个简单的文件，通过给出的三个数据，第一列数据对应的是每年出差/旅行的公里数，第二列是玩游戏消耗时间的百分比，第三列是每周消费的冷饮公升数，然后用K-近邻算法预测剩余其它项的值。完成一个相亲配对。

## 所需要安装的一些包
安装matplotlib用于绘制图形，安装numpy用于计算，tkinter用于绘制界面，collections用于更简单的找到反馈回的信息。
前两个包Python应该是没有自带，需要安装，后面两个包Python一般都是自带的。
```bash
pip3 install matplotlib
pip3 install numpy
```

## 主要文件
其中的数据文件来于datingTestSet.txt这个文件，这里面的数据作为训练集，后续的数据都是和这个训练集进行匹配得出结果的。
三维可视化数据.py这个文件会将训练集中的数据绘制出来，能直观的看到我们的数据分布情况。当然，这一步也可以不做。
相亲配对.py这个文件用户完成配对和返回配对结果的，我写了一个交互界面，程序运行后直接在窗口上收集用户输入和返回给用户匹配结果。

## 备注
这里K-近邻算法中我取的范围是10个，可能不是很合理，可以根据需求进行修改。
我还是一个小白，没有接触过机器学习，暂时在这记录一点我目前的想法：如果我的数据很多，或者我的程序并不完善，需要在运行的过程中不断的学习，我会将数据导入到数据库中，每一次运行，先进行匹配，如果匹配出来的结果和实际情况相同，如果不相同，我们设置更改，每一次运行的数据都导入数据库中，这样我们的数据库中的值会不断的变大，但是，我们所能够参照的数据变多了，程序的匹配就会越来越准确。我不知道这样算不算是一个简单的机器学习思路。不局限与这个项目，这只是一个简单的小数据处理，放在其它项目中去，这样的思路让程序分析的结果越来越精确是否可行，随着数据量增大，Python的速度是否跟得上，在这里，我是每匹配一次就从txt文件中读取一次，因为数据量比较少，数据量很大以后，这样的方法是不是就不可行了，有没有更好的解决办法。（以上只是我写这篇说明时的想法，在这里记录一下，欢迎邮箱交流）
