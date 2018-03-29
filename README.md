# 汉升链商 — Hub Intelligent Things

#### 基于区块链的物联网商业平台
##### 核心：设备数字化 + 资产证券化 = 价值流通
##### 应用：设备投资（加盟 + 共享 + 转让） + 金融服务 + 区块链 = 收益保证
##### 主链：汉升链，全新链结构和共识机制，最贴近真实应用的主链

# 产品和技术白皮书
info@hansheng.io
2018.03 (v 1.0)

**目录**
=================
- [1. 项目概述](#1-项目概述)
- [2. 行业背景](#2-行业背景)
  - [2.1. 共享经济](#21-共享经济)
  - [2.2. 物联网 — 万物互联](#22-物联网--万物互联)
  - [2.3. 区块链和智能合约](#23-区块链和智能合约)
  - [2.4. 物联网 + 区块链](#24-物联网--区块链)
- [3. 新兴市场：物联网投资和数据交易](#3-新兴市场物联网投资和数据交易)
  - [3.1. 物联网设备的价值和分类](#31-物联网设备的价值和分类)
  - [3.2. 投资物联网设备遇到的问题](#32-投资物联网设备遇到的问题)
  - [3.3. 汉升解决物联网投资难题](#33-汉升解决物联网投资难题)
- [4. 汉升链商](#4-汉升链商)
  - [4.1. 合作加盟](#41-合作加盟)
  - [4.2. 出售长期收益](#42-出售长期收益)
  - [4.3. 共享设备能力和使用时间](#43-共享设备能力和使用时间)
  - [4.4. 共享生产能力和管理能力](#44-共享生产能力和管理能力)
  - [4.5. 金融服务（依靠交易流水和信誉评估）](#45-金融服务依靠交易流水和信誉评估)
  - [4.6. 其它应用场景](#46-其它应用场景)
- [5. 汉升链技术架构简介](#5-汉升链技术架构简介)
  - [5.1. 区块链 vs. 汉升链](#51-区块链-vs-汉升链)
  - [5.2. 设计目标](#52-设计目标)
  - [5.3. 设计原则](#53-设计原则)
  - [5.4. 技术框架名词解释](#54-技术框架名词解释)
    - [5.4.1. 地址链（Address Chain）](#541-地址链address-chain)
    - [5.4.2. 间接地址（RA, Reference Address）](#542-间接地址ra-reference-address)
    - [5.4.3. 地址之间的层级关联](#543-地址之间的层级关联)
    - [5.4.4. NAC — 由交易和多链构成的有向无环图](#544-nac--由交易和多链构成的有向无环图)
    - [5.4.5. GPoS — 权益证明担保](#545-gpos--权益证明担保)
    - [5.4.6. 见证节点 — 交易打包 + 金融服务 + 身份服务](#546-见证节点--交易打包--金融服务--身份服务)
  - [5.5. 链外系统](#55-链外系统)
    - [5.5.1. 链外系统](#551-链外系统)
    - [5.5.2. 存储节点：IPFS](#552-存储节点ipfs)
    - [5.5.3. 计算节点与云服务](#553-计算节点与云服务)
    - [5.5.4. 中继节点](#554-中继节点)
  - [5.6. 目录存储（Directory Service）](#56-目录存储directory-service)
  - [5.7. 交易及非交易消息类型](#57-交易及非交易消息类型)
    - [5.7.1. 交易（Transaction）](#571-交易transaction)
    - [5.7.2. 声明（Announcement）](#572-声明announcement)
    - [5.7.3. 通知（Notification）](#573-通知notification)
- [6. 技术先进性](#6-技术先进性)
  - [6.1. 无手续费 + 高并发交易](#61-无手续费--高并发交易)
  - [6.2. 可局部运行 + 无双花，无分叉](#62-可局部运行--无双花无分叉)
  - [6.3. 增强账号匿名性](#63-增强账号匿名性)
  - [6.4. 可锁定账号，恢复密钥](#64-可锁定账号恢复密钥)
  - [6.5. 链结构直接支持所有权关系](#65-链结构直接支持所有权关系)
  - [6.6. 所有权和使用权分离](#66-所有权和使用权分离)
  - [6.7. 有效信誉评价机制](#67-有效信誉评价机制)
- [7. 愿景和发展规划](#7-愿景和发展规划)
  - [7.1. 团队愿景](#71-团队愿景)
  - [7.2 执行计划](#72-执行计划)
  - [7.3. 推广策略](#73-推广策略)
  - [7.4. 社区建设](#74-社区建设)
- [8. 汉升币](#8-汉升币)
  - [8.1. 汉升币（主链）](#81-汉升币主链)
  - [8.2. 汉升代币（以太坊）](#82-汉升代币以太坊)
  - [8.3. 流通价值](#83-流通价值)
- [9. 团队介绍](#9-团队介绍)
  - [9.1. 创始团队](#91-创始团队)
  - [9.2. 顾问团队（按加入时间排名）](#92-顾问团队按加入时间排名)
- [10. 免责声明](#10-免责声明)
- [11. 参考资料](#11-参考资料)

## 1. 项目概述
**汉升链商** 是基于区块链的开源去中心化物联网设备投资和价值共享平台。用户可以在汉升链商上投资、共享和处置物联网资产，并享受完善的金融服务。

汉升链商为物联网设备投资、设备共享、设备转让以及数据交易提供完善的应用功能和金融服务；汉升链商让投资者快速获取资金来购买设备，共享设备的使用价值，或将手中设备的收益权抵押融资，加速资金流转速度。

汉升链商的底层技术平台是汉升链（区块链）。汉升链商将设备运营数据（流量、收益、使用率等）数据写入汉升链，利用汉升链上数据不可篡改的特性，这些数据能直接反映设备的资产价值，并作为设备定价和投资保险等金融服务的可靠依据。通过汉升链上的身份验证服务、设备所有权管理、信誉评价体系，以及完善的支付服务，能大大降低参与者选择投资对象和投资方式的进入难度，从根本上改变传统的“加盟”和“共享”模式。

以Mini KTV为例：如果商家选择使用加盟方式，通常只能根据设备成本确定加盟价格，无法根据Mini KTV的不同铺设位置做差异化定价。对于加盟者而言，一方面很难判断加盟价格的合理性，另一方面，在转让设备的时候也很难让接收方信任自己的定价。但如果将Mini KTV的所有运营数据（用户缴费数据）都存入汉升链，从金融角度来说，一个被放置的Mini KTV设备就是一个可以根据运营数据评估其价值的资产，商家可以很容易对其定价，加盟者则很容易评估其价值。汉升链商基于运营数据撮合交易，并作为交易中介，使用智能合约确保设备所有权和收益权的转移。

无论是拥有数百个停车场的大型商业公司，或是在某个商场安置儿童木马的小规模个人投资者，还是共同出资在 CBD 投资无人超市的联合投资人，都能使用汉升的电商和金融服务，获得短期和长期的投资回报。

虽然汉升链商是中心化的服务，但用户的所有财务信息和交易记录都保存在去中心化的汉升链上，由汉升链上不可篡改的分布式账本保证用户的资产安全。

"**汉升链**"是全球范围内的物联网安全通信和交易系统；汉升链将区块链拉进日常生活所需要的真实应用场景，为衣食住行、协同协作、生产制造提供更便利、更安全、成本更低的基础信息服务。汉升链是最贴近真实社会需求和现实应用的区块链。

汉升链提出 NAC (Network of Address-Chain) 多链结构以及更贴近真实应用场景的GPoS (Guaranteed Proof of Stake) 共识机制，致力于解决传统区块链交易速度慢、分区性差、手续费昂贵、能耗高、无法建立信用体系、普通用户难以使用以及缺少必要的基础应用功能等一系列问题。

## 2. 行业背景
### 2.1. 共享经济

由于供需之间的信息不对称，再加上交易过程中陌生人难以建立直接信任关系，因此可以被流转使用的大量闲散社会资源不能得到充分利用，这是对社会财富的巨大浪费。

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image001.png)

 
移动互联网时代到来之后，经过应用厂商接近十年的努力，已经让共享经济的消费理念深入人心。在出行、旅游、金融、教育、住宿、日用工具、通讯（比如Wi-Fi万能钥匙）、众包、生产能力（比如智能机床）等领域，这些厂商基于共享概念开创了大量优秀的平台应用，并在部分行业取得了很好的经济效益。

### 2.2. 物联网 — 万物互联
据市场研究公司 Gartner 称，2017 年全球物联网设备数量可达到 84 亿 —— 比 2016 年的 64 亿增长 31%，而全球人口数量仅为 75 亿。到 2020 年，物联网设备数量将达到惊人的 204 亿。Gartner 称，2017 年全球物联网设备和服务总支出预计达到约人民币 13.8 万亿元。其中大中华区、北美和西欧这三大地区的物联网设备占到物联网设备总量的 67%。

这些设备具有各式各样的功能和形状，具备不同的计算能力和P2M（人与机器）及M2M（机器与机器）交互接口，设备与设备之间可以通过中心化或者去中心化的注册中心互相发现并交换数据。结合人工智能芯片，自主交互的物联网设备能形成高度智能的物联网络，为提升工作效率、缩短研究和制造时间、节约社会成本、改善人们的生活做出巨大贡献。智能物联网络将覆盖人们日常生活和工作的每一个环节。

为更好地利用设备能力，更好地为用户提供服务，增强设备的可用性和易用性，设备的使用者应该能够安全便捷地访问和控制这些设备，设备和设备之间应该能够自主建立连接，自动交换信息和数据，自动发起和接收交易请求——这是智能物联网络的技术基础。

物联网设备在智能制造、环境监控、智能家居、供应链管理、仓储管理、设备标识和认证等方面已经取得广泛应用，但是，物联网设备的互联互通能力、数据共享能力都有待提升；如何将物联网设备的"数字信息"和"物理资源实体"相结合等实际应用问题的探索还处于起步阶段，应用和基础设施建设也有待大力开发。这些都需要我们不断利用新的技术来发展和完善的物联网生态系统。

以安全的点对点连接技术为基础，设备所有者能够灵活制定租用规则，出租自己的设备或设备能力，比如能源生产、科学计算、数据存储、网络带宽等等；通过设备之间的自主交互以及对设备数据的采集和规划，设备的使用者能够轻松盘点库存，订购原材料和零部件，跟踪物流信息，管理供应商，根据零售渠道的库存和用户反馈预测并制定生产计划；通过可信设备标识，用户能够查询设备（以及相关物理对象）的生产、制造以及流转信息；结合智能制造，工厂可以随时接收用户的弹性订单，并自动购买原料进行加工生产，同时保证整个过程对客户透明可见。

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image002.png)
 
### 2.3. 区块链和智能合约
由中本聪精心设计的“比特币”，是区块链思想的第一个可用实现。比特币以密码学为基础，以工作量证明（PoW）共识机制为核心，完整解决了交易匿名性、交易可信性、交易记录不可变更性和系统可靠性等问题，成为第一个去中心化的分布式的共数字账本。

鉴于区块链所提供的匿名性和可信性等优点，基于区块链的数字货币迅速得到了大量用户的认可，截至 2018 年 1 月 22 日 21 时 30 分，比特币市值已经超过 193 亿美元，每一个比特币的价值超过 10,000 美元。

在比特币之后，以“以太坊”为首的智能合约平台，将代币（Token）发行、代币交换和代币使用推进到实用阶段，得到社区的广泛认可，并形成了巨大的经济生态体系。

基于智能合约，企业和个人能够用“代币”为数字资产、物理资产和投资收益进行定价和交易，促使以太坊成为最火热的新兴价值流转（融资和权益交易）平台。
 
![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image003.png)

### 2.4. 物联网 + 区块链

自 2008 年比特币面世以来，专为加密数字货币设计的区块链技术得到广泛普及。去中心化和可靠共识的信息交换机制吸引了大量创业公司和 IoT 设备制造商为降低信息系统的开发和运维成本，建立真正可信智能的全球性物联网络，致力于将区块链和物联网结合，以整合物联网生态中的各个环节。

IBM 的研究报告表明，和传统的中心化服务相比，去中心化的物联网平台可以为企业（以及最终用户）节省 99% 的系统构建和运维成本。

在区块链和物联网结合的研究机构和组织中，最著名的是可信 IoT 联盟。

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image004.png)

目前，各厂商的工作方向主要集中在身份认证、互联互通、信息记录、资产交易、供应链管理和优化等如下几个方面：
-	为用户提供安全、可靠的设备标识服务
-	为用户提供资源（数据、能源、带宽、存储）共享服务
-	扩展链的处理能力，为海量物联网设备互联互通提供超高吞吐的消息系统和交易系统
-	为安全可靠的设备间信息交换、信息处理提供基础组件

基于上述技术改进，并结合现有的区块链技术和区块链之外的通信、安全等技术，在应用层面各厂商主要为用户提供如下服务：
-	仓储及供应链管理 ，以及与之相结合的智能制造、生产预测和监控等服务
-	人、设备、组织等对象的身份识别
-	清洁能源等资源交易
-	音频、视频等数据信息的知识产权等级和知识产权保护

## 3. 新兴市场：物联网投资和数据交易

###	3.1. 物联网设备的价值和分类

按照物联网设备的功能和运营模式，具有投资价值的常见物联网设备可分为如下几类。

**高价值无人值守设备**：高价值无人值守设备具有很强的使用价值，主要用来满足人们日常生活中的娱乐等日常需求，具有很好的投资价值。比如摆放在公司里的自动售货机和饮料机；在人流密集处安置的抓娃娃机等娱乐设备；高铁站、商场里的自助按摩椅；电影院门口的自助点唱机（Mini KTV ）；公园里的迷你自助健身房；以及汽车充电桩等等。   

**短时租赁设备**：共享单车，共享汽车，共享无人机，共享充电宝等。

**生产能源的设备**：能源具有毋庸置疑的直接使用价值。比如小型水电站，小型家用光伏发电站等清洁能源设备；车载行驶记录仪；温度和湿度等工农业传感器。

**生产信息的设备**：大量设备上的传感器持续从自然环境、设备运行状态中搜集信息，这些信息对设备的主人的直接使用价值很小，或者仅具有一次性使用价值；但是将数据搜集汇聚，然后经过大数据分析和人工智能处理，可以为设备制造、环境优化、提升物流效率、甚至保险和二手车交易等大量应用提供坚实的数据支撑。设备的主人也能够出售（本来无用的）数据使用权来获得经济回报。

**占用物理资源的设备**：这些设备的价值通过他们占据的物理资源来实现，物联网设备设备是人们访问或者使用物理资源的手段，比如自助缴费的独立停车位。

**有闲置计算能力的设备**：海量中低端物联网设备具有闲置的计算能力、存储能力和网络带宽；将闲置计算能力租借给其它用户，可以为设备的主人分担设备购买成本并带来收益。

### 3.2. 投资物联网设备遇到的问题

**安装维护**：无人值守的大型设备必须安装到特定物理位置，并定期进行维护保养。普通投资者没有能力做到这点，和自己耗时耗力处理相比，把这些工作交给专业的服务厂商来处理是更好的选择。

**记账和结算**：产生信息和能量的设备，在出售生产出来的信息和能量时，需要灵活的计价方式，其中按照使用流量、使用时长来计费是最常见的结算方式。这类设备产生的账单额度低，交易对象分散，具有小额、碎片化的特点，不适合采用人工处理的方式来完成。因此计费平台必有具有自动化并且稳定可靠的记账和结算能力。

在多种场景下，比如设备由第三方代为维护，比如设备的所有者将设备收入进行抵押，比如多人联合投资等等，都更要求把设备收益以可信任的方式保存在账本上。

**金融服务**：大型物联网设备属于重资产投资。个人投资人在投资时可能无力直接支付现金购买一台设备，商业公司在投资购买设备之后，也希望能回笼部分资金。

传统金融服务注意到了这些困难，并通过一些产品手段来规避这些问题。例如，允许以融资租赁/分期支付的方式购买设备，但由于传统金融服务的成本高，传统金融提供的融资租赁服务只能针对特别高价值的设备。

### 3.3. 汉升解决物联网投资难题

通过长期的市场竞争，传统电商积累了大量优秀的产品功能。除搜获商品和下单购物外，以大数据和人工智能支撑的商品评价和商品推荐系统，物流配送，以及售后服务和金融服务等子系统也是现代电商平台不可或缺的重要组成部分。

物联网设备，特别是高价值无人值守设备具有非常好的价值。但是传统电商和金融服务提供给用户的交易模式以及支撑这些交易应用的底层技术，并不适用于上述物联网设备交易—— 特别是以投资为目标的物联网设备交易。由于缺少合适的服务平台，投资者在购买和管理这些设备时，常遇到资金压力、设备运维困难、以及收付款等各方面的问题。

个人投资者在投资高价值无人值守设备时，需要处理设备运维和收账等问题；如果委托给第三方代管，又必须存在可靠的信任体系，保证财务数据（设备收入）的可靠性。商业公司在投资此类物联网设备时，则需要解决一次性资金投入大，需要更灵活的融资手段和融资渠道等问题。大数据已经在现有的金融业务中发挥了大的作用，一旦可以通过区块链技术确保物联网设备运营数据的真实性和可靠性，针对物联网投资的金融服务就有了更多的可能性。

物联网设备产生海量数据信息，需要超高并发的交易处理能力，用中心化的结构来处理需要高昂的系统开发和维护成本，最终这些成本还是要转嫁给用户。
为了最大化利用社会闲置资源，去中心化的区块链方案能够降低共享系统的信息发布代价，建立透明的用户信誉评价系统，最大化的加速信息流转，并最小化直接用户所需要分担的系统成本，从而对个人和企业的共享行为合理的激励。

## 4. 汉升链商

汉升为用户提供简单易用、高度安全、高度灵活的物联网电商服务。投资者可以在汉升链商上发现和发展新颖的投资方式，从设备共享、设备交易、设备证券化、以及数据交易中赚取经济利益。最终用户可以在汉升链商上租赁设备、购买数据，避免支付中心化服务所带来的昂贵（不必要）成本。

除直接租售设备的使用权之外，通过汉升链商，用户可以从下列场景中受益，实现更加良好的资产流转和更高的设备利用率：

1.	合作加盟，小投资人独立购买设备，商业团队集中运维管理
2.	出借设备，按次数和使用时间获得收益
3.	出售设备的短期收益权
4.	出借自己的生产和管理能力，为他人代管（维护）设备
5.	出售设备，转让所有权，转让时甚至可能不需要交割设备
6.	抵押、保险等金融服务

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image005.png)

### 4.1. 合作加盟
共享单车、共享汽车等行业属于超重资产行业。商业投资者需要消耗巨量资金才能投放足够多的设备，以覆盖用户的主要活动范围。对企业来说这会带来巨大的资金压力，而小规模投资者，比如个人投资者，则更不可能具备这样的投资能力。

使用汉升链商，商业投资者可以采用合作加盟模式，由个人投资者购买少量设备，以加盟合作的方式形成完整的地域覆盖。个人投资者获得了良好的投资渠道，能提供优秀产品的商业团队则可以极大地减轻资金压力，专注于产品开发和用户服务。

个人投资者拥有对自己所购买设备的所有权。将这些设备委托商业团队统一管理后，个人投资者的收益由汉升链的分布式账本和智能合约保证。设备损伤等意外情况，则可以交给汉升链商上的第三方保险服务来降低投资风险。

### 4.2. 出售长期收益

用户发行代币转让物联网设备的收益权，之后通过定期回购、收益分红等多种方式向代币持有者发放投资回报。

汉升链的分布式账本和智能合约可保证用户资产的真实性，保证代币持有者的收益权。

比如预售某商业地产在未来五年内的停车收益；停车场管理者发行代币回笼部分资金，缓解资金压力；依据汉升链上设备的真实运营记录，投资者竞拍优质地段的停车场，或者单独竞拍某一个停车位，享受超额投资回报。整个过程公开透明，租售双方的交易成本远低于传统的中心化应用。

拥有独立车位的个人用户，可以预售车位的收益权，降低自己购买车位时的现金压力。

用户之间能通过智能合约，将零散的、分属于不同用户的同类资产组成共享联盟，便于其它投资者集中购买（或租用）。

### 4.3. 共享设备能力和使用时间

通过智能合约出租自己的设备，向其他用户提供数据、能源以及物理资源，比如出售计算能力、存储能力、网络带宽、电力等等。

设备能力租用的主要难点有两个：

1.	如何对服务节点的服务质量进行有效评价，即信誉评价机制的安全性和有效性；
2.	如何计价和结算，包括谁来定义价格，是否存在价格欺诈，按照什么样的周期和方式进行结算等；

信誉评价机制是汉升链GPoS共识机制所解决的主要问题之一；计价和结算问题则是汉升链的NAC多链结构所解决的主要问题之一。具体技术实现请参见“汉升链架构简介”。

### 4.4. 共享生产能力和管理能力

用户投资物联网设备，并委托第三方管理这些设备，然后向第三方支付固定的管理费用，或者按照约定的方式和第三方进行收益分成。

比如用户投资购买Mini KTV，委托服务方部署在影院、商场等人流密集的位置，并支付费用让服务方负责KTV设备的清洁和维护。Mini KTV的所有收益都记入汉升链，通过智能合约绑定，用户直接获得这些收益，不需要经过第三方的支付系统。

比如用户购买猪仔并委托绿色农场代为照管。用户支付一定的费用，养猪场定期发布猪仔的生长状态，并最终将猪肉交付给用户；也可以依照用户的委托将生猪出售。如果用户愿扩大投资规模，还能委托养猪场代为喂养数百乃至数万头生猪，和农场分享最后的销售收入。

### 4.5. 金融服务（依靠交易流水和信誉评估）

汉升链上保存每台设备的交易流水，这些交易不可被任何人篡改。可信的交易记录能够让金融机构快速评估每台设备的盈利能力，对设备的长期盈利能力做出评定和预测，然后根据这些评测为投资者提供设备贷款、设备质押、投资收益保险等灵活多样的金融服务。

1.	设备贷款：查看交易记录和信用记录，依据链上的可靠数据发放贷款。
2.	设备质押：根据设备的历史收益，评定未来一定周期内（比如一年内）设备可能产生的收益，据此计算质押设备对应的贷款金额。
3.	设备收益保险：当投资者购买物联网设备后，为规避投资风险，向金融企业或加盟厂商缴纳保险金，金融企业根据同类设备的历史收益情况承保投资人的投资收益。

### 4.6. 其它应用场景

和传统区块链相比，汉升链针内置了设备注册、信誉评价、账户委托、链外交易等应用能力，并对并发交易性能做了巨大提升，这些改进让汉升链能够很好地满足如下应用场景：

1.	物联网设备管理系统：提供设备注册、查找、远程控制、数据通信、设备升级等服务；
2.	供应链管理系统：提供资产跟踪和车队管理等服务，允许企业轻松定位和监控关键资产，以优化物流，维持库存水平；
3.	商品溯源和生命周期追踪系统：从生产到最终零售，所有商品都会在物流、仓储等环节经过复杂的存储和流转过程，真实有效的流转记录是保证这些环节可靠性的基础；
4.	供应链金融：让金融服务商快速确认企业的资产和负债，实时评估企业信誉和偿还能力，为企业提供高效灵活的供应链金融服务。

## 5. 汉升链技术架构简介

### 5.1. 区块链 vs. 汉升链

经典区块链主要由网络和存储层、核心扩展层，以及应用服务层等三层结构组成。各层的主要功能模块如下图所示：

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image006.png)

和经典区块链对比，汉升链针对物联网应用的多种场景做出了全面的基础架构优化和应用能力扩展。具体细节如下图所示（和经典区块链相同的部分不再列出）：

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image007.png)

### 5.2. 设计目标 

专为加密货币设计的区块链技术在比特币和以太坊上得到了巨大成功和社会认可，但是在处理物联网相关的真实应用场景时，存在交易性能差，确认周期长，在可用性、一致性和分区性（CAP）之间的平衡性不合理等问题；另外还缺乏端到端安全通信等多种必要的基础网络服务，以及账号管理和设备管理等应用服务。

因此需要新的架构将区块链和物联网相融合，以适应多种多样的复杂应用场景。新的系统架构需要在安全、可靠、可信的基础上，让设备和设备之间能自主沟通协作，让人和设备之间的交互更加便捷，让交易双方的信用评估和交易验证更加快速可信，让数据搜集、汇总和处理更加高效透明，从而实现万物可信互联，构建自主智能的全新物联网系统。 

这正是汉升链的设计目标 —— 以比特币、以太坊、EOS和IOTA取得的巨大工程成果为基础，结合真实应用场景和用户习惯，让后区块链“走进日常生活，实现智能互联”。

###	5.3. 设计原则

长年的技术管理和产品开发经验，让汉升团队深刻理解应用场景的多样性和复杂性，因此汉升链在保证系统安全可用的基础上，会尽力给予用户更多的选择自由，避免因底层架构的设计限制，而被迫限定用户使用上层应用的行为模式。

### 5.4. 技术框架名词解释 

详细的技术架构和运行原理请参考《汉升链技术架构白皮书》。

#### 5.4.1. 地址链（Address Chain）
比特币中的交易对象只进行对等匿名交易。但是物联网体系中的参与者天然地具有不同的类型和角色，在系统中必须予以明确区分。汉升链内置三种角色，通过合理的组织，开发者和用户能够用这三种角色实现所有的业务场景：

1.	设备所有者 — 拥有设备，能够转让设备的所有权和使用权
2.	设备使用者 — 能够控制设备、获取和更新设备状态
3.	物联网设备 — 设备之间可以有从属关系，设备可以自主交易

汉升链采用多级地址来描述真实世界中设备管理和使用过程中的层级结构。

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image008.png)
  
在汉升链中，每个账号（人、组织、设备）、合约都拥有全局唯一的散列地址（HA, Hash Address）。地址的拥有者，以其拥有散列地址所对应的私钥为唯一验证用户身份的合法依据。

汉升链为每个哈希地址分配一条链，链的功能与经典区块链相同，但是链上的交易节点会指向其它相关链，形成有向无环的哈希价值网络。

这种为每个哈希地址都分配一个链的做法，叫做地址链，即 Address Chain。

#### 5.4.2. 间接地址（RA, Reference Address）

通过智能合约，用户可以为自己的散列地址指定一个或者多个“可读地址”（human readable address），作为该地址的别名。可读地址是间接地址的一种。

间接地址在链的“地址注册表”有对应的属性节点，但没有自己的链对象实体。

#### 5.4.3. 地址之间的层级关联

通过智能合约，用户可以将当前地址授权给另外一个地址（可以是散列地址或可读地址）全权管理，以此实现地址的层级关系。

地址的层级关系能够解决真实物联网世界中的设备归属问题，比如一家企业可能拥有数千个物联网设备，其管理人员只需要通过企业地址（账号）就可以统一管理所有的网络设备。

地址的层级关系也可以解决真实交易场景下的开支来源问题，比如当物联设备实现智能组网和智能交互时，设备之间的交易，在本质上是其拥有者之间的交易，因此系统在处理交易时必须了解设备和其它地址之间的从属关系（以及操作或执行权限）。

#### 5.4.4. NAC — 由交易和多链构成的有向无环图

在汉升链中，通过交易将相关的地址链（Address Chain）关联在一起，所有的链和交易构成有向无环图，这样得到的价值网络被称为NAC，Network of Address Chain。

和主流区块链方案以及其它使用DAG的方案相比，汉升链主要有如下显著区别：

1.	为每个地址设置一条独立的链。这样的优点是用户可以选择一个或者多个见证节点。每个见证节点不用保存无关数据，在执行节点迁移时，新的见证节点只需要从旧的见证节点同步很小一部分数据集就可以开始为被迁移节点提供服务。
2.	链和链之间可形成任意多级的网络关系，高级别的链仅用来确认低级别链上的区块；低级别链在整个网络中可以只被少数服务节点存储和更改，即形成局部链，基于此能力，网络中的节点可以随时组成自己的联盟链或私链。
3.	链的地址和账号地址相同，根据功能上的区别可以将链分为三种：
-	实体链，用户（人、设备、组织）创建的账号所对应的链
-	公共链，为完成某种功能而设定的、对所有参与者都可见并受其约束的链
-	私有链，由单独或者几个服务节点创建的链

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image009.png) 

#### 5.4.5. GPoS — 权益证明担保

经典区块链的共识机制建立在这样的假设之上：所有网络节点都应该被贴上不可信标签，但网络中51%（或者66%等其它数字）的节点是善意节点；为了完成交易，用户发送的交易请求必须被全网中特定比例的节点确认，或者被绝大多数评选出来的代理人确认之后才算完成。因此经典区块链系统既不能实时确认交易，又在可支持的并发交易数量上存在巨大瓶颈。

经典区块链的另外一个问题是，如果发生较大面积的网络故障，独立网络环境下或者无法生成有效交易，或者在和主链合并时会将已经确认的交易回滚。这都完全不能满足物联网系统的交易需求（具体描述参见上文）。

根据CAP原则，数据一致性、可用性、以及分区容忍度不能同时得到最大程度的满足。因此一些非常优秀的新兴主链方案希望通过牺牲数据一致性来大幅提升可用性，以及整体系统的分区容忍度。对于以交易为主要目的系统来说，牺牲数据一致性同样无法令人满意。

基于汉升团队在应用开发方面的深厚经验，汉升链在设计共识机制时，采用了一种不同于上述两种方式的机制：

1.	牺牲部分数据一致性：不强求数据的全球一致性，但要求所有入链的交易都具有逻辑上的合法性（在其相关地址链上一致）
2.	牺牲部分可用性：为了获得更好的服务，用户需要为自己的交易选择见证节点（或者见证联盟），在选在见证节点之后，用户的交易只能由见证节点代理，如果见证节点失效（或者见证联盟集体失效），则用户不能进行任何交易。
注：高级见证机制可以在此时将用户的单笔交易退化到全局DPoS共识上，当见证节点全部失效时，用户可以额外支付手续费应对突发性交易请求
3.	确保分区容忍度

实现上述机制的共识机制叫做权益证明担保（GPoS, Guaranteed Proof of Stake）。该机制结合了PoS和DPoS的部分特点，同时和它们又有如下显著区别：

1.	在DPoS中使用代理人概念，代理人由网络选举产生；而GPoS中使用担保人概念，担保人由服务节点自愿提供，任何节点都可以把自己声明为见证节点；
2.	在DPoS中用户发起交易时必须使用网络选举出的代理人；而GPoS中用户自愿选择担保人（或者多个担保人形成的担保联盟）
3.	如果选择担保联盟，则用户发出的交易请求必须被联盟中 2/3 以上的节点确认之后才算成功；
4.	在DPoS中代理人要收取转账手续费，而且只能提供智能合约能力范围内的计算服务（包括转账）；而在GPoS中，只要用户授权，担保节点可以为用户提供储蓄、密钥恢复等多种日常生活中最经常使用且必不可少的金融和身份认证服务
5.	在PoS和DPoS中，没有用户的私钥就不能对用户的资产做任何操作；在GPoS中同样遵循这一设计原理，但经过用户明确授权的见证节点可代替用户行驶资产管理权

汉升链的设计理念是“底层架构允许用户灵活选择系统使用方式”。这一理念在GPoS上也得到了充分体现。在汉升链上，用户能够根据自己对隐私和应用功能的使用偏好，选择最适合自己的上链方案：

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image010.png)
 
#### 5.4.6. 见证节点 — 交易打包 + 金融服务 + 身份服务

如上文所述，结合汉升链独特的多链和多级网络结构，见证节点能够让汉升链的并发交易吞能力无限扩展，不存在理论瓶颈。除加快交易速度外，见证节点还有其它重要作用：
1.	用户指定的见证节点可以锁定用户账号，帮助用户更换密钥；
2.	用户指定的见证节点可以接管用户账号中的数字资产，为用户提供完善的金融服务，避免让用户的数字资产白白的躺在账号上

### 5.5. 链外系统

汉升链中的节点被分为“服务节点”和“边缘节点”两类：
-	服务节点（service node）：向边缘节点提供汉升链服务
-	边缘节点（edge node）：物联网设备，没有足够的计算和存储能力，通过服务节点访问区块链；服务节点可以是自主搭建的私有节点，也可以是开放的公共节点。

在汉升链中，一个服务节点可以提供一种或者多种服务。同时提供设备能力和汉升链服务的节点称为全功能节点。汉升链上的服务的类型有如下四种：
-	存储服务：维护分布式文件系统，为边缘节点存储消息和其它信息
-	计算服务：为边缘节点执行智能合约之外的计算任务
-	见证服务（Witness）：见证链上的交易，负责存储及确认交易
-	中继服务（Relay）：为节点之间的端到端通信提供中继隧道

#### 5.5.1. 链外系统

存储服务、计算服务和中继服务在本质上都属于链外系统。作为通用物联网平台，他们是汉升链不可分割的一部分。链外系统的身份认证、配置引导等信息都存储在汉升链内。

链外系统提供的服务可以是收费服务，也可以是免费服务。当节点使用收费服务时，费用结算在链内自动完成。

#### 5.5.2. 存储节点：IPFS

汉升链底层的分布式存储系统采用 IPFS 作为底层技术平台。

星际文件系统（InterPlanetary File System，缩写IPFS）是一个旨在创建持久且分布式存储和共享文件的网络传输协议。它是一种内容可寻址的对等超媒体分发协议。在IPFS网络中的节点将构成一个分布式文件系统。它是一个开放源代码项目。

IPFS协议利用比特币区块链协议和网络基础设施的优势来存储不可更改的数据，移除网络上的重复文件，以及获取存储节点的地址信息——用以搜索网络中的文件。IPFS提供了一个高吞吐量、按内容寻址的块存储模型，及与内容相关超链接。这形成了一个广义的Merkle有向无环图（DAG）。IPFS结合了分布式散列表、鼓励块交换和一个自我认证的命名空间。IPFS没有单点故障，并且节点不需要相互信任。分布式内容传递可以节约带宽，和防止HTTP方案可能遇到的DDoS攻击。该文件系统可以通过多种方式访问，包括FUSE与HTTP。将本地文件添加到IPFS文件系统可使其面向全世界可用。

#### 5.5.3. 计算节点与云服务

计算节点为边缘节点执行智能合约之外的计算任务，计算节点并不需要和边缘节点部署在同个物理区间，而且计算节点需要的计算能力与标准化的容器或者虚拟机一致。
Docker作为云计算领域近几年最热门的技术，解决了用户了在部署与发布的痛点，极大地提高了生产效率。汉升链为计算节点提供标准 Docker 套件。让服务提供者能够一键部署存储服务。这样计算节点不仅可以运行在支持Docker的云服务上，也可以运行在单台电脑上，以便进行测试开发。

传统公有链的计算节点一般使用专业的GPU或者ASIC矿机充当，在计算节点上扩展智能合约的能力就会受到很大的限制。汉升链使用Docker化的计算节点，不仅有利于去除专业硬件的依赖化，同时有利于开发者与用户的使用与部署，利用全球云厂商实现物理上的分布化，而且还可以利用容器即开即用的特性为每个智能合约提供单独的运行环境 。

计算节点可以在AWS、 Windows Azure、Google Compute Engine运行，也可以在全球其它的云服务厂商上运行，同时也可以用户自己的IDC里运行。

#### 5.5.4. 中继节点

物联网设备以及设备的使用者所处的网络环境可能非常复杂，为了确保设备之间能够互联互通，在不得已的情况下（即不能直连、也不能穿越防火墙）需要由中继节点为通讯者提供可靠的数据传输通道。

### 5.6. 目录存储（Directory Service）

目录服务是汉升链上的一个特殊公有链。其目的是存储整个系统中的节点信息，用来辅助执行交易、节点通信和节点管理等功能：
-	公开信息：可读地址和散列地址映射、地址的服务节点配置、地址的从属关系。
-	私密信息：地址的私有属性，比如公网 IP，支持的协议，设备能力等。

在链上实现并应用目录服务由汉升链首创。汉升链上的目录服务能够处理海量物联网设备交互所带来的超高并发数据查询请求，能够保证设备注册信息的真实可靠性。利用非对称加密等安全手段，还可以保证目录数据的私密性。

### 5.7. 交易及非交易消息类型

根据CAP定理，数据一致性、分区容错性和系统可用性不能同时兼得。对于全球性的物联网系统而言，必须根据具体的应用场景在这三者之间进行取舍。良好的通用底层架构不应该强迫用户接收某种既定方案，从而让用户被迫为不同的常见应用场景寻找多种解决方案，甚至很可能还要花费大量时间和经济成本将他们集成在一起。

识别不同场景下的消息类型，将这些类型进行抽象并实现，让汉升链能够在一个平台上为用户供多种选择。

#### 5.7.1. 交易（Transaction）

“交易”由一个或者多个发起方、接收方组成；交易的内容是交易的发送方向接收方转发一定数量的汉升币（或其它 token）。

服务节点在收到并确认该交易时，首先验证交易的合法性，即发送方是否使用了伪造身份；然后检查并确认发送方是否具有足够的账号余额。

#### 5.7.2. 声明（Announcement）

声明类似于欠条（IOU），“资金到账声明”相当于“收款确认单”。通过“声明”消息，可以实现远比交易更灵活的金融服务。

比如：轮胎厂商和汽车厂商具有非常好的信任关系，因此决定通过“声明”来记账。
1.	汽车厂商：收到1000 个轮胎，应付 200,000 元人民币
2.	汽车厂商：收到 500 个轮胎，应付 100,000 元人民币 
3.	轮胎厂商：收到货款 300,000 元人民币

在这样的场景下，如果两个厂商设置了大致相同的见证节点，则交易的稳定性、时效性、并发交易处理能力都将得到巨大提升。

#### 5.7.3. 通知（Notification）

通知（单向消息）时设备和设备通讯的一种重要手段。汉升链的通知由服务节点保存和转发。服务节点应尽可能保证消息的可靠性（Best Effort Service），但设备的应用层不能依赖于服务节点的可靠性。

通知消息是单向消息，接收者不需要发送任何响应。复杂的消息交互由应用层自己完成。

## 6. 技术先进性

###	6.1. 无手续费 + 高并发交易

NAC多链结构和权益证明担保算法的结合，在确认交易时，只需要很少几个见证节参与就可以实现交易确认，就能能保证交易的不可篡改性。

这让汉升链可以极快地响应用户的交易请求，同时消除了每秒并发交易数量的限制。

###	6.2. 可局部运行 + 无双花，无分叉

指定见证节点（或见证联盟）的用户，只能将请求发送到该见证节点上。在见证节点上，该用户的交易只能被串行处理，因此不会出现“双花“等全局数据不一致问题。也就避免了在网络故障时被隔离成孤岛的服务节点重新上线后可能会面对的分叉问题。

### 6.3. 增强账号匿名性

用户可以根据自己的实际需求，在资产安全性和资产隐私性之间进行权衡，选择是否设置可读地址，是否为可读地址设置用于恢复散列地址密钥的智能合约。
地址的层级结构，以及地址的映射关系存储在汉升链上，由区块链保证其真实和有效性。

###	6.4. 可锁定账号，恢复密钥

可读地址除了能够提供友好的助记功能外，其首要目标是和见证节点一起，解决传统加密货币（区块链）中存在的两个问题：

**密钥管理难、丢失密钥等于丢失资产**：和技术极客不同，大多数用户没有能力妥善保管的自己的私钥，如果私钥丢失或者被盗的后果是账号资产丢失，则很难对系统做大众化的普及推广。密钥丢失时，用户需要快速恢复对资产的管理权；当密钥被盗时，用户需要快速锁定资产并更换新密钥。

**身份认证不够安全**：作为高频使用的交易工具，如果用户不具备保存密钥的专业知识，仅仅使用密钥不足以保证账号的安全性，需要有更灵活和丰富的多因子认证体系。

### 6.5. 链结构直接支持所有权关系

用户和设备的对应关系，是物联网系统中最核心的关系之一，如果该功能（以及其他类似功能）由上层应用提供，而不是内置在链的基础结构中，上层应用必须在链中或者链外寻求存储空间，设计合适的数据结构，保证数据更新和读取的一致性；而且难以把解决方案推广到全链统一使用，也很难把权限等功能应用到链的核心对象上。

汉升链在设计之初就把类似核心需求在执行效率、应用推广难度、以及功能特性等多方面的要求进行了全面分析和探讨，因此汉升链的基础结构在框架上能够满足此类核心需求。

### 6.6. 所有权和使用权分离

将所有权和使用权分离，可以有效的实现设备共享（租赁等）。

在系统中，所有权和使用权并非汉升链架构中的第一类属性，而是通过 profile 机制实现的一个应用功能。除所有权和使用权外，汉升链不会在平台架构层面提供复杂的权限管理系统 —— 这部分功能应该由灵活的应用层自行通过 profile 机制实现。

### 6.7. 有效信誉评价机制

增加有效身份的获取难度，是建立良好信誉评价机制的前提。如果用户能够迅速抛弃旧的账号，并零成本立即开始使用某个新账号，则所有的信誉评价机制都将失去所预期的监督和管制能力。

鉴于上述原因，当用户需要参与到信誉评价体系时，必须加大用户获取账号的成本，特别是培养高信誉账号的成本，来规避用户频繁切换账号的风险。有效身份的稀缺，是阻止极端用户作恶的重要手段。

汉升链上的见证节点，不仅可以见证交易，还可在链上确认用户的身份，为用户身份的真实有效性背书，解决陌生场景下投资人和用户的互信问题。

## 7. 愿景和发展规划

###	7.1. 团队愿景

用产品改善生活，用技术推进社会进步。

汉升团队坚信，物联网时代即将来临，物联网设备的智能互联互通，以及设备能力的共享将极大地节约社会成本，为生活便利和经济发展做出巨大贡献。因此为设备共享和价值交换提供服务的链商平台将成下一代电商平台，其交易体量会超出目前市面上所有的传统电商。

为链商提供基础支撑的主链（汉升链）技术，能作用于日常生活所需要的其它应用场景，为衣食住行、协同协作、生产制造提供服务。

### 7.2 执行计划

汉升链商的发展规划大致如下：
-	2018.09, 汉升链商正式上线，和六家以上合作伙伴展开业务合作
-	2019.06, 对接银行、保险等附加金融服务，在线物联网设备超过 10 万
-	2019.12, 拆分主链项目，汉升链独立试运营，作为通用主链为其它系统提供服务
-	2020.06, 成为最好知名度最高的全球物联网链商

### 7.3. 推广策略

汉升的推广策略是以团队 BD 和社区建设相结合的方式，通过媒体宣传、用户口碑、政策引导等方式，让厂商和个体投资者了解并喜欢汉升链商提供的便捷投资方式，同时接受汉升链商。
-	与政府部门合作，建设区块链示范工程
-	与设备制造商，比如自动收货机、游戏机等厂商合作，帮助厂商吸引加盟投资人
-	与拥有物联网设备的商业公司合作，帮助厂商提升收益，降低资金压力
-	用挖矿奖励吸引个人投资者，并且让投资者在投资物联网设备时获取更大的收益
-	社区推广，奖励汉升链上的优秀应用
-	媒体和渠道宣传

###	7.4. 社区建设

汉升将学习现有成功区块链项目先进经验和管理理念，结合汉升团队的资源优势，充分发展设备生产厂商、政府、商业机构、个人投资者、开发者等社群用户。官方将建立社区交流平台。具体措施如下：
-	由汉升基金会和社区志愿者共同成立活动小组，汉升基金会从社区激励计划中拿出一部分代币作为志愿者的参与奖励；
-	活动小组主要负责市场开拓、发展顾问、安全检查、应用开发、需求整理、政策探讨、标准制定、活动组织、媒体宣传、联络协调等工作；
-	活动小组由汉升基金会协调，但小组管理层从社区中直接产生；
-	设立社区发展基金，接受捐助并扶持和奖励汉升链上的应用开发者

## 8. 汉升币

### 8.1. 汉升币（主链）

汉升链上承载价值流转的单元是汉升币。汉升币的总量固定为三亿，并按照下表描述的比例进行分配：

![image](https://raw.githubusercontent.com/hanshengchain/public-doc/master/images/image011.png)

汉升币发行格详细规则如下表：

HC的所有者 |	比例 |	数量 |	代币发行
----------- | --- | ----------- | ---------
主链生态激励 |	60%	| 180,000,000	| 不发行代币
社区生态建设 |	5% |	15,000,000 |	发行
天使投资者	| 5%	| 15,000,000	| 发行（有锁定）
私募及公募 |	20% |	60,000,000 |	发行
开发团队和HC基金会预留 |	10% |	30,000,000 |	发行（有锁定） 

汉升链在主链创世块中分配 9000 万汉升币，做为代币与汉升币兑换的准备金。预计在汉升链上线后 18 个月内完成代币兑换，并在兑换截止时永久销毁所有代币。

为弥补类似用户钱包丢失等自然损耗的流通量，以及保持其支撑的智能经济生态微量通胀等，汉升币每年保持固定同比 2% 的增发。增发的汉升币会平均分布在每个区块上。
为了保持汉升链生态的可持续发展，为开发和管理团队设置长期有效的激励机制，自汉升链正式上线后，五年内增发的汉升币将在基金会和矿工之间按比例分配。

### 8.2. 汉升代币（以太坊）
在汉升链主链发布前，所有投资人将在以太坊上获得“汉升代币“；当汉升链上线后，汉升链投资人将代币以一比一的兑换比例兑换成汉升链上的 “汉升币“。

汉升代币是基于以太坊区块链的 ERC-20 标准代币，汉升代币的代码开源在 GitHub 项目中，接受所有用户的监督和审核。

汉升基金会和开发团队持有的代币有 24 个月的总锁定期，这部分代币在项目启动后每六个自然月释放 25%。

汉升代币和以太坊（ETH）的兑换比例和兑换方式如下。其中的私募和公募部分为初始定价，汉升基金会将根据项目实际进展和资金需求进行分批募资、分批定价。
-	天使兑换比例：1:9000，半年总锁定期，逐月投放；
-	私募和公募兑换比例：1:6000，无锁定期

按照发行计划，汉升币在发行初期的总融资额为11,667 ETH，按照当前以太坊的交易价格计算，约等于630万美元。

### 8.3. 流通价值

预计在未来一年内，将汉升币的流通排名发展到全球加密货币市场的前 200 名。

预计在未来的两年内，将汉升币的流通排名发展到全球加密货币市场的前 100 名。

（注：实时币值排名及其流通市值请参考https://coinmarketcap.com）

## 9. 团队介绍
汉升团队以产品和高技术人才为核心。汉升团队在金融、区块链、物联网、网络安全及云平台建设方面均具有长期的高级技术管理和产品开发经验，具备物联网平台及公链开发所必需的技术能力、产品能力和运营能力。

### 9.1. 创始团队

李国鹏：毕业于清华大学。曾任北京风信科技有限公司CTO和CEO，为企业、家庭等办公设备和物联网设备提供端到端的安全通信服务。在加入风信前有七年创业公司、六年外企工作经历，最近十年主要移动安全通信、物联网通信等工作，另外在 Email, IM, OA, HIS, PACS 等传统企业软件上也有丰富的工作经历。

杨德升：毕业于上海交通大学，以太坊智能合约 DApp「以太红包」作者，现任汽车行业创业公司联合创始人 CTO，原OFO技术副总裁，周伯通招聘联合创始人 CTO，开源社区 ThinkSNS 核心开发者，拥有一项互联网技术发明专利，在社交产品、互联网技术、区块链技术等方面有丰富的经验。

### 9.2. 顾问团队（按加入时间排名）
段　念：花虾金融CEO。在加盟花虾金融之前，曾担任宜信互联网金融子品牌宜人贷CTO，见证了宜人贷在纽交所成功上市。之前他还曾在豆瓣网担任工程副总裁，并在Google、华为、乐元互动、OpenTV等公司任职。

郭理靖：现任京东云区块链实验室及云数据库负责人。他曾任北京同仁堂国际CTO，也曾在盛大创新院、阿里巴巴、金山等知名公司就职。他在云计算、分布式数据库、NoSQL、DevOps、区块链等领域有丰富的经验，拥有多项云计算相关的专利，也活跃于国内各大技术社区，曾在澳大利亚维多利亚大学做过一年访问学者。

杨毓丞：现任蛋糕、下午茶零售行业MES每实公司COO，原游谱旅行CTO，Tripadvisor旗下酷讯技术经理，亚信PRM系统核心研发，在旅游产品，电信产品，互联网技术等方面有丰富的经验。

熊昌伟：现任用友畅捷通公司运维总监，阿里云MVP。专注于云平台的系统研发与运维，对公有云、私有云、混合云都有丰富的研发经验，从2010年开始做虚拟化云平台，2014年转为容器云平台研发，2016年平台上运行的容器规模达到30万+。期间作为技术负责人与Intel\IBM\SUN建立合作研究室，在虚拟化、分布式存储上积累了非常丰富的研发和运维经验。现负责畅捷通技术运营团队，专注于小微企业SAAS云服务。通过技术运营的理念，为全国几百万小微企业提供稳定，高效的SAAS服务。

郭瑞华：汽车新零售平台小得科技 CEO。曾创建移动医疗知名品牌彩带网络，13年商业运营落地经验，曾就职于 MOTOROLA、NEC、GOOD Technology，负责中国全境的手机业务供应链、运营、战略，为企业创收亿元美金，成功发起和推动中国手机市场的运营模式改革。在企业战略发展和业务运营领域有成熟的落地经验。

赵　鹏：Hyper CEO，云计算开源领域知名专家，Hyperledger天使投资人，曾服务过摩根大通，量子基金，汇丰，雷曼兄弟，MUFJ等多家国际金融机构，拥有丰富的金融技术背景和经验。

## 10. 免责声明

本文档仅作为传达信息之用，文档内容仅供参考，不构成在汉升及其相关公司中出售股票或证券的任何投资买卖建议、教唆或邀约。此类邀约必须通过机密备忘录的形式进行，且须符合相关的证券法律和其他法律。

本文档内容不得被解释为强迫参与互换。任何与本白皮书相关的行为均不得视为参与互换，包括要求获取本白皮书的副本或向他人分享本白皮书。参与互换则代表参与者已达到年龄标准，具备完整的民事行为能力，与汉升签订的合同是真实有效的。所有参与者均为自愿签订合同，并在签订合同之前对汉升进行了清晰必要的了解。

汉升团队将不断进行合理尝试，确保本白皮书中的信息真实准确。开发过程中，平台可能会进行更新，包括但不限于平台机制、代币及其机制、代币分配情况。文档的部分内容可能随着项目的进展在新版白皮书中进行相应调整，团队将通过在网站上发布公告或新版白皮书等方式，将更新内容公布于众。请参与者务必及时获取最新版白皮书，并根据更新内容及时调整自己的决策。汉升明确表示，概不承担参与者因下述：A）依赖本文档内容，B）本文信息不准确之处，以及C）本文导致的任何行为等三条原因而造成的损失。

汉升团队将不遗余力实现文档中所提及的目标，然而基于不可抗力的存在，团队不能完全做出完成承诺。

汉升币是平台发生效能的重要工具，并不是一种投资品。拥有汉升币或者汉升代币不代表授予其拥有者对汉升链商的所有权、控制权、决策权。

汉升币作为一种数字加密货币不属于以下类别：(a)任何种类的货币；(b)证券；(c)法律实体的股权；(d)股票、债券、票据、认股权证、证书或其他授与任何权利的文书。

汉升代币的增值与否取决于市场规律以及应用落地后的需求，其可能不具备任何价值，团队不对其增值做出承诺，并对其因价值增减所造成的后果概不负责。在适用法律允许的最大范围内，对因参与互换所产生的损害及风险，包括但不限于直接或间接的个人损害、商业盈利的丧失、商业信息的丢失或任何其它经济损失，汉升团队不承担责任。

汉升遵守任何有利于互换行业健康发展的监管条例以及行业自律申明等。参与者参与即代表将完全接受并遵守此类检查。同时，参与者披露用以完成此类检查的所有信息必须完整准确。

汉升明确向参与者传达了可能的风险，参与者一旦参与互换，代表其已确认理解并认可细则中的各项条款说明，接受本平台的潜在风险，后果自担。

## 11. 参考资料
- https://www.trusted-iot.org 
- http://iota.org 
- http://filament.com 
- https://chronicled.com 
- http://energolabs.com 
- https://www.streamr.com 
- https://www.solcrypto.com 
- https://slock.it 
- http://identity.foundation
- https://github.com/EOSIO/Documentation/blob/master/TechnicalWhitePaper.md
- https://iota.org/IOTA_Whitepaper.pdf
- https://github.com/ethereum/wiki/wiki/Proof-of-Stake-FAQ
- https://groups.csail.mit.edu/tds/papers/Lynch/jacm88.pdf
- https://groups.csail.mit.edu/tds/papers/Lynch/jacm85.pdf
- https://blog.ethereum.org/2015/11/15/merkling-in-ethereum/
- https://bitcoin.org/bitcoin.pdf
