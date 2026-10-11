# 四旋翼脉冲神经网络扰动补偿资料

本仓库对应论文 Recurrent Spiking Disturbance Compensation for Quadrotor Attitude Control。

## 下载完整资料

打开右侧 Releases，下载名为 SNN_Quadrotor_Reproducibility_v1.0.0.zip 的附件。

GitHub自动显示的 Source code (zip) 只有仓库首页文件。完整训练数据、模型和程序在上面的专用ZIP附件中。

资料包括24段完整训练和开发数据、选定及最终模型、211000步训练记录、30组相同条件下的90次控制运行，以及对应的程序、六张表和六张图。全部对比结果保留。

## 检查文件

解压后进入 ras_reproducibility 文件夹，在终端运行：

```text
python verify_reproducibility.py --hashes-only
python verify_reproducibility.py
```

第一条检查文件是否完整，使用Python自身功能。第二条还会从保存的数据重新算指标，需要安装NumPy。它们都只检查已有记录。重新运行控制仿真的入口和所需软件，见ZIP中的README。

## 本资料说明的研究范围

SNN提供控制中的z3扰动补偿数值，原ESO提供角度和角速度并继续内部计算。五组扰动重复使用同一个已训练网络。资料保留完整误差、运行条件和电机指令变化。该资料不提供特殊芯片上的速度或能耗测量。

公开副本已经去掉电脑用户名和绝对路径，并记录新旧文件之间的对应关系。数据数组、模型张量存储和实验条件保持。当前发布未额外指定程序和数据的再利用许可。
