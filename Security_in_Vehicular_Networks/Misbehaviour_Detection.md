总结了一些车联网中不当行为检测相关文献。

## 综述
- S. Dong, H. Su, Y. Xia, F. Zhu, X. Hu and B. Wang, "A Comprehensive Survey on Authentication and Attack Detection Schemes That Threaten It in Vehicular Ad-Hoc Networks," in IEEE Transactions on Intelligent Transportation Systems, doi: 10.1109/TITS.2023.3297527. [[paper]](https://ieeexplore.ieee.org/abstract/document/10201386)
  - 现有的Sybil攻击检测方案可以大致分为五类：基于身份验证、基于位置验证、基于轨迹验证、基于资源测试（工作负载证明）和基于邻居列表。
- A. Boualouache and T. Engel, "A Survey on Machine Learning-Based Misbehavior Detection Systems for 5G and Beyond Vehicular Networks," in IEEE Communications Surveys & Tutorials, vol. 25, no. 2, pp. 1128-1172, Secondquarter 2023, doi: 10.1109/COMST.2023.3236448. [[paper]](https://ieeexplore.ieee.org/document/10015746) 



## 机器学习方案
- K. A. Bonfim, F. D. S. Dutra, C. E. T. Siqueira, R. I. Meneguette, A. L. Dos Santos and L. A. P. Júnior, "Federated Learning-based Architecture for Detecting Position Spoofing in Basic Safety Messages," 2023 IEEE 97th Vehicular Technology Conference (VTC2023-Spring), Florence, Italy, 2023, pp. 1-5, doi: 10.1109/VTC2023-Spring57618.2023.10199980. [[paper]](https://ieeexplore.ieee.org/document/10199980) [[code]](https://github.com/c2dc/fl-ieee-vtc2023/tree/master) [[Dataset]](https://mega.nz/folder/5Bp2QCSY#TxAiyrJOmt9itJ12K6Lxlw)
    - 最小工作节点数量：2。

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
- A. Paranjothi and M. S. Khan, "Enhancing Security in VANETs with Sybil Attack Detection using Fog Computing," 2023 IEEE 98th Vehicular Technology Conference (VTC2023-Fall), Hong Kong, Hong Kong, 2023, pp. 1-6, doi: 10.1109/VTC2023-Fall60731.2023.10333491. [[paper]](https://ieeexplore.ieee.org/document/10333491)
    - 提出了一种基于雾计算的VANET女巫攻击检测（FSDV），它利用该地区所有车辆的车载单元（OBU）来创建动态雾，使用统计技术进行流氓节点检测。我们的目标是减少数据处理延迟、开销和 FPR，以检测在高车辆密度下导致女巫攻击的流氓节点。我们的框架的性能是通过使用OMNET++和SUMO模拟器进行模拟来实现的。
    - 保护节点利用所有车辆的 OBU 动态创建雾，以检测该区域广播较低速度值的流氓节点。部署雾层后，守卫节点开始将相邻车辆添加到邻居列表中，这是第一次遇到的情况。否则，它会更新相邻车辆的时间戳。当信标消息在区域中广播时（即每 100 毫秒），邻居列表会持续更新。然后，通过对比和分析信标消息中广播的速度值来实现对恶意节点的检测。如果速度差大于动态阈值，则检测到女巫攻击。
    - Greenshields 模型认为道路的最佳密度为固定值，与道路限速无关。
    - **缺点**：纯靠V2V通信，如果Sybil车辆速度与动态雾车辆速度相当，检测效果将会很差，加入精度高的定位传感器，可以解决这一问题。

- M. S. Ali and P. Merdrignac, "Distributed Misbehavior Detection based on Vehicle Perception Model and CPM Data Collection," 2023 IEEE 98th Vehicular Technology Conference (VTC2023-Fall), Hong Kong, Hong Kong, 2023, pp. 1-5, doi: 10.1109/VTC2023-Fall60731.2023.10333637. [[paper]](https://ieeexplore.ieee.org/document/10333637)
    - 本文介绍了一种创新的不当行为检测（MBD）算法，该算法旨在使用集体感知消息（CPM）识别协作智能交通系统（C-ITS）中的错误**突然停车**信息。该算法集成了车辆感知模型和来自相邻车辆的 CPM 数据。通过使用 Omnet++、SUMO 和 Veins 进行的综合模拟，我们探索了该算法在各种感知范围内的性能。
    - 基于感知和分布式算法的开发：我们设计了两种 MBD 算法，LCPMBDA 和 LP-MBDA，它们利用感知模型来验证接收到 CPM 中的信息。这些算法以分布式方式运行，因为所有车辆都使用相同的感知模型，从而能够对 CPM 信息进行分布式验证。
    - 性能评估：通过在真实场景中的大量模拟，对所提出的算法进行了严格的评估。通过专注于以数据为中心的方法并利用本地和接收到的信息，我们的算法展示了抵御不断变化的威胁和攻击的鲁棒性。仿真使用SUMO实现道路网络和感知模型，使用Veins进行V2X通信，使用OmNet进行整体仿真。

- Q. Hu, X. Fan, A. Shan and Z. Wang, "Sybil Attack Detection Method based on Timestamp-Chain in Internet of Vehicles," 2021 IEEE International Conference on Smart Internet of Things (SmartIoT), Jeju, Korea, Republic of, 2021, pp. 174-178, doi: 10.1109/SmartIoT52359.2021.00035. [[paper]](https://ieeexplore.ieee.org/document/9556187)
    - 时戳链、邻居列表、RSSI。

## 2023.12.27
- L. N. Balico, A. A. F. Loureiro, E. F. Nakamura, R. S. Barreto, R. W. Pazzi and H. A. B. F. Oliveira, "Localization Prediction in Vehicular Ad Hoc Networks," in IEEE Communications Surveys & Tutorials, vol. 20, no. 4, pp. 2784-2803, Fourthquarter 2018, doi: 10.1109/COMST.2018.2841901. [[paper]](https://ieeexplore.ieee.org/document/8368199)
    - 车载自组网定位预测
- A. Balaram and S. Pushpa, “Sybil attack resistant location privacy in VANET,” Int. J. Inf. Commun. Technol., vol. 13, no. 4, pp. 389–406, 2018. [[paper]](https://dl.acm.org/doi/abs/10.5555/3292823.3292824)

- K. Rabieh, M. M. E. A. Mahmoud, T. N. Guo, and M. Younis, “Cross-layer scheme for detecting large-scale colluding Sybil attack in VANETs,” in Proc. IEEE Int. Conf. Commun. (ICC), Jun. 2015, pp. 7298–7303. [[paper]](https://ieeexplore.ieee.org/abstract/document/7249492)
    - **提出了一种跨层方案，使RSU能够识别这种女巫车辆。**。当可疑车辆经过RSU时，RSU询问位置坐标和当前速度。然后，RSU 计算车辆的下一个位置 A，并使用定向天线向该方向发送查询消息。该车辆应在地点A回复查询消息。否则，RSU怀疑该车辆不在所声称的地点，并确定其可能是Sybil车辆，并将报告给TA进行进一步调查。
- M. Baza et al., “Detecting Sybil attacks using proofs of work and location in VANETs,” IEEE Trans. Dependable Secure Comput., vol. 19, no. 1, pp. 39–53, Jan. 2022. [[paper]](https://ieeexplore.ieee.org/document/9091099)
    - 提出了一种使用工作和位置证明的女巫攻击检测方案。这个想法是，每个路边单元 （RSU） 都会发出一个带有签名的时间戳标签，作为车辆匿名位置的证明。**从多个连续的 RSU 发送的证明用于创建用作车辆匿名身份的轨迹。** 此外，一个 RSU 的贡献不足以创建轨迹，而是需要多个 RSU 的贡献。通过这种方式，攻击者需要破坏不可行的 RSU 数量来创建虚假轨迹。此外，在收到来自 RSU 的位置证明后，车辆应通过运行工作量证明 （PoW） 算法来解决计算难题。