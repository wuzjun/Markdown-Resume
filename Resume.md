 <center>
     <h1>吴焯钧</h1>
     <div>
         <span>
             <img src="assets/phone-solid.svg" width="18px">
             13690139909
         </span>
         ·
         <span>
             <img src="assets/envelope-solid.svg" width="18px">
             w1159904119@gmail.com
         </span>
         ·
         <span>
             <img src="assets/github-brands.svg" width="18px">
             <a href="https://github.com/wuzjun">wuzjun</a>
         </span>
     </div>
 </center>

## 个人信息 

&emsp;&emsp;吴焯钧/男/1999&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;本科/华南理工大学广州学院机器人工程专业

&emsp;&emsp;工作经验：1年&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;求职意向：嵌入式工程师

## 工作经历
*深圳市正浩创新科技股份有限公司* - 嵌入式软件工程师 研发体系&ensp;&ensp;&ensp;&ensp;2022.5 ~ 至今

研发项目：1.[智能割草机](https://www.ecoflow.com/eu/blade-robotic-lawn-mower)；2.[割草机清扫套件](https://www.ecoflow.com/eu/blade-robotic-lawn-mower)；3.[River系列](https://www.ecoflow.com/cn/river-2-portable-power-station)

## 项目经历

*智能割草机* - 深圳市正浩创新科技股份有限公司&ensp;&ensp;&ensp;&ensp;2022.7 ~ 2023.7

**项目描述：** 限定割草范围内后，可自主在区域内规划路线，沿轨迹实现割草功能，并在完成任务后能自动回充。

- **运动控制：** 底盘运动使用后驱双动力轮，在草地会有走不直问题，使用角度+角速度+线速度闭环方法解决，能做到在草地直线运动 10 米内左右偏移不超过 5cm；刀盘升降运动使用单磁编+步进电机方案，由于刀盘结构上有遇障碍物避障功能，避免过多 if 嵌套将升降动作抽象为具体数字模型，能完成功能需求且实现升降堵转检测。
- **传感器：** 按照文档编写 MMC，IMU 等传感器驱动，并解决使用中问题（校准偏移量等）。
- **通信模块：** 编写通信模块驱动，排查串口 IAP 升级缓慢等问题，分析计算 CAN，UART 负载率等参数指标。
- **研发自测：** 根据功能需求编写测试用例，按照要求提交对应pr以及测试结果；负责固件打包发布，版本功能验证。
- **产测：** 负责单板 fct 治具、各种组件（升降组件等）、整车治具的通信接口，步骤编写。完成试产和 5k 量产需求；

*割草机清扫套件* - 深圳市正浩创新科技股份有限公司&ensp;&ensp;&ensp;&ensp;2022.5 ~ 2023.7

**项目描述：** 连接上智能割草机后，完成清扫收集落叶功能。

- 升降运动使用推杆电机+霍尔方案，会有控制僵硬且不精准问题，通过估算距离+霍尔校准能解决并实现传感器失效故障检测；按照需求编写测试用例，提前识别生产风险；完成试产及量产需求。

## 教育经历

&emsp;&emsp;第二十届 RoboMaster 机甲大师赛&ensp;&ensp;&ensp;&ensp;2021.9 ~ 2020.9&emsp;电控组组长和步兵机器人电控负责人。

&emsp;&emsp;第十九届 RoboMaster 机甲大师赛&ensp;&ensp;&ensp;&ensp;2020.9 ~ 2019.9&emsp;哨兵机器人电控负责人。

### 比赛经历

一、 比赛 - 哨兵机器人 - 独立开发（电控）&emsp;&emsp;&emsp;&emsp;2019.9 ~ 2020.9

- 作为 RoboMaster 赛事中哨兵机器人：主要在轨道上自动索敌并移动规避伤害。

- **技术上：** ①[HAL 库](https://misty-drip-914.notion.site/STM32-cubemx-6201be48c5b74bd8a1b7d7686808b318?pvs=4)快速开发外设、②[运动算法仿真](https://github.com/wuzjun/2020RM_Sentry)、③使用 DSP 库、④FreeRTOS 实现任务管理

- **实现效果：** ①解决了底层代码移植出错等问题，提高开发效率、②提前验证电控逻辑和算法，减少“脑补”出错、③提高自动追击算法中数学函数运行效率

二、 比赛 - 步兵机器人 - 独立开发（电控）&emsp;&emsp;&emsp;&emsp;2020.9 ~ 2021.9

- 作为 RoboMaster 赛事中步兵机器人：主要在赛场上灵活游走打击。

- **技术上：** ①[HAL 库](https://misty-drip-914.notion.site/STM32-cubemx-6201be48c5b74bd8a1b7d7686808b318?pvs=4)快速开发外设、②[串级和动态 PID 算法](https://misty-drip-914.notion.site/PID-287da5b821c64573934ce085139cd33b?pvs=4)、③[PVD断电保存](https://misty-drip-914.notion.site/15-PWR-c429a437c01f4eb39d1947f2702402cd)、④使用 DSP 库、⑤FreeRTOS

- **实现效果：** ①提高开发效率、②串级 PID 提高云台精准度；动态 PID 提高底盘跟随响应，而且建立一套系统的调参方法，大大减少调参消耗时间、③各种校准数据随断电后会自动保存、④自瞄预测算法需要矩阵运算

- [开源步兵代码地址](https://github.com/wuzjun/2021RM_Infantry)

### 奖项与专利

- 竞赛：
    - 2020 年 8 月份荣获 RoboMaster 机甲大师线上赛全国二等奖。
    - 2021 年 4 月份荣获 RoboMaster 高校联盟赛步兵机器人省赛二等奖。
    - 2021 年 8 月份荣获 RoboMaster 步兵竞速与智能射击单项赛全国一等奖 。
    - 2021 年 8 月份荣获 RoboMaster 机甲大师超级对抗赛全国二等奖。
- 专利：

    - 名称：一种监控防御装置&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;公开号：215232051U
    - 名称：一种轨道移动装置的调整方法&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;公开号：112494924A
- 校内奖项：
    - 2018-2021 连续三个学年校三好学生，荣获三等奖学金&emsp;&emsp;证书：二级 C 语言程序设计

## 专业技能

- 熟悉使用 C（掌握分散加载），了解 C++
- 熟悉 STM32 各种外设配置和使用（USART，TIM等），熟悉使用 cubeMX 配置 HAL 编程，熟悉使用 FreeRTOS（任务，队列）
- 掌握 Linux 操作系统（进程，Makefile编译等）
- 熟悉使用 webots 运动模型仿真
- 熟悉使用Git、keil 5 和 vscode工具

## 致谢

感谢您花时间阅读我的简历，期待能有机会和您共事。