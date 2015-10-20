# Kinect-for-3D-face
3D的人脸识别主要运用到Kinect的三个模块：Fusion、Face、HD Face.<br>
* Fusion<br>
  Fusion主要是对人体进行三维重构，Kinect Fusion对物体的追踪仅仅使用传感器产生的深度数据流。
* Face<br>
  Face是将人脸进行二维的空间展示，主要提供的接口有Detetion、Alignment、Orientation、Expressions.
* HD Face<br>
  HD Face是将人脸进行三维的空间展示，通过人脸模型构建器，提供94个面部模型点，1347个面部顶点。

许老师开会主要提到的几点：
* 提取出脸部的深度数据，Kinect Fusion是重构整个人体，因此我们第一步要做的就是筛选出面部的深度数据，n*n的矩阵；
* 拿到面部深度数据后，首先探究Kinect SDK提供的面型顶点是否可以加以利用来刻画出一个面部面型，若不能，就采取小组自己的标点方案；
* 进一步研读相关论文，利用3D数据实现人脸识别；
* (可选)做微表情，在已有的面部接口上寻找其他的面部参数；

## 相关资源
  * [台湾大牛Heresy写的Kinect二代系列文章](https://kheresy.wordpress.com/kinect-for-windows-v2-cpp-index/ )
  * [在校生的Kinect二代博客](http://blog.csdn.net/dustpg/article/category/2408183)
  * [微软官方发布的一个Kinect入门视频](https://www.microsoftvirtualacademy.com/zh-cn/training-courses/-kinect-for-windows-v2--8743?l=15BQDzV1_4504984382)
