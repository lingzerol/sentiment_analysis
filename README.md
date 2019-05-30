# sentiment_analysis
根据人们对电影的评论进行情感上的区分，分为正面和负面。

功能
----
先对数据进行预处理，处理不必要的特征，然后使用TD-IDF进行分析，将不同评论进行量化成为一个21787维向量。建立以一个(512,256,128,64,1)的神经网络模型，采用梯度下降法，并将量化后的数据进行分批训练。将测试数据带入训练好后的模型，并对模型的准确率进行评价。

程序效果
--------

>训练过程loss损失变化曲线图
>![Image](https://raw.githubusercontent.com/lingzerol/sentiment_analysis/master/Program_performance/trainning_loss.png)

>test数据的准确率
>![Image](https://raw.githubusercontent.com/lingzerol/sentiment_analysis/master/Program_performance/accuracy.png)

>test数据的ROC曲线
>![Image](https://raw.githubusercontent.com/lingzerol/sentiment_analysis/master/Program_performance/roc.png)