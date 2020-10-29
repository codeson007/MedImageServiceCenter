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
linux、mac 系统命令curl进行调用API进行自定义操作。  
windows 一般用什么？~~~哈哈~~
# 2 安装&&依赖
python 2.7 +
依赖包  
flask等包  
# 3 使用方法
### 命令行操作方式
### coder方式，不同的语言（python\R\java\matlab\go）可以用http协议调用方式操作具体的API
### 下面是命令行调用方式  （常见的dicom操作都包含在里面，哦哦，噢噢） 
$ curl  http://xxxx:prot/img-data-service/send-dicom?parmas...  
$ curl  http://xxxx:prot/img-data-service/get-dicom?parmas...  
$ curl  http://xxxx:prot/img-data-service/start-receiver-dicom?parmas...  
$ curl  http://xxxx:prot/img-data-service/anonym-dicom-in-path?parmas...  
$ curl  http://xxxx:prot/img-data-service/compress-patients-file-to-path?parmas...   


等等等   

##
![image](https://github.com/codeson007/MedImageServiceCenter/blob/main/public/image/send.PNG)  
![image](https://github.com/codeson007/MedImageServiceCenter/blob/main/public/image/pre-send.png)  
![image](https://github.com/codeson007/MedImageServiceCenter/blob/main/public/image/pos-send.png)  
  
等等等   
## 数据集操作
创建数据集，并未数据授予具体权限...   
导入、分配数据等等...  
配合实验员（学生、医生等）脚本RUN数据...  
建立简单的没有可视化功能的PACS功能...  
$ curl  http://xxxx:prot/img-data-service/create-dataset?params  
$ curl  http://xxxx:prot/img-data-service/drop-dataset?params  
$ curl  http://xxxx:prot/img-data-service/up-dataset?params  
$ curl  http://xxxx:prot/img-data-service/get-dataset-patients-location-csv?params  
$ curl  http://xxxx:prot/img-data-service/copy-dataset-patients-to-newpath?params   
等等等  


# 


### 界面目前仅在考虑中，暂不开发...
### 勿恼~~
###
###
#
### 疫情影响，
### 这个项目，我个人准备有偿服务，费用收取结构：
#### 1、项目费用
#### 2、维护费用
#### 3、定制开发费用
#### 联系方式：mycoder_son@163.com
