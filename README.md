# Shift AI models to real world products

Readme [中文](/README.md) | [English](/Translate/README_EN.md)

  > 欢迎协助完成英文版翻译工作。

## 前言

离开老东家快一年了，在半休息半工作的轻量负荷下，可以系统的做一些事情：1、把快给管理荒废了的撸码捡起来，补补DeVOps这条Pipline各种工具的功课，看看React，VUE，Flutter这些新东西；2、从数学到理论系统性的看看DL的东西；3、瞎琢磨。同时，在各路猎头的对接下，和一些国内AI领域的公司有过工作岗位的沟通与面试，基本上分为以下几类：  

  > - AI头部创业公司
  > - AI中小创业公司
  > - 国外AI创业，准备回国内落地
  > - 准备进入AI领域（毕竟是风口）

聊了也算不少家，皆无果。究其因，无非就是`人家看不上我`，`我看不上人家`这两种。一方面年龄40+，在当下这个环境，这是最大的竞争劣势；另一方面多年的工作重心在产品、架构、项目以及技术管理上，写代码这件事基本给废了；再一方面，虽然16年开始上手AI，做的项目也交付了，但不是科班，显然没有扎实的DL基础；最后，怎么说呢，也许就是个靠嘴干活的渣渣。  
所以我关注的机会，更多的是偏向需要技术支撑的综合技能要求偏高的方向，而不是“计算机视觉研究员”、“高级程序员”这种明显力不从心的岗位，实际的无果原因基本是`大多数沟通或者面试，聊着聊着要么“跑偏了”，要么实在是无法继续下去了，只能想办法快速结束，继续下去只能是互相浪费时间`，具体有以下几种情形：  

  > - JD方向是诸如“工程化落地与交付”、“AI应用示范”等的，基本都是聊1到2个小时，但真正与JD关键词相关的问题好像没有超过10分钟的，实在不知道JD的要求，面试官是否清楚；
  > - 最奇葩的一家，目标是找“有B/G领域项目交付经验的CTO”，技术面第一个问题：`Python的tuple和list什么区别`；然后是React、MongoDB、Redis、Docker等；近一个小时，没有一个DL问题，没有一个产品、交付的问题；问到Flask如何在生产环境部署，真的抓狂了，这是面3年以内Python开发还是拿我闹着玩呢？答：Python Web就是写Demo，生产都是 Java， C#， .NET Core这些，演示就是laptop开发环境把 http 拉起来，没部署过生产环境。只求赶快能让人家判断我不行，面试结束。
  > - 遇到过很有“追求”的问题：`你来规划我们的AI产品，如何能确保在2年后落地还是属于领先的技术水平`，我的天，在2个月不看新闻，不读Paper的就要落伍的AI时代，要做到2年后落地还要技术领先，我不知道谁能做到，反正我肯定做不到。
  > - 遇到过极其“好学”的CTO来面试，3个多小时，简直就是一场AI基本概念讲座，我问了一个问题，就后悔前面3个多小时的“科普”了：“贵公司的‘人工智能应用总监’目标是解决哪些场景的DL问题？”。答案基本是：还没想好，有做AI的需求，但是具体做什么需要入职后再讨论。
  > - 某团队有个细分的算法，产品化的程度基本比Demo强不了多少，准备做B/G市场项目，听了好多人家的设想，抛出去灵魂三连问：`1、一个算法其实就是看起来能解决某个领域问题的一个功能点，但是对于B/G市场，用户需要的解决方案和完整的产品，咱们这方面有什么规划？2、以我的理解（非常巧，一个以前带过的产品经理在做的产品和他们的方向很相似，正好这哥们儿之前找我聊过不少，要我给点建议）要做这方面的项目，还需要有……，这些算法和产品规划，有没有时间和成本的考虑？3、B/G项目是一个长周期的事情，尤其是这种新兴事物，用户教育和市场培育需要投入和耐心，这方面公司有没有做好长期作战的储备？`。人家思考后，没有回答，给我了一个问题：“`那你觉得我们的商业模式应该是什么呢？`”。面试互怼，好欢乐。
  > - AI头部公司CTO，分管的异地研发中心是要做工程、产品化落地的，亲自面试没有一个工程、产品与交付的问题。

其实，所有的面试，我都是做好准备“**挂**”在DL的算法、框架或者各种参数的问题上，但，很不幸，这些问题真不多，只有一次，Caffe没用过，问题没法回答；没有一家对我之前落地的项目感兴趣，去追问一些工程、产品和算法实现细节以及对项目的反思，对此，略感惊讶。  

五年前，不提**Big Data**、**Hadoop**出门都不好意思跟人打招呼，这两年公司不想办法往**AI**、**Block Chain**方向靠，都不好意思更新网站，在这个热闹非凡，热点轮转的时代，以上种种意想不到的情况，在一定程度上来说，也是必然。  

2、3年前基本少有人对 AI 落地非常关心，“**豪华团队 + Paper + 比赛刷榜**”就是一个团队最好对背书，不管是谁的钱，投资总是需要考虑回报这个问题的，在大方向都转向比拼落地能力的2019年，为什么没有感觉到这个行业对于落地的急迫，依然有对豪华团队的迷之自信，可看看知乎的这个问题：[清华AI四大公司PonyAI、RealAI、Face++、商汤未来能否达到Google、微软的高度？](
https://www.zhihu.com/question/334397581/answer/748974753)。必须要说，对于这些横跨学术与产业的技术大牛的贡献，我是无比敬佩，IT领域也算混了二十年，从来没见过哪个方向有如此强大的开源与分享动力，框架、论文、实现代码、权重与参数（预训练模型）大家你争我抢，毫无保留的都给社区随便用（当然从开源协议来说，大多都是没法商用的，比如ImageNet下载协议的第一条就是`Researcher shall use the Database only for non-commercial research and educational purposes`，做CV的有几家能全部避免使用ImageNet的相关产物？为了下数据集，找在学校任教的同学、朋友借edu邮箱，前几年估计很多产业界的人都干过这样的事情）。用半年业余加班时间就能从0开始做出检测算法Demo，活着爬出销售挖的坑，没有这些开源分享，就算有“飘柔”般的自信和“梁静茹”给的勇气，这事情也是想都不敢想的。  

其实，对于非AI领域的公司积极拥抱AI，出现的各种理解与认识偏差，是能理解的（毕竟，我就是摸着石头一步一步往前走的），但是对于**Scientists**坐镇的AI公司，现阶段也不缺钱，工程化、产品化落地情况依然不乐观，这件事我是有点困惑的。  

对于AI的落地，我相信，一定会有：“**训练几个 model 搭几个 inference 的 APIs，业务去调用不就好了么？**”这样的简单想法存在。我的理解是：对于AI这个“边缘”技术领域，如何从解决一个特定问题的构想到最终的工程化落地的产品、项目，虽然看起来都是写代码，但是和我们传统的软件开发过程、产品思考、交付能力要求相比，还是有较大差异的。  

基于这种理解，结合工作近二十年对售前、产品、研发、咨询、交付与技术管理的认识与实践，入门DL后的学习探索与项目落地交付实践，还有近一年来较为深入的阅读、学习与思考，把我对于如何实现`Shift AI models to real world products`的一孔之见与相关实践回馈给社区。  

考虑到我的知识局限性（熟悉B/G项目和产品，略懂CV和监督学习），所以内容和其中的一些建议与举例，更倾向监督学习、CV在B/G端的产品与项目落地，对于机器学习的NLP、RL等领域以及像推荐算法这些在线学习的互联网方向的应用，争取也能做一些建议。

## 目录

### [一、概述](/ch01_Overview.md)

### [二、机器学习项目基本过程](/ch02_Lifecycle-of-a-ML-Project.md)

### [三、机器学习项目团队组成](/ch03_ML-Teams.md)

### [四、产品经理的工作挑战](/ch04_Product-Manager's-Challenge.md)

### [五、产品/项目启动](/ch05_Project-or-Product-Setup.md)

### [六、数据采集、标注与管理](/ch06_Data-Collection-Labeling-and-Management.md)

### [七、训练与调试](/ch07_Training-and-Debugging.md)

### [八、模型部署与测试](/ch08_Deployment-and-Testing.md)
### [九、机器学习的DevOps](/ch09_ML-DevOps.md)
### [十、项目售前与解决方案](/ch10_Project-Consulting-and-Solutions.md)
### [十一、项目交付](/ch11_Project-Delivery.md)


## Authors

* **Kevin Di**

  [![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/lonelygo?style=social)](https://twitter.com/lonelygo)



## License

[![CC-BY-SA-4.0](https://img.shields.io/badge/license-CC--BY--SA--4.0-brightgreen)](/LICENSE)

## Acknowledgments
