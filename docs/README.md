您好！这里有一份网络简历，请查收！

## 个人简介

**吴煌**，统计学硕士，2年计算机视觉与深度学习工作经验，5年机器学习项目经验，深耕AI+教育领域，并在K12在线教育领域有丰富的AI产品落地经验。喜欢钻研，研究生期间发表3篇SCI/EI检索论文；皮实稳重，经得起压力与挫折并吸收困难经验完成既定目标；愿意分享，乐于思考和交流且常在个人网站上分享所学所思。从事人工智能相关行业，主攻方向是计算机视觉与深度学习，目前在上海一家K12教育公司担任CV算法工程师，主要职责是负责将计算机视觉技术与公司业务相结合，已推出“Tais-Toi计划”用以增强在线课堂趣味性和互动效果，“水银计划”用以实现离线课堂视频的品控功能，“轻轻AI赋能平台”用以整合当前的技术积累和自研功能展现，“在线课堂质量评估系统”实现K12教育一对一在线课堂教学质量自动评估功能。

## 专业技能

统计模式识别（LR, Bayes, SVM, ID3, C4.5, CART, RF, Boosting, Stacking, Blending）

卷积神经网络（VGG, Inception, ResNet, FCN）

通用目标检测（YOLOv3, Faster-RCNN, SSD）

人脸检测和识别（MTCNN, PCN, facenet, RetinaFace, insightFace）

场景文字检测和识别（CTPN, EAST）

人体动作识别（HMM, LSTM）

编程技能（C/C++, Python, Go, MATLAB, PHP, JavaScript）

计算机视觉与深度学习（OpenCV, Dlib, Scikit-Image, Keras, TensorFlow, Pytorch, MXNet）

机器学习与数据挖掘（Scikit-Learn, XGBoost, LightGBM）

## 其他信息

性别：男

民族：汉

学历：统计学硕士

研究方向：统计模式识别

从事领域：人工智能+在线教育

联系邮箱：wuhuang@outlook.com


## 工作经历

### 2018/7 ~ Now 上海轻轻信息科技有限公司@算法工程师

## 项目经历

### 在线课堂质量评估系统（2020/1 – Now）| 团队Leader 

#### 基于计算机视觉、自然语言处理和语音识别等AI技术实现在线课堂教学质量自动评估系统。 

1）对接业务方了解业务需求，理解业务模型并转换成技术可实现的解决方案，产品性能分析、技术可行性研究并进行技术选型和模型设计，随时追踪最新的前沿技术和落地算法。

2）实行“先有后优”的原则，选型和模型确定后采用“低耦合”策略，首先完成项目Pipeline，后期不断优化算法、更新模型逐步提升效果。

3）协调和拟定语音处理、图文识别、文本分析人员的时间配置和工作内容，定期验收与会议评审，根据结果改进工作并对技术资料归档和总结。

### AI赋能平台（2019/10 – 2020/1）| 团队Leader

#### 建立公司自研AI技术内宣平台并基于容器技术构建AI服务的WebAPI。

1）设计公司AI微服务框架、实现流程和接口类型，并基于业务要求和云原生理念定义拆分粒度，实现多个微服务聚合成一个应用服务。

2）基于容器技术Docker构建微服务的调用接口，使用Python+Flask实现功能RESTful API，Nginx实现负载均衡，统一调用规范并建设宣传展示网页 ( https://ai.changingedu.com )。

### 水银计划（2018/12 – 2019/10）| 个人Leader

#### 基于视频图像等AI技术实现轻轻课堂一对一在线视频的智能品控工作

1）人脸检测功能，基于Retinaface模型finetuning，在Backbone上使用轻量级骨干网络MobilenetV2替换掉ResNet152在CPU上达到实时检测；在损失函数上调整人脸分类损失函数和包围框回归损失函数的权重系数，加大人脸分错的惩罚力度提高召回率；在特征融合时去掉低层特征，减少关注业务无关的小脸特征，加快训练和推理速度。

2）人脸识别系统，包括1vs1比对和1vsN识别， 早期使用MTCNN+facenet（Tensorflow）搭建人脸识别系统，现在更新为RetinaFace+insightface（MXNet）。新版系统准略率更高，对于侧脸和遮挡情况更加鲁棒。

3）板书整洁识别，采用OCR技术识别老师的板书是否整洁，具体是使用Advanced EAST模型实现文本检测功能。

4）竞品Logo检测，基于YOLOv3实现Logo检测和分类。调整location，objectness，classification 项的系数并添加Focal Loss到损失函数，加大对困难样本的学习能力。另外，更改Backbone为MobilenetV2可提高训练和推理速度。

5）着装规范识别，基于Pytorch+Deeplabv3plus的人像分割技术，对业务适用的MHP数据集进行fine-tuning得到业务模型。

### Tais-Toi 计划（2018/7 – 2018/12）| 个人Leader

#### 开发Windows客户端版实时人脸检测，光线识别和美颜贴纸功能的SDK。

1）实时提取视频的亮度（光线明暗），饱和度（色彩鲜艳），色调（色彩主调）和对比度（画质清晰度）等客观参数实现视频质量检测，并结合实际教学场景自动调节光线增强画质，即太暗补光和太亮降光。

2）采用LBP+Gentle AdaBoost（libfacedetection）实现实时人脸检测和人脸关键点检测功能，并采用双边滤波和ColorLUT颜色滤镜技术实现磨皮和美颜功能。

3）基于人脸关键点实现实时动态贴纸功能，并进行贴纸自动缩放和旋转、抖动稳定以及移动平滑等优化工作。

4）结合SSE4.2指令集重编译OpenCV，C++编写SDK并打包成DLL文件，并根据业务需求均衡性能和损耗，达到CPU实时应用。

## 教育经历

### 2015/9~2018/7 安庆师范大学@统计学

### 2011/9~2015/7 安庆师范学院@计算机科学与技术

## 研究成果

主要研究方向为机器学习(ML)、模式识别(PR)和人体动作识别(HAR)。课题是基于骨骼数据提取运动特征来识别人体动作，项目论文和代码均托管在 GitHub 上( https://github.com/vic9527 )。

### 内容：

1）提出了一种基于分层策略的人体动作识别方法。该方法是根据人体解剖学的层次结构和人体运动学的物理特性，结合动作粒度的粗细，将人体动作进行分层识别，并在每一层提取不同的运动特征和选择合适的分类器。

2）提出了一种基于自选择机制的人体动作识别方法。该方法就是在分类器构造环节中，为了消除人脑经验等主观因素对分类器选择的影响，设计了一个最佳分类单元，其内部是常见的机器学习分类算法，通过数据来训练每个分类器，让数据选择最适合它的分类器。

### 论文：

1. Human action recognition method based on hierarchical framework via Kinect skeleton data (DOI: 10.1109/ICMLC.2017.8107747,  EI: 20180904842839)

2. Accurate Hierarchical Human Actions Recognition from Kinect Skeleton Data (DOI: 10.1109/ACCESS.2019.2911705,  SCI: 000466798900001)

3. Hierarchical Human Action Recognition with Self-Selection Classifiers via Skeleton Data (DOI: 10.1088/0253-6102/70/5/633,  SCI: 000451760400018)

4. 基于骨骼数据的人体动作识别方法研究（研究生优秀毕业论文）

## 学术交流：

1）参加国际机器学习与控制论会议（The 2017 International Conference on Machine Learning and Cybernetics）并口头报告（Oral Presentation）（2017.7，宁波，宁波凯洲皇冠假日酒店）

2）参加第六届中国科技大学《计算机图形学》暑期课程（2017.7，合肥，中国科学技术大学）

3）参加Google师资培育与课程建设(人工智能)研讨班（2017.6，兰州，兰州大学）

4）参加国际健康医疗科学与工程会议（The 2017 International Conference on Healthcare Science and Engineering）并口头报告（Oral Presentation）（2017.6，郑州，郑州大学）

5）参加2017全国深度学习技术应用大会（2017.3，北京，北京航空航天大学）

6）参加第三届智能感知与可视媒体计算学术研讨会（2016.10，安庆，安庆师范大学）

7）参加第五届中国科技大学《计算机图形学》暑期课程（2016.7，合肥，中国科学技术大学）

8）参加第十二期计算机视觉（CCF-CV）前沿技术及应用系列报告会（2016.4，合肥，安徽大学）


## 实习经历

### 2014/10~2015/4 安庆市广进科技有限公司@网站程序员

这是本人在大四时期的实习工作，参与网站制作（HTML+CSS+JavaScript+PHP），服务器搭建（ECS，OSS）和项目运维以及活动策划，打造一款面向乡镇市场的外卖订餐的服务平台。此项目是面向乡镇市场的外卖服务平台，主要是填补美团或者饿了么外卖在乡镇市场的空白，平台虽小，五脏俱全。(网址：www.waisongke.com)

### 2014/2~2014/6 安庆海军职校@网页设计课程老师

大三时期参加“顶岗支教”志愿活动任教一个学期，主要职责和工作内容如下：

(1)当时任海军职校支教小组的组长，负责统筹管理本次支教任务的顺利实施。

(2)授课任务是网页设计，面向中专班的学生。

(3)同时任代理班主任，负责管理学生纪律。

(4)支教任务顺利完成，并获“优秀实习生”和“顶岗支教优秀生”。

## 个人荣誉

1）研究生期间荣获"优秀共产党员"荣誉称号（2017/4）、一等学业奖学金（2017/10）和校级双优生（2018/3）

2）2016年国家级大学生创新创业训练计划项目#2016/10#国家级 (新闻地址: http://www.moe.gov.cn/s78/A08/A08_gggs/A08_sjhj/201609/t20160929_282721.html)

3）安徽省第三届"生态安徽"青少年公益广告大赛平面类优秀奖#2013/06#省级 (新闻地址: http://www.ahedu.gov.cn/28/view/226816.shtml)

## 个人媒体

**微信公众号：剑指 AI ( SwordAI )**

**阿Q书屋：** https://www.aqexam.com

**AI从业论坛：** https://bbs.aqexam.com

**K12在线教育平台——学而时习之：** https://www.k12coursera.com

## 业余技能

**办公软件Office**（Word, Excel, PPT, WPS）

**网站建设**（PHP + HTML + CSS + JavaScript）

**论文写作**（Latex, Acrobat）

**视频剪辑**（绘声绘影，EDIUS，Premiere）

**绘图制表**（Visio, Photoshop）

**思维导图**（百度脑图，XMind）

**电脑达人**（装系统，修电脑）

**文艺爱好**（微电影编剧与拍摄， 小说阅读与创作）

## 个人宣传

任职期间获得公司管理层的认可，特摄“成长足迹”短视频以兹鼓励，树立榜样。

<video id="video" controls="" preload="none" poster="http://qiniu.aqexam.com/whcv.png" width="100%">
      <source id="mp4" src="http://qiniu.aqexam.com/huang.mp4" type="video/mp4">
</video>

## 自说自话

文能提笔写论文（英文论文撰写），武能拆机修电脑（电脑达人）；

进可统计做分析（研究生工作），退可建网包运维（PHP网站开发）；

上爱编剧拍视频（自编自导自演过微电影），下爱构思写小说（17K小说上有一个部...）；

前会翻墙查资料（额...比较会找资源），后会演讲装斯文（曾支教当老师...）

## Self Introduction

Huang Wu (English name is Vic Woo), Master of Science (MSc), graduated from Institute of Statistics in School of Computer and Information, Anqing Normal University, Anhui, China. The main research directions and interests are in Machine Learning (ML), Pattern Recognition(PR) and Human Activity Recognition(HAR). Furthermore, the more attentions are paid on Big-data technology and Deep Learning, working on artificial intelligence in education about ML&DL, HAR, DIP, CV and so on.

> Huang Wu, Master of Statistics, graduated from Anqing Normal University. The main research interests include Computer Vision (CV), Human Action Recognition (HAR) and Deep Learning (DL). Currently, working on Artificial Intelligence (AI) in education.
Huang Wu received the master’s degree in statistics from Anqing Normal University. He is currently working on artificial intelligence in education. His current research interests include computer vision, human action recognition, and deep learning.
> 
> from: https://ieeexplore.ieee.org/document/8693506/authors#authors
