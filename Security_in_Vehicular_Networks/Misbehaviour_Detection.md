总结了一些车联网中不当行为检测相关文献。

## 综述
- S. Dong, H. Su, Y. Xia, F. Zhu, X. Hu and B. Wang, "A Comprehensive Survey on Authentication and Attack Detection Schemes That Threaten It in Vehicular Ad-Hoc Networks," in IEEE Transactions on Intelligent Transportation Systems, doi: 10.1109/TITS.2023.3297527. [[paper]](https://ieeexplore.ieee.org/abstract/document/10201386)
  - 现有的Sybil攻击检测方案可以大致分为五类：基于身份验证、基于位置验证、基于轨迹验证、基于资源测试（工作负载证明）和基于邻居列表。


## 机器学习方案
- Mohammed A. Abdelmaguid, Hossam S. Hassanein, and Mohammad Zulkernine. 2023. A VeReMi-based Dataset for Predicting the Effect of Attacks in VANETs. In Proceedings of the Int'l ACM Conference on Modeling Analysis and Simulation of Wireless and Mobile Systems (MSWiM '23). Association for Computing Machinery, New York, NY, USA, 175–179. [[paper]](https://doi.org/10.1145/3616388.3617548) [[Dataset]](https://borealisdata.ca/dataset.xhtml?persistentId=doi:10.5683/SP3/R09EWA)
    - 本文提出了一个基于 VeReMi 的数据集，名为 VeReMi for Attack Prediction (VeReMiAP)。由不当行为检测框架 (F2MD) 开发。 VeReMiAP 包含三个关键要素：合作意识消息 (CAM)、一种称为虚假报告攻击的新型攻击，以及对该攻击影响的评估（在本例中表现为道路危险）。
    - 加入了车辆的移动方向（车载传感器类型信息的示例）等信息以及车道索引和当前道路最大减速度（RSU 接收的信息类型的示例）等详细信息，提高了模拟场景的真实性和真实性。
    - [3] 利用 LSTM 模型来识别现实世界驾驶数据集 comma2k19 [8] 中的欺骗攻击。该数据集包含 GPS、CAN 和 IMU 等各种传感器数据，可以预测位置间距离。他们的重点是一种特定的欺骗攻击变体，其中操纵 GNSS 信号来欺骗自动驾驶车辆。

- A. Lochbihler, A. Husseinat, M. Ma, M. Abuibaid, J. S. Huang and B. Zhu, "Misbehaviour Detection of 5G-Connected Vehicles Using Deep Learning," 2023 IEEE 20th International Conference on Mobile Ad Hoc and Smart Systems (MASS), Toronto, ON, Canada, 2023, pp. 646-651, doi: 10.1109/MASS58611.2023.00091. [[paper]](https://ieeexplore.ieee.org/document/10298340) [[code]](https://github.com/Aidanlochbihler/5G-BSM-Threat-Detection)
    - 提出了一种在 5G 网络上运行的 CAV 系统中不当行为检测的新深度学习方法。
    - 为了减少过拟合，创建了一个简单的 CNN，其中包含三个压缩层、一个 ReLU 密集层和一个用于分类的密集 Sigmoid 层。该模型的损失函数为二元交叉熵，以精度为指标。该模型经过 300 个 epoch 的训练，其中 10% 的验证集使用性能指标从最佳 epoch 中挑选模型。训练了更复杂的CNN（如Densenet）;然而，由于数据维度较小，模型很快过拟合。
    - XGBoost 被用作基线模型，与 CNN 进行比较。XGBoost 历来是所有机器学习或非神经网络方法中表现最好的，并具有非常高的推理时间的潜力。
    - LSTM 架构的性能明显优于 Transformer，因为 Transformer 通常需要大量相对复杂的数据才能正确学习其注意力机制。
    - CNN 模型可以使用 16 个给定特征来区分非攻击车辆和攻击车辆，准确率为 72%，精度为 81%。

- Z. Wang and T. Yan, "Federated Learning-based Vehicle Trajectory Prediction against Cyberattacks," 2023 IEEE 29th International Symposium on Local and Metropolitan Area Networks (LANMAN), London, United Kingdom, 2023, pp. 1-6, doi: 10.1109/LANMAN58293.2023.10189424. [[paper]](https://ieeexplore.ieee.org/document/10189424) [[code]](https://github.com/CoderTylor/FL-TP)
    - **FL-TP** 方案：基于 VeReMi 数据集，结合 FL 和 LSTM 提出了一种基于联邦学习的针对网络攻击的车辆轨迹预测算法，检测 VeReMi 中的攻击。

- M. A. Shahid and A. Jaekel, "Hybrid Approach to Detect Position Forgery Attacks in Connected Vehicles," 2023 14th International Conference on Network of the Future (NoF), Izmir, Turkiye, 2023, pp. 47-51, doi: 10.1109/NoF58724.2023.10302810. [[paper]](https://ieeexplore.ieee.org/abstract/document/10302810)
    - **HPFAD** 方案：基于 VeReMi 数据集，将第一种类型的攻击，即恒定偏移攻击的攻击者先划分出来，再使用机器学习的方法（RF、DT、kNN、LR、SVM）检测其他 4 种类型攻击。
    - 实验设置：训练集 : 测试集 = 80% : 20% 。

- A. Sharma and A. Jaekel, "Machine Learning Approach for Detecting Location Spoofing in VANET," 2021 International Conference on Computer Communications and Networks (ICCCN), Athens, Greece, 2021, pp. 1-6, doi: 10.1109/ICCCN52240.2021.9522170. [[paper]](https://ieeexplore.ieee.org/document/9522170)
    - 方案：基于 VeReMi 数据集，使用机器学习的方法（kNN、RF、DT、NB）检测 5 种类型攻击。

- S. Ercan, M. Ayaida and N. Messai, "Misbehavior Detection for Position Falsification Attacks in VANETs Using Machine Learning," in IEEE Access, vol. 10, pp. 1893-1904, 2022, doi: 10.1109/ACCESS.2021.3136706. [[paper]](https://ieeexplore.ieee.org/document/9656118)
    - 基于 VeReMi 数据集，比较了两种不同的机器学习分类方法，即 kNN 和 RF，用于检测使用这些特征的恶意车辆。最后，还进行了集成学习（EL），结合了不同的 ML 方法，在我们的例子中是 kNN 和 RF，以提高检测性能。构建了IDS，允许车辆以分布式方式检测不当行为，同时集中训练检测机制。

- S. Gyawali and Y. Qian, "Misbehavior Detection using Machine Learning in Vehicular Communication Networks," ICC 2019 - 2019 IEEE International Conference on Communications (ICC), Shanghai, China, 2019, pp. 1-6, doi: 10.1109/ICC.2019.8761300. [[paper]](https://ieeexplore.ieee.org/document/8761300)
    - 方案：基于 VeReMi 数据集，使用机器学习的方法（LR、KNN、DT、Bagging、RF）检测 5 种类型攻击。

- S. So, P. Sharma and J. Petit, "Integrating Plausibility Checks and Machine Learning for Misbehavior Detection in VANET," 2018 17th IEEE International Conference on Machine Learning and Applications (ICMLA), Orlando, FL, USA, 2018, pp. 564-571, doi: 10.1109/ICMLA.2018.00091. [[paper]](https://ieeexplore.ieee.org/document/8614116)
    - 方案：基于 VeReMi 数据集，使用机器学习的方法（KNN、SVM）检测 5 种类型攻击。
    - 实验设置：训练集 : 测试集 = 70% : 30% 。

- Rens W van der Heijden. Misbehavior Detection Framework. [[code]](https://github.com/vs-uulm/Maat)
    - 除了数据集中引入的各种攻击者之外，作者还包括使用精确召回曲线评估的四种基本合理性。
    - 在每个场景中，都可以找到大约 500 辆接收车辆的 JSON 文件形式的日志。 每个文件都保存单个车辆（相同 ID）在整个旅程中从相邻车辆（300 米范围）接收到的 BSM 记录。 第一个要求是构建发送者-接收者对，定义单个发送者的完整旅程。 在一个场景中，所有 JSON 文件都被转换为 CSV 格式，然后连接在一起。 名为“攻击者类型”和“接收者 ID”的附加属性已添加到创建的串联 CSV 文件中。

- J. Kamel, M. R. Ansari, J. Petit, A. Kaiser, I. B. Jemaa and P. Urien, "Simulation Framework for Misbehavior Detection in Vehicular Networks," in IEEE Transactions on Vehicular Technology, vol. 69, no. 6, pp. 6631-6643, June 2020, doi: 10.1109/TVT.2020.2984878. [[F2MD-paper]](https://ieeexplore.ieee.org/document/9056489) [[F2MD-code]](https://github.com/josephkamel/F2MD)


## 非机器学习方案
- Q. Hu, X. Fan, A. Shan and Z. Wang, "Sybil Attack Detection Method based on Timestamp-Chain in Internet of Vehicles," 2021 IEEE International Conference on Smart Internet of Things (SmartIoT), Jeju, Korea, Republic of, 2021, pp. 174-178, doi: 10.1109/SmartIoT52359.2021.00035. [[paper]](https://ieeexplore.ieee.org/document/9556187)
    - 时戳链、邻居列表、RSSI。