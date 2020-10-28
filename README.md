# MedImageServiceCenter
本项目初衷为大学、医院、科研中心等更方便的操作影像数据。包括：数据收集、发送、匿名化、查询、共享等基础服务。可以把共同参与同一课题研究的所有被试数据组成为一个DataSet。该数据集包含从CT\磁共振等影像设备采集来的MateData、AnonymData等等。同时在数据存储设备中，保持DataSet数据权限的私有性，数据可按照被试、序列导出。
# 1 开发内容简介
应用采用python语言开发，采用ResetFul 方式设计程序API的风格:
http://example.org/api/
http://example.org/v1/path1
....
返回方式以Json方式
{
"code":0,
"message":"sucess"
"data":"data"
}

调用时可以使用
linux 系统命令curl进行调用API进行自定义操作。

# 2 安装&&依赖
python 2.7 +
依赖包
flask


