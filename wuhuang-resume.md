 <center>
     <h2>吴 煌 <a style="font-size:11px;background-color:black;color:#fff;
border-radius:8px 0px 8px 0px;padding:3px 6px;vertical-align:12px">算法工程师</a></h2>
     <div>
         <span>
             <img src="assets/phone-solid.svg" width="20px">
             <a href="tel:15856528646">15856528646（微信同号）</a>
         </span>
         ·
         <span>
             <img src="assets/envelope-solid.svg" width="20px">
             <a href="mailto:me@whing.cn">me@whing.cn</a>
         </span>
         ·
         <span>
             <img src="assets/github-brands.svg" width="20px">
             <a href="https://github.com/vic9527">Vic9527</a>
         </span>
         ·
         <span>
             <img src="assets/rss-solid.svg" width="20px">
             <a href="https://whing.cn/blog">我的博客</a>
         </span>
     </div>
 </center>

​        统计学硕士，3年工作经验，主要从事CV研发落地和工程化部署，熟悉常见的深度学习算法，能够快速搭建、改进和训练深度网络，熟悉Python3和C++11。项目经验包括人脸检测与识别，目标检测，人像分割，人体动作识别，风格迁移，数据挖掘，个性化推荐，ASR，OCR等。2篇SCI和1篇EI论文，业务思维能力较强，有5~10人团队管理经验。

#### <img src="assets/briefcase-solid.svg" width="22px"> 工作经历

- **上海明胜品智人工智能科技有限公司（明略科技）               智能数据部                2020/12 ~ Now**

**[Tasks]** 设计并实现面向客户的CV解决方案，负责参考设计、POC、算法开发和工程化部署。

- **上海轻轻信息科技有限公司（轻轻教育）                               BI 部门 	         	 2018/07 ~ 2020/12**

**[Tasks]** 结合在线教育场景的AI算法研发与应用，负责实际业务中图像相关问题的分析与建模，并推动项目落地和持续优化。

#### <img src="assets/project-diagram-solid.svg" width="23px"> 项目列表

- **人脸检测与识别			（2018/07 ~ 2020/12）	Owner**

**[Target]** 本项目为公司智能美颜贴纸、视频教学品控、人脸风控系统和在线课评估提供基础功能。

**[Action] **
	 **①** 基于Retinaface模型结构，在骨干网络中添加注意力机制（SE模块），使用K-means聚类方式设计Anchor的尺度和比例，采用FPN技术实现多尺度信息融合，增强小目标的检测能力。
	 **②** 人脸检测任务损失函数上，采用Focal Loss作为分类损失，GIoU Loss作为Bounding Box损失，Wing Loss作为Landmark损失，构建多任务学习。
	 **③** 人脸识别任务损失函数上，基于度量学习方法实现one-shot人脸表征学习，使用ArcFace Loss作为Facenet的学习目标。
	 **④** 训练过程中进行数据增强，采用 AdamW（在 Adam 中加入正则项）优化器进行权重更新，使用Warm-up策略保持模型训练稳定性，结合OHEM方法加强困难样本的权重。
	 **⑤** 独立实现美颜滤镜和动态贴纸功能，针对效果显示问题，优化贴纸自动缩放和旋转、抖动稳定以及移动平滑等问题，使用C++封装SDK并打包成DLL动态链接库。
	 **⑥** 基于Docker部署人脸一对多识别工程，并采用空间换时间的策略，在服务器部署Milvus向量搜索引擎计算相似度加速人脸检索。

- **实时背景抠图			 （2019/10 ~ 2020/04）	Owner**

**[Target]** 本项目为公司教学客户端（轻轻课堂）提供实时人像抠图和背景替换功能。

**[Action]** 
	 **①** 基于SINet轻量级人像分割模型，改进空间压缩模块，将固定窗口的平均池化修改为空间金字塔池化（SPP）结构，增加多尺度信息。
	 **②** 在多尺度信息融合的过程中，对不同分辨率的特征图（由SSP生成）进行处理，构造上采样、通道拼接和逐点卷积模块做融合操作，增强上下文信息。
	 **③** 基于MNN框架进行量化压缩和加速推理，为了减少模型压缩的损失，通过训练量化（QAT）来提高量化模型的精度。
	 **④** 在替换新背景时，对人像Mask边缘采用高斯模糊，实现图层融合时的平滑过渡。
	 **⑤** 使用C++封装成DLL动态链接库，并集成到x86+Windows客户端，实测在i5笔记本下单线程每帧推理速度在25ms左右，达到CPU实时。

- **竞品LOGO检测			（2019/02 ~ 2019/08）	Owner**

**[Target]** 本项目为防止教师在教学过程中使用含有竞品公司Logo的PPT，方便平台规范授课行为。

**[Action]**
	 **①** 基于单步检测器YOLOv3实现，选用ResNet50作为Backbone；在部分网络层使用可变形卷积，缓解Logo扭曲和方向旋转等问题；采用Mish激活函数，可以稳定网络梯度流和提高泛化能力。
	 **②** 修改原坐标回归损失Smooth-L1 Loss为GIoU Loss，使得学习目标更加关注预测框与真实框的重合度，并使用DIoU-NMS提升bbox预测的准确率。
	 **③** 基于Flask和RESTful编写WebApi接口，使用Docker部署服务，Nginx做负载均衡。

- **智能冻仓OCR			（2020/12 ~ 2021/3）	Owner**

**[Target]** 本项目作为乙方向甲方KFC提供冷链包装OCR识别服务，包括产品名称、货品编码、有效日期、生产日期等用于货物统一管理。

**[Action]** 
	 **①** 采用基于分割的自然场景文本检测方法DBNet实现文本检测，采用基于CNN+Bi-LSTM+CTC Loss结构的CRNN网络实现文本识别，结合业务场景数据集进行迁移学习。
	 **②** 使用Style-Text数据合成工具，使用少量目标场景的图像，批量合成所需的标注数据，构造用于业务场景识别的数据集。
	 **③** 编写正则匹配关键信息并结构化输出，完成智能识别冷链包装信息的PoC、接口定义和模型转换以及在不同边缘盒子（intel, arm, nVidia）上的安装部署工作。

- **师资推荐系统			（2020/01 ~ 2020/12）	Owner**

**[Target]** 本项目为提高测评课出席成功率和降低助教筛选成本而研发的自动化师资推荐系统。

**[Action]** 
	 **①** 基于公司业务场景设计师资匹配系统，构建特征库及用户画像体系，合理定义与选取训练和测试数据，完善ABtest、Badcase分析流程；
	 **②** 改进LightGBM模型增强对类别非平衡数据的预测能力，在业务模型上引入衰减策略缓解师资推荐中的马太效应；
	 **③** 根据模型线上运行情况，更新迭代模型，提升模型性能。


#### <img src="assets/graduation-cap-solid.svg" width="22px"> 教育背景

- **2015/09~2018/07                        安庆师范大学                       统计模式识别                               硕士 **

**[Reaps]** 一等奖学金，双优生，2次国际会议Oral Presentation，2篇SCI和1篇EI论文。

- **2011/09~2015/07                        安庆师范大学                       计算机科学与技术                       本科**

**[Reaps]** 顶岗支教，优秀毕业生，2016年国家级大学生创新创业训练计划立项项目。

#### <img src="assets/paper.svg" width="22px"> 出版论文

**[1] Accurate Hierarchical Human Actions Recognition from Kinect Skeleton Data**

**[[Link](https://ieeexplore.ieee.org/document/8693506)&[PDF](https://github.com/vic9527/KAR_Articles/raw/master/2.IEEE-Access：Accurate Hierarchical Human Actions Recognition From Kinect Skeleton Data.pdf)]** IEEE Access (DOI: 10.1109/ACCESS.2019.2911705, *SCI: 000466798900001*)

**[2] Hierarchical Human Action Recognition with Self-Selection Classifiers via Skeleton Data**

**[[Link](https://iopscience.iop.org/article/10.1088/0253-6102/70/5/633)]&[PDF](https://github.com/vic9527/KAR_Articles/raw/master/3.CTP：Hierarchical Human Action Recognition with Self-Selection Classifiers via Skeleton Data.pdf)]** Communications in Theoretical Physics (DOI: 10.1088/0253-6102/70/5/633, *SCI: 000451760400018*)

**[3] Human action recognition based on hierarchical framework via Kinect skeleton data**

**[[Link](https://ieeexplore.ieee.org/document/8107747)&[PDF](https://github.com/vic9527/KAR_Articles/raw/master/1.ICMLC2017：Human action recognition method based  on hierarchical framework via Kinect skeleton data.pdf)]** 2017 International Conference on Machine Learning and Cybernetics (DOI: 10.1109/ICMLC.2017.8107747, *EI: 20180904842839*)