### 论文提纲
题目：基于深度学习的建筑企业安全管理信息系统的研究与实现
一、绪论
1.1 选题背景
1.2 研究意义
1.3 国内外研究进展
1.3.1 国外安全管理信息系统研究现状
1.3.2 国内安全管理信息系统研究现状
1.4 研究内容
1.5 技术路线

二、对工作流程中危险源辨识及风险评估
2.1 对风险及隐患信息进行规范统计和处理
针对整个企业生产建设过程对技术改造和企业管理等方面的危险、有害因素进行辨识。
将安全条例、规章制度录入安全知识库中，为用户提供安全知识参考。事故案例中常见的事故类型，包括应急组织、应急处置和注意事项，为用户提供应急救援预案案例，在线管理应急预案。不断更新安全知识，将理论知识结合实际做好安全管理工作，实现安全技术与管理的标准化和科学化。 

2.2 对生产作业环境进行风险评估
系统会检索出所设置的区域，选择不同的作业区域，进行安全评价。
选择要评价的方法，包括道氏指数法、作业条件危险性分析法、事故后果模拟法、安全检查表法，通过实现这些方法的计算程序，省去了繁琐的计算过程。

三、基于深度学习的作业区作业人员实时监控算法的实现
对于意外闯入非安全区域的人员进行跟踪检测并向相关安全负责人预警
可以通过实时画面对算法的检测情况进行直观了解，此时系统通过接口获取该设备在指定报警类型下的实时检测画面。
目前各施工作业区施工过程中的异常情况监测往往依赖于监控人员通过现场监控视频记录，或采用安全监督人员人工巡逻的方式对异常情况进行监测，无法及时获取每一个作业人员的情况。针对该问题，预期设计开发一种基于深度学习的作业区作业人员异常情况实时监控与识别模块，以保障施工作业区的生产安全。

3.1 异常行为数据集的建立
3.2 基于 AlphaPose 的作业人员异常行为检测方法
3.3 基于 EfficientNet 的作业人员异常行为识别

四、企业安全管理信息系统的设计

4.1 用户需求分析

4.2平台整体设计结构与模块组成
系统主要功能体现在信息管理、安全评价、安全控制三大功能模块，具体功能如下： 

4.2.1 系统开发技术简介
该系统后端控制部分主要采用SpringBoot+Spring MVC+Mybatis框架实现，数据库部分由MySQL提供支持。
基于深度学习的作业区作业人员实时监控算法采用 python 语言进行编写，Flask 框架对于两种语言间的通信在其中发挥了重要作用。

​4.2.2 信息管理模块
系统登陆界面：
为了提高系统的安全性设置用户登录。企业人员需要在系统中完成个人账号注册，录入后台数据库，检索到相应登录信息，便可以进入系统。
主要负责人可以查看用户的注册资料以及各个专业区科的相关信息。通过权限管理，可以进行角色设定、角色权限设置，可以添加信息、修改信息和查看所有信息，进行添加部门、查看所有部门和编辑部门。
个人信息管理：
实现包括姓名、性别、民族政治面貌以及出生日期、本人照片等信息管理，用户可以对个人信息进行填写修改，以及对密码进行重置，方便了系统管理员的统计与管理。
​作业区和设备信息管理：
实现作业区和设备信息的管理，主要包括对作业区安全程度的区分，设备信息查找和维修系统报备等操作。

4.2.3 安全评价模块
对工作流程中危险源辨识及风险评估

4.2.4 安全监控模块
基于深度学习的作业区作业人员实时监控算法的实现

4.3 非功能性需求分析 
非功能性需求包括时间特性、适应性、安全性、可靠性、可扩充性、互操作性、健壮性、易使用性、可维护性、可移植性、可重用性。
其中主要方面有：
（1）正确性与完整性
正确性是系统设计首要考虑的要素，系统在正常运行的状态下能否正确处理用户操作界面，满足用户性能需求。系统设计完整，各项功能能顺利执行，操作流畅，用户在使用系 统时能够准确处理各项操作。 
（2）实用性与易操作性
系统的研发设计需要以实际用户的需要为主体，结合公司实际需要，每一项功能模块的设计都需要站在使用者的角度，考虑到使用者的日常工作实际需要、操作习惯等，应该操作简单，能够很快被使用者掌握。工人文化程度普遍不高，因此便于用户操作是设计系统要求之一。界面设计简单不繁琐，有提示性的标识，提示用户下一步的动作，同时也要操作灵活。 
（3）安全性与运行可靠性 
系统开发的重要指标之一是长期稳定的运行，减少故障的出现，避免数据的丢失，出现故障时能给用户提示，或者自动处理因操作错误出现的故障。系统管理员分配给系统用户的账号和密码，登录后拥有不同的管理权限和不同的显示界面，避免了其他用户随意注册、泄露数据，具有较高的安全性。 

4.4 系统应用及效果分析

五、结论与展望
总结全文研究内容以及当前改进存在的不足指出，并提出下一步工作的改进方向。



我在了解了一些电子信息与互联网行业的基础知识和相关从业者信息之后，发现安全工程所教的东西宽泛而浅显，根本无法形成技术壁垒、行业护城河，这就导致了其他行业如果想进入这个行业的成本几乎为零，只能通过专业背景以及学历提升来挑选人材，也就是熬资质来晋升。而人们在面向就业的时候所展现出来的基础素质与综合素质是通过个人成长带来的，通常与专业所提供的平台无关，这使得大学四年在学校所消磨的时间大多被浪费掉了。