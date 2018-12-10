基于移动充电的区域巡查无人机群体协作系统设计
==============
设计描述
--------------
以最大化区域巡查为目标，结合地面移动充电基站，实现无人机群体自组织协作飞行。本设计包含以下四部分内容：1）以区域巡查为目标，设计合理的无人机自组织群体协作飞行技术，并针对不同的障碍环境实现自组织避障以及队形变形，最后以可视化形式展示区域巡查成果；2）设计地面移动平台，接供接触式无线充电，在与空中机器人充分交换状态信息条件下，完成中继充电，从而提升群体续航能力；3）设计地对空观测系统，确保子任务2中继充电任务实现的鲁棒性；4）根据已知移动充电站能源储存总量，以及无人机充放电性能特性，设计最优充放电策略，实现群体作业能力最大化。

期望结果
--------------
实现一套完整的地面充电中继-空中无人机自组织协作群体，全面提升作业时长。通过自主充电策略调度，用于进行充电的总能耗不应高于系统总储能的20%。在地面充电中继能源可持续补给的情形下，实现无人机群体无限时长执行任务。协作群体具有分布式智能，单一个体的损毁不影响协作群体任务的有效完成。

Preliminary Design
------------------
* **Area Coverage Problem.**<br>
    Given a square area, the solution is able to allow a swarm to cover the whole area.
    The algorithm should consider collision avoidance and coverage efficiency.
* **Dynamic Scheduling Problem.**<br>
    This may be related to the Operations Research. Consider both current and future feasibility.
* **Object Recognition and Localization.**<br>
    First, use OpenCV to detect and track markers. Second, control drones to land on the ground station.
* **Ground platform.**<br>
    This is for the next step.