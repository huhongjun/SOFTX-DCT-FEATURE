# README

红外图片和可见光图片检测电力线问题。  
matlab用于提取特征，提供五种算法；  
weka执行分类，采用NaiveBayes、RAndomForest、SVM三种。

## 安装

1. 安装weka 3.8  
    package manager中安装liblinear，normalize
2. 安装matlab 2013b

## 运行

打开matlab，打开5个目录，执行目录下的main*.m即可；

打开weka=》knowledge flow打开CLASSIFICATION_MODEL文件  
双击arff loader选择文件，然后点击text saver设置输出

点击左上角run即可。

## FAQ

### Weka package manager 无法打开的问题

1.打开日志窗口，可以看到服务器连接不上，一是官方的props文件，另外也需要连接sf.net  

2.runweka.bat增加如下一行  
    set _JAVA_OPTIONS=-Dhttp.proxyHost=127.0.0.1 -Dhttp.proxyPort=8580  
    使用代理连接服务器，http代理成功，socks5代理提示ziplib出错，repo缓存下载大小约2M。

