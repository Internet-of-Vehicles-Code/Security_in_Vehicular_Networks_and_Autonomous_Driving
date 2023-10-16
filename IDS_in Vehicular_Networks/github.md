# survey
 - [Security of vehicular ad-hoc networks: A comprehensive survey](https://www.sciencedirect.com/science/article/pii/S0167404818312872)
 - [A Survey on Machine Learning-Based Misbehavior Detection Systems for 5G and Beyond Vehicular Networks](https://ieeexplore.ieee.org/document/10015746)
 - [A Comprehensive Survey on the Applications of Blockchain for Securing Vehicular Networks](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9738808)

# paper with code
 - [NDNIDS : An Intrusion Detection System for NDNBased VANET](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9129365)------------[github](https://github.com/praveensankar/NDNIDS)
 - [IDS for CAN: A Practical Intrusion Detection System for CAN Bus Security](https://ieeexplore.ieee.org/abstract/document/10001536)-----------[github](https://github.com/brooke-lampe/ids_for_can)
 - [NovelADS: A Novel Anomaly Detection System for Intra-Vehicular Networks](https://ieeexplore.ieee.org/abstract/document/9706416)---------[github](https://github.com/kushagra-2503/)





# In-Vehicle Detection
 - [A Many-Objective Optimization Based Intelligent Intrusion Detection Algorithm for Enhancing Security of Vehicular Networks in 6G](https://ieeexplore.ieee.org/document/9347691) Their Goal: 开源的 CAN 总线消息数据集和篡改攻击场景被用于评估提出的算法对于不同 ID 数据帧的有效性。他们实验结果表明，提出的算法可以有效地提高精度，降低假阳性率.
 - [Anomaly intrusion detection method for vehicular networks based on survival analysis](https://www.sciencedirect.com/science/article/pii/S2214209618301189?via%3Dihub) Their Goal: 识别恶意 CAN 消息，并准确检测车辆网络的正常和异常状态，而无需了解 CAN ID 功能的语义知识。
 - [SAIDuCANT: Specification-Based Automotive Intrusion Detection Using Controller Area Network (CAN) Timing](https://ieeexplore.ieee.org/document/8937816) Their Goal: 现代车辆中嵌入式设备的普及，使得传统的封闭式车辆系统面临通过物理和远程访问车辆网络（如控制器局域网（CAN））的网络安全攻击风险。CAN 总线没有实现能够保护车辆免受日益增加的网络安全和物理攻击的安全协议。为解决这一风险，用于提取 CAN 总线的实时模型参数，并开发了 SAIDuCANT，一种基于规格的入侵检测系统（IDS），使用基于异常的监督学习算法，以实时模型作为输入.
 - [Collaborative Intrusion Detection for VANETs: A Deep Learning-Based Distributed SDN Approach](https://ieeexplore.ieee.org/document/9216536) Their Goal: 现有的IDS解决方案仅限于检测局部子网下的异常网络行为，而不是整个VANET。为了解决这个问题，我们利用深度学习与生成式对抗网络，并探索分布式SDN设计了一个协同入侵检测系统 (CIDS) 的无线自组网，它使多个SDN控制器共同训练个全局入侵检测模型，为整个网络，而不直接交换他们的子网流量。 


# Vehicle-Vehicle Detection
 - [ECF-MRS: An Efficient and Collaborative Framework With Markov-Based Reputation Scheme for IDSs in Vehicular Networks](https://ieeexplore.ieee.org/document/9153014) Their Goal: VANETs 的快速移动和高度动态的特性，很难采用已经在有线网络中得到适当使用的相同 IDS。因此，在本文中，提出了一种高效协作的框架，基于 Markov 的信誉方案，即 ECF-MRS。在该提出的框架中，协作机制是通过使用非支配排序遗传算法-III（NSGA-III）协作来合并 VANETs 中 IDS 的优势，以生成更优越的 IDS，而非线性规划（NLP）优化则被设计为高效的机制，以减少 VANETs 中 IDS 的执行时间。此外，考虑到协作的安全风险，提出了一种基于隐藏广义混合转移分布（HgMTD）模型的信誉方案，即 RS-HgMTD，用于评估 VANETs 中每个车辆邻居的信用价值。
 - [SP-CIDS: Secure and Private Collaborative IDS for VANETs](https://ieeexplore.ieee.org/document/9269477) Their Goal: 一个安全和私人协作的入侵检测系统(SP-CIDS) 提出检测网络攻击，以减轻安全问题.该系统提高了IDS的存储效率、准确性和可扩展性。 然而，有显着的数据隐私问题可能在这种合作中，一个CIDS可以作为一个恶意的系统，可以访问的中间阶段的学习过程。此外，SP-CIDS系统使用差分隐私(DP) 技术来解决与基于DML的CIDS相关联的上述数据隐私风险
 - [Hybrid fuzzy multi-criteria decision making based multi cluster head dolphin swarm optimized IDS for VANET](https://www.sciencedirect.com/science/article/pii/S2214209617301080?via%3Dihub) Their Goal: 研究集群通信，为了减轻单个集群头子的负担，提出了多集群头方案，其中集群中的多个节点可以作为集群头子来分担单个集群头子的负载。为了选择稳定的集群头子，提出了混合模糊多准则决策（HF-MCDM）方法，其中模糊层次分析过程（AHP）和 TOPSIS 方法结合在一起进行最优决策。
 - [GaDQN-IDS: A Novel Self-Adaptive IDS for VANETs Based on Bayesian Game Theory and Deep Reinforcement Learning](https://ieeexplore.ieee.org/document/9573515) Their Goal: 关于在 VANETs 中部署 IDSs的研究主要关注于有效性和效率之间的权衡，但在可变网络中权衡的适应性方面所做的努力很少。因此，我们解决了两个关键问题：1）IDS 如何从其角度感知环境变化？2）如何在不同场景下使 IDS 具有适应性？
 - [A novel Intrusion Detection System for Vehicular Ad Hoc Networks (VANETs) based on differences of traffic flow and position](https://www.sciencedirect.com/science/article/pii/S1568494618306835?via%3Dihub) Their Goal: IDS 的性能仍需改进，以适应 VANETs 这种快速移动、高度动态的场景.
 - [Trust aware support vector machine intrusion detection and prevention system in vehicular ad hoc networks](https://www.sciencedirect.com/science/article/pii/S0167404818307569?via%3Dihub) Their Goal: 主动网络攻击通常旨在减少或中断网络的可用性。他们提出了一种完整的基于共享信任值的 VANET IDS，该信任值由修改后的杂项模式数据收集和支持向量机（SVM）数据分析组合而成，以建立每个网络车辆的信任感知 SVM-based IDS（TSIDS）这种方法确保了源车辆或节点以及任何中间网络节点都了解其下一个跃点的活动，并在恶意行为或故障情况下，它们会相应地做出反应，以尽可能保持网络性能。
 - [An Efficient Conditional Privacy-Preserving Authentication Scheme for Vehicular Sensor Networks Without Pairings](https://ieeexplore.ieee.org/document/7369988) Their Goal: 为了支持 VSN 中车辆的安全通信和驾驶员隐私，我们开发了一种基于椭圆曲线密码系统（ECC）的新型基于身份（ID-based）签名，并将其采用为提出一种新颖的条件隐私保护身份验证方案。

# Dataset
1. [VeReMi](https://github.com/VeReMi-dataset/VeReMi/releases)
   - **是使用omnet++和vein等模拟工具生成的模拟数据集。实现了五种类型的位置证伪:**
    1. 常量:包括广播固定位置;
    2. 固定偏移量:广播在实际位置上加上固定偏移量;
    3. 随机:包括广播属于模拟地区的随机位置;
    4. 随机偏移:包括广播属于车辆周围矩形的随机位置;
    5. 最终停止:攻击者在一段时间内表现正常，然后在一段时间内通过广播固定位置进行攻击。该数据集是针对不同的流量密度和不同的攻击者无线电生成的。
2. [VeReMi extension](https://github.com/josephkamel/VeReMi-Dataset)
   - **VeReMi扩展也是使用Framework For Misbehavior Detection生成的模拟数据集，该数据集基于omnet++和vein。该数据集代表了VeReMi的扩展，实现了九种类型的攻击:**
   1. 位置伪造(恒定、随机、恒定偏移和随机偏移);
   2. 速度故障(恒定、随机、恒定偏移、随机偏移);
   3. 延迟消息;
   4. DoS攻击;
   5. DoS随机;
   6. 数据回放;
   7. 破坏性;
   8. 最终停止;
   9. 交通拥堵西比尔。
3. [DARPA](https://www.ll.mit.edu/r-d/datasets/1999-darpa-intrusion-detection-evaluation-dataset)
   - **是使用麻省理工学院林肯实验室模拟网络环境创建的流行入侵检测数据集**
    1. 扫描攻击
    2. U2R (User-to-Root)攻击、
    3. R2L (Remote-to-Local)攻击
    4. 可用性的攻击，如DoS攻击
4. [CAIDA DDos2007](https://www.caida.org/catalog/datasets/ddos-20070804_dataset/)
   - **包括来自DDoS攻击(UDP泛洪)的大约一个小时的流量跟踪，该攻击试图通过消耗服务器上的计算资源和连接服务器到Internet的所有网络带宽来阻止对服务器的访问。跟踪信息只包括攻击流量流向受害者和受害者对攻击的响应**
5. [AWID 2](https://icsdweb.aegean.gr/awid/awid2)
   - **数据集实现了基于小型测试平台生成的802.11流行攻击。它包括对身份验证(例如，ARP注入)，可用性(例如，请求发送(RTS)信标)和机密性(例如，流氓接入点)的各种攻击。AWID数据集包含在不同时间、不同设备和不同环境中捕获的不同大小的数据包。每个跟踪包括154个特征和一个指示跟踪是良性的还是攻击的标签**
6. [KDD CUP 99](https://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html)
   - **是在国际竞争中提出的一种流行的入侵检测数据集，旨在建立一种能够区分正常和恶意网络流量的预测模型。KDD CUP 99包括23种针对身份验证和可用性的攻击，例如在军事网络环境中模拟的R2L、探测攻击、DoS和U2R**
7. [NSL-KDD](https://www.unb.ca/cic/datasets/nsl.html)
   - **数据集包含与KDD CUP 99相同的攻击。它主要是通过删除重复和创建更复杂的子数据集来增强KDD CUP 99。具体来说，与KDD CUP 99不同，NSL-KDD不包括训练和测试数据集中的冗余痕迹，这有助于消除对更频繁记录的偏见**
8. [Kyoto](http://www.takakura.com/Kyoto_data/BenchmarkData-Description-v5.pdf)
   - **是一个蜜罐数据集，其中包含转换为称为会话的新格式的真实基于数据包的流量。每个会话包含24个特征，其中14个特征受到KDD CUP 99数据集的启发。其余10个是基于流的特性，如IP地址、端口、持续时间等**
9.  [UNSW-NB15](http://www.takakura.com/Kyoto_data/)
    - **是在一个小型模拟环境中用了31个小时创造出来的。数据集包括原始网络数据包。训练数据集中的记录数为175,341条，测试数据集中的记录数为82,332条，来自不同类型(正常和攻击)。具体来说，它包括九种攻击，如后门、DoS、漏洞利用、模糊攻击或蠕虫**
10. [CICIDS2017](https://www.unb.ca/cic/datasets/ids-2017.html)
    - **已经在模拟环境中创建了五天。它以真实的交通背景生成，抽象人类交互行为，生成自然的良性背景交通。它包含广泛的攻击类型，如SSH暴力破解、botnet、botnet、DoS、DDoS、Web和渗透攻击**
11. [CRAWDAD (mobiclique)](https://crawdad.org/thlab/sigcomm2009/20120715)
    - **包括蓝牙接触的痕迹，机会主义信息，以及在SIGCOMM 2009上使用MobiClique应用程序的76名用户的社会概况。具体来说，每个设备定期执行蓝牙发现以发现附近的设备，并记录发现结果和所有数据通信。此外，这些设备还记录了用户的社会概况、演变和应用程序级消息传递的详细信息**
12. [NGSIM trajectory datasets](https://ops.fhwa.dot.gov/trafficanalysistools/ngsim.htm)
    - **NGSIM计划在2005年至2006年期间收集了美国四个不同地点的高质量交通数据集，包括两个高速公路段和两个主干道段。为每个位置收集和生成的数据集包括特定区域所有车辆的纵向和横向定位信息**