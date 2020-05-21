# face_recognition_py
本项目基于OpenCV使用Haar级联分类器实现人脸检测，与dlib库进行实时跟踪，应用LBPH算法开发了一个功能相对完整的人脸识别系统。系统采用MySQL进行数据存储，能够进行学生上课考勤人脸点名的功能，并拥有基于PyQt5设计的GUI实现。

## 系统预览
### 核心框架
![](https://github.com/kuronekonano/Face-Recognition-Based-Attendance-System/raw/master/images/CoreUI.png)
### 人脸采集
![](https://github.com/kuronekonano/Face-Recognition-Based-Attendance-System/raw/master/images/DataRecordUI.png)
### 数据管理
![](https://github.com/kuronekonano/Face-Recognition-Based-Attendance-System/raw/master/images/DataManageUI.png)

## 如何运行？
以下操作基于Anaconda3环境，并在Windows10 x64上测试。
### 克隆代码
```
$ git clone https://github.com/kuronekonano/Face-Recognition-Based-Attendance-System.git
$ cd Face-Recognition-Based-Attendance-System
```
### 创建Python虚拟环境
```
$ conda create -n opencv python=3.6
$ activate opencv
```
### 安装OpenCV
```
$ cd modules
$ pip install opencv_python-3.4.1+contrib-cp36-cp36m-win_amd64.whl
```
### 安装dlib
```
$ pip install dlib-19.8.1-cp36-cp36m-win_amd64.whl
```
### 安装其它依赖包
```
$ cd ..
$ pip install -r requirements.txt
```
### 运行核心框架
```
$ python core.py
```
### 运行人脸采集系统
```
$ python dataRecord.py
```
### 运行数据管理系统
```
$ python dataManage.py
```
### 更新
```
$ git pull
```
### 退出虚拟环境
```
$ deactivate
```

## License
GPL-3.0
