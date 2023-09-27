# Survey
1. T. Alladi, V. Chamola, N. Sahu, V. Venkatesh, A. Goyal and M. Guizani, "A Comprehensive Survey on the Applications of Blockchain for Securing Vehicular Networks," in IEEE Communications Surveys & Tutorials, vol. 24, no. 2, pp. 1212-1239, Secondquarter 2022, doi: 10.1109/COMST.2022.3160925. [[paper]](https://ieeexplore.ieee.org/document/9738808) 
    - 区块链在车载网络中的应用综述
    - 
2. X. Wang, H. Zhu, Z. Ning, L. Guo and Y. Zhang, "Blockchain Intelligence for Internet of Vehicles: Challenges and Solutions," in IEEE Communications Surveys & Tutorials, doi: 10.1109/COMST.2023.3305312. [[paper]](https://ieeexplore.ieee.org/document/10217209)


## Authentication
### 陕西大学计算机科学学院**周彦伟**副教授团队，主要研究方向：密码学、信息安全。[[Home Page]](https://ccs.snnu.edu.cn/info/1017/8712.htm)
[1] Z. Wang et al., "An Anonymous and Revocable Authentication Protocol for Vehicle-to-Vehicle Communications," in IEEE Internet of Things Journal, vol. 10, no. 6, pp. 5114-5127, 15 March15, 2023, doi: 10.1109/JIOT.2022.3222469. [[paper]](https://ieeexplore.ieee.org/document/9953072)
- 该文提出一种基于无证书的车对车通信匿名可撤销认证协议，将身份验证过程与流量消息验证分开，避免了频繁的身份撤销列表（IRL）检查的缺点，减少了通信和消息身份验证的开销。

[2] Y. Xu et al., "An Efficient Identity Authentication Scheme With Provable Security and Anonymity for Mobile Edge Computing," in IEEE Systems Journal, vol. 17, no. 1, pp. 1012-1023, March 2023, doi: 10.1109/JSYST.2022.3185258. [[paper]](https://ieeexplore.ieee.org/document/9820763)
- 本文为MEC创建了一个具有可证明安全性和匿名性的高效身份认证协议，保证了用户在通信过程中保持匿名，并且基于随机预言机模型中的经典复杂性假设可以严格证明其安全性。

[3] Z. Qiao, Y. Zhou, B. Yang, M. Zhang, T. Wang and Z. Xia, "Secure and Efficient Certificate-Based Proxy Signature Schemes for Industrial Internet of Things," in IEEE Systems Journal, vol. 16, no. 3, pp. 4719-4730, Sept. 2022, doi: 10.1109/JSYST.2021.3131589. [[paper]](https://ieeexplore.ieee.org/document/9652559)
- 本文中为了进一步解决之前CBPS方案提案中的一些安全问题和设计缺陷，引入了三种具有更高安全性的CBPS方案新结构。在前两个提案中，委派有效性可以由指定的验证者（代理签名者）验证，最后一个构造的签名授权是可公开验证的（任何签名者）。此外，基于离散对数问题在随机预言机中使用分叉引理给出形式化安全证明。文中还讨论了构建安全CBPS方案的两个必要条件，以避免未来研究中的安全漏洞。

### 其他
[4] M. A. Shawky, M. Bottarelli, G. Epiphaniou and P. Karadimas, "An Efficient Cross-Layer Authentication Scheme for Secure Communication in Vehicular Ad-Hoc Networks," in IEEE Transactions on Vehicular Technology, vol. 72, no. 7, pp. 8738-8754, July 2023, doi: 10.1109/TVT.2023.3244077. [[paper]](https://ieeexplore.ieee.org/document/10041975)
- 该文提出一种车载通信的跨层认证方案，结合无线信道的短期互易特性对相应终端进行重新认证，降低了整体复杂度以及计算和通信开销。

[5] P. Zhao, Y. Huang, J. Gao, L. Xing, H. Wu and H. Ma, "Federated Learning-Based Collaborative Authentication Protocol for Shared Data in Social IoV," in IEEE Sensors Journal, vol. 22, no. 7, pp. 7385-7398, 1 April1, 2022, doi: 10.1109/JSEN.2022.3153338. [[paper]](https://ieeexplore.ieee.org/document/9718264)
- 为了有效防止数据泄露，降低数据的传播延迟，本文设计了一种针对共享数据的联邦学习协同认证协议。车辆客户端模型的参数由联邦学习中的协议加密。协议的载体和其他实体实现了高效的匿名相互认证和密钥协议。所提协议的安全性在随机预测机模型中得到了证明。在SUMO和OMNeT++平台上的仿真结果表明，与其他协议相比，认证延迟最低，丢包率降低至4.68%。此外，有效解决了全局聚合模型的过拟合问题。

[6] S. Bojjagani, Y. C. A. P. Reddy, T. Anuradha, P. V. V. Rao, B. R. Reddy and M. K. Khan, "Secure Authentication and Key Management Protocol for Deployment of Internet of Vehicles (IoV) Concerning Intelligent Transport Systems," in IEEE Transactions on Intelligent Transportation Systems, vol. 23, no. 12, pp. 24698-24713, Dec. 2022, doi: 10.1109/TITS.2022.3207593.
- 设计了一个名为AKAP-IoV的新系统，该系统支持车辆，路边单元以及雾和云服务器之间的安全通信，相互身份验证和密钥管理。
- AKAP-IoV使用Scyther和Tamarin进行了测试和验证，以确保其对网络威胁的抵抗力。
- 使用实数或随机（RoR）预言机模型进行了正式的安全分析，以逻辑地评估安全属性。

[7] X. Liu, W. Chen, Y. Xia and R. Shen, "TRAMS: A Secure Vehicular Crowdsensing Scheme Based on Multi-Authority Attribute-Based Signature," in IEEE Transactions on Intelligent Transportation Systems, vol. 23, no. 8, pp. 12790-12800, Aug. 2022, doi: 10.1109/TITS.2021.3117400. [[paper]](https://ieeexplore.ieee.org/document/9568772)
- 提出了一种用于车辆群感知的消息认证方案，该方案允许发布者灵活地定制潜在参与者必须满足的细粒度策略，并使用基于属性的签名来验证消息。这可以有效提高车辆群感中的感知精度。
- 提出一种基于属性签名的感知车辆隐私保护机制，将感知车辆的唯一标识混淆为一组属性，实现感知车辆的匿名认证。
- 提出了一种多权限密钥管理架构来实现高效感知，其中每个属性权限管理车辆属性的密钥。它可以在动态车联网中更安全、更高效地为车辆生成属性密钥。

[8] Y. Zhou, Z. Wang, Z. Qiao, B. Yang and M. Zhang, "An Efficient and Provably Secure Identity Authentication Scheme for VANET," in IEEE Internet of Things Journal, vol. 10, no. 19, pp. 17170-17183, 1 Oct.1, 2023, doi: 10.1109/JIOT.2023.3273234. [[paper]](https://ieeexplore.ieee.org/document/10121784)
- 提出了一个改进的VANET的CLAS方案，以解决目前基于无证书聚合签名（CLAS）的VANET身份验证方案在其安全模型下都不能抵抗公钥替换攻击的问题。
- 简要回顾了Thumbur等人[10]和Chen和Chen[11]的CLAS方案，并表明两者都不能抵抗公钥替换攻击。
- 提出的CLAS方案重构了现有的CLAS方案，完全基于ECC，比使用双线性配对的方案更有效，更安全。与基于ECC的方案相比，所提方案在验证效率和通信开销方面具有优势。
- 本文引入通用分叉引理来改进无证书签名（CLS）方案的安全证明，为CLAS方案的安全证明提供新思路。
   
[9] S. Zhang, R. He, Y. Xiao and Y. Liu, "A Three-Factor Based Trust Model for Anonymous Bacon Message in VANETs," in IEEE Transactions on Vehicular Technology, vol. 72, no. 9, pp. 11304-11317, Sept. 2023, doi:10.1109/TVT.2023.3270333. [[paper]](https://ieeexplore.ieee.org/document/10108063)
- 基于期望、风险和置信3个信任因素，构建基于三因素的数据中心信任模型，评估条件隐私保护认证协议下匿名信标消息的可信度。由于该模型不需要周围车辆之间的交互，因此该模型具有很高的效率。
- 基于三个因素构建信托决策。匿名信标消息的决策是根据信任域做出的， 信任域是基于信任与三个因素之间的定性关系构建的.与现有信任决策中使用的信任阈值相比，信任域能够很好地反映信任与这三个因素之间的关系。
- 使用Veins 5.1进行了模拟，这是一个开源框架，用于运行基于OMNeT++和SUMO的车辆网络模拟。为了验证所提模型的通用性，我们在双向直线道路和两个交叉路口的十字路口两种常见场景中进行了仿真，如图所示。5.为了获得道路的预测速度，在场景中的每条道路上设置了传感器。在直线道路上，传感器之间的间隔为 300 米。此外，由于情况复杂，我们在十字路口周围设置了8个传感器。最接近信标消息中位置信息的传感器计算的平均速度将被视为预测速度.我们将传感器设置为每 5 秒计算一次平均速度。

[10] M. Luo and Y. Zhou, "An Efficient Conditional Privacy-Preserving Authentication Protocol Based on Generalized Ring Signcryption for VANETs," in IEEE Transactions on Vehicular Technology, vol. 71, no. 9, pp. 10001-10015, Sept. 2022, doi: 10.1109/TVT.2022.3179371. [[paper]](https://ieeexplore.ieee.org/document/9786717)
- 多数CPPA方案允许可信机构（TA）暴露恶意邮件的发件人，但它们很难证明跟踪结果的真实性。因此，我们提出了一种新的CPPA协议来解决这些问题。在我们的协议中，引入广义环签密码，在一个算法中提供环签名模式和环签密码模式，以满足复杂应用场景下不同的安全需求。设计了方便的公共验证算法，使跟踪结果可证明且更可信。此外，我们证明我们的协议实现了机密性、不可伪造性和已知会话特定的临时信息安全 （KSSTIS）。
- 先前RSU与当前RSU通信，确认身份。
- 使用 JPBC 库 [48] 来计算加密操作的执行时间。

[11] M. W. Akram et al., "A Secure and Lightweight Drones-Access Protocol for Smart City Surveillance," in IEEE Transactions on Intelligent Transportation Systems, vol. 23, no. 10, pp. 19634-19643, Oct. 2022, doi: 10.1109/TITS.2021.3129913. [[paper]](https://ieeexplore.ieee.org/document/9646496)
- 为无人机辅助的VANET设计了一个基于DLA的密钥交换协议。该协议扩展了可扩展性，并使用安全的按位异或运算、单向散列函数，包括用户和无人机相互认证时的用户生物特征验证。所提出的协议可以抵御许多众所周知的安全攻击，并在随机预言机模型（ROM）下提供正式和非正式的安全性。

[12] Y. Zhao, Y. Wang, P. Wang and H. Yu, "PBTM: A Privacy-Preserving Announcement Protocol With Blockchain-Based Trust Management for IoV," in IEEE Systems Journal, vol. 16, no. 2, pp. 3422-3432, June 2022, doi: 10.1109/JSYST.2021.3078797. [[paper]](https://ieeexplore.ieee.org/document/9442949)
- PBC库
- 该文利用基于身份的群组签名，提出了一种新型的隐私保护公告协议，保证了隐私保护和转发公告的效率。
- 设计了一个基于区块链的TM（BBTM）系统，其中RSU采用加权和方法来评估车辆的声誉。此外，在PBTM中使用混合PoW和改进的PBFT共识机制来提高验证效率。

[13] P. Vijayakumar, M. Azees, S. A. Kozlov and J. J. P. C. Rodrigues, "An Anonymous Batch Authentication and Key Exchange Protocols for 6G Enabled VANETs," in IEEE Transactions on Intelligent Transportation Systems, vol. 23, no. 2, pp. 1630-1638, Feb. 2022, doi: 10.1109/TITS.2021.3099488. [[paper]](https://ieeexplore.ieee.org/document/9507051)
- 1）提出一种匿名相互认证，V2V通信的计算开销低 2）提出一种高效的批量认证协议，以显著降低RSU端的总认证开销 3）提出一种完整性保存协议，将基于位置的消息从RSU广播到VANET车辆，而无需在覆盖传输过程中进行任何修改RSU 的区域。

[14] H. Sikarwar and D. Das, "A Novel MAC-Based Authentication Scheme (NoMAS) for Internet of Vehicles (IoV)," in IEEE Transactions on Intelligent Transportation Systems, vol. 24, no. 5, pp. 4904-4916, May 2023, doi: 10.1109/TITS.2023.3242291. [[paper]](https://ieeexplore.ieee.org/document/10042068)
- NoMAS 仅使用五个哈希函数和每条消息的 XoR 操作对车联网通信执行有效的身份验证。此外，NoMAS 需要 20 字节用于两个 MAC 函数和 4 字节用于时间戳，因此总通信开销为 44 字节。
- 在安全分析部分，使用BAN逻辑，我们在理论上证明了NoMAS满足所有安全需求。我们还使用 ProVerif 工具和 Pi 演算的概念提供了基于软件的形式化安全证明结果。

## 区块链
- 数据共享
- 数据与资源交易
- 车辆管理

## Privacy protection

## 入侵检测
