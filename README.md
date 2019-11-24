# 第五次作业

  本次作业选择的两张图表一张是条形图，一张是既有条形图也有折线图的。如下二图：
  <img src="pictures/hw51.svg" width="600">
  <img src="pictures/hw52.svg" width="600">
  
为了在R Studio里实现第一张图，使用了如下代码：

>crimeman1 <- read_excel("crimeman.xlsx")  #首先读取和存储数据

>ggplot(crimeman1,aes(x=factor(year),y=crimeman)) +  #然后照葫芦画瓢使用ggplot这个包

>+geom_col(fill ="blue",width =0.8,position=position_dodge(1.5)) +  #下面照着书籍了调整了一些参数

>+geom_text(aes(label=crimeman),vjust = -0.2,colour = "black")

得到了下面这个图：




[之前的作业](https://github.com/cheerupyxolive/keshihuazuoye/blob/master/previoushw.md)

