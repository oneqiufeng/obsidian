# 中国屋顶光伏的碳减排潜力_NC

#太阳能光伏 #高质量文章 #屋顶光伏 #能源 #建筑设计 #建筑屋顶设计 #二氧化碳

标题：Carbon mitigation potential afforded by rooftop photovoltaic in China

期刊：Nature communications

类型：Article

一作：Zhixin Zhang

通讯：Min Chen

时间：2023-04-14

DOI：https://doi.org/10.1038/s41467-023-38079-3

屋顶光伏（rooftop photovoltaics, RPV）对于实现能源转型和气候目标至关重要，尤其是在建筑密度高、能耗高的城市中。鉴于评估屋顶面积的困难，估计整个大国城市层面的RPV碳减排潜力具有挑战性。在这里，使用多源异构地理空间数据和机器学习回归，作者总共确定了 2020年中国354个城市的65,962 km2的屋顶面积，在理想假设下，这意味着4亿吨的碳减排量。考虑到城市土地扩张和电力结构转型，到2030年，中国计划碳达峰时，潜力仍有3-4亿吨。然而，大多数城市只挖掘了不到1%的潜力。作者提供了地理禀赋分析，以更好地支持未来的实践。这项研究为中国有针对性的遥控飞行器开发提供了重要的见解，可以作为其他国家类似工作的基础。

屋顶设计的过程中，考虑不同的形状接收到的能量和相关的光伏布置，会产生不同的电能、光污染等影响因素，作为0-1相关的测试指标，可以通过相关的内容进行补充。
#光伏城市 #光污染问题 #安全风险评价 
# Introduction
为应对温室气体排放带来的气候变化全球挑战，世界各国正在广泛合作。目前，作为世界上最大的二氧化碳排放国之一，且2020年的年碳排放量超过100亿吨，中国已经做出了一系列的碳减排努力。在第75届联合国大会上，中国承诺到2030年达到碳达峰，到2060年实现碳中和。作为高度依赖化石煤的主要能源生产国，中国的电力部门约占中国能源相关碳排放量的一半。太阳能光伏系统已被公认为一种有前途的技术，可以使电力部门脱碳，估计到2050年将满足全球25–49%的电力需求。2020年，中国累计光伏装机容量达到253GW，占全球装机容量的三分之一。最近，[[分布式光伏]]（distributed photovoltaic, DPV）系统因其广泛的适用性、易于本地实施、较低的峰值需求和更少的传输问题而成为首选。全国DPV系统安装份额从2016年的13%上升到2020年的31%。中国非常庞大的建筑存量，近几十年来经历了城市化和建筑热潮，为DPV系统的发展提供了有利的场地条件。此外，光伏与现有基础设施的整合为可再生能源分布式发电的开发和实施提供了新功能。为了更好地了解RPV的发展潜力以及该系统对碳减排工作的贡献，迫切需要在全国范围内进行评估。  

#碳排放 #节能减排 #建筑节能设计 

在城市层面评估中国的RPV碳减排潜力对于有针对性的可持续能源规划至关重要。一些城市层面的光伏应用研究作为案例研究被提出，并在实地调查的基础上进行了更深入的分析。然而，中国有300多个地级市，每个城市都有不同的地理条件和社会经济特征。现有的单个城市研究仅限于局域发展，因此不能作为中国其他城市的充分参考。值得注意的是，RPV系统以分散的方式部署，这增加了其评估的复杂性。最大的不准确性归因于建筑物屋顶的划定和计算。在以往的研究中，屋顶区域的详细测绘数据是通过高分辨率遥感获得的，信息处理成本很高；因此，对于中国大多数城市来说，这些数据很难获得。大多数现有的多城市研究都应用易于获取的国家统计数据，如建筑面积和土地利用，间接确定屋顶面积，当屋顶区域的数据不可用时，这些方法有效；但是，评估的准确性受到输入数据质量的限制。此外，国家统计数字一般在省级或更高一级汇总，这导致市级评估存在巨大差距。具有更高精度的详细地理空间数据对于估计RPV潜力至关重要。因此，有必要开发新的方法来解决全国范围内缺乏屋顶总面积数据的问题。

目前，我国城市建设正处于快速发展阶段。在人工智能等新技术的支持下，城市信息获取研究不断涌现和完善，为建立精细化城市测量提供了新机遇。为了解决城市级估算中通常遇到的主要数据和计算瓶颈，一种准确获得整个大国规模的屋顶面积的方法至关重要。为此，我们引入了一种基于机器学习的准确回归分析，该分析依赖于多源异构地理空间数据，特别是我们之前开发的矢量化屋顶区域数据集，覆盖了中国总面积的16%。我们的研究量化了354个中国城市的RPV碳减排潜力，这些城市在2020年覆盖了全国总面积的88%。此外，我们阐明了RPV碳减排潜力的地理异质性，并通过聚类分析揭示了这种变化的原因。考虑到城市土地扩张和电力结构转型的不同情景，我们估计了2030年中国计划达到碳达峰时潜力的未来变化。此外，还介绍了光伏安装、能源消耗和电网排放的现状，以支持对估计潜力的可持续利用。
# Materials and Methods

**1）假设和系统参数**
作者对本研究中涉及的RPV系统进行了统一的假设，包括组件效率、光利用率、组件表面污染、转换效率、逆变器效率、线损、传输效率和光伏系统可用性的系统效率修正参数光伏系统的平均能效比、光伏应用的规模和性能参数等，并假设系统中的所有光伏电池板都固定在水平位置。

**2）[[屋顶面积]]回归分析**
为了将现有的86个城市的屋顶区域与全国联系起来，开发了一个回归模型。选择道路长度、建成区、人口规模和夜间光照强度作为解释变量。这些变量在网格单元格中计数，最后聚合到结构化表中。

**3）RPV碳减排潜力评估**
见原文。

**4）位置条件的聚类分析**
对于影响RPV碳减排潜力的三个位置条件：屋顶面积、太阳辐射和电网排放，使用K-means++聚类算法将354个城市分为不同的聚类。
# Results
## **1）研究区域和城市代表**
本研究从作者在以前的工作中创建的大规模矢量建筑屋顶面积数据集中改进了建筑屋顶面积测量，其整体准确率和F1得分分别为98%和83%。该数据集覆盖了中国总面积的16%，包含具有不同行政级别和地理位置的城市，这些城市在经济，政治和地理上都是多样化的。基于该数据集，使用基于机器学习的回归模型获得国家屋顶区域。

屋顶区域到太阳能潜力的转换是使用高分辨率（10km）的中国表面太阳辐射数据集进行的，其性能优于大多数传统产品。为了评估RPV的碳减排量，我们使用了碳减排因子，该因子衡量RPV系统替代当地电网中现有和新建发电厂所产生的电力时的碳减排量。碳减排因子通过中国区域电网基准排放因子确定。

由于没有香港、澳门、台湾和西藏的基线排放因子，本研究区域包括354个中国城市，覆盖面积超过8百万km2。其中，基于矢量化数据集获取86个城市的屋顶区域，其余268个城市的屋顶区域则通过多源异构地理空间数据和机器学习的回归分析进行外推（图1）。

在本研究中，RPV碳减排潜力被定义为CO2通过RPV系统产生的电力替代电网电力而引起的缓解。结果基于屋顶可用性为35%，光伏电池板转换效率为20%，整体RPV系统效率为80%的假设。市级评估的主要投入和产出数据见补充数据1。为了解释不同RPV系统参数和屋顶可用性引起的变化，我们记录了2020年不同环境下的一组国家RPV碳减排潜力（补充表2）。解释主要结果的其他假设和限制分别记录在方法和讨论部分。

![[../../归档/picture/研究区域和城市代表性的概述.jpg]]

矢量化屋顶数据的地理范围。b, 太阳辐射数据。c,电网排放数据。d, 研究区域范围根据测量屋顶面积值的 86 个城市推断至中国其他268个城市。数据来源：所有城市行政边界均来自高德地图(Amap)。

## **2）屋顶面积的推断和验证**

屋顶面积以小区为基本单位外推；每个单元的面积为10km2。研究区域被划分为1,045,022个正方形单元。选择具有可用测量屋顶面积值的86个城市作为样本区域，总共191,370个单元格（补充表3）。为构建屋顶面积外推回归模型，选取道路长度、建成区面积、人口规模、夜间光照强度4个与城市建设密切相关的指标作为解释变量。可公开访问的高质量数据，包括来自 OpenStreetMap(OSM)的矢量道路网络数据、来自环境系统研究所 (ESRI) 的土地覆盖数据（分辨率为10m）、来自WorldPop的栅格人口数据（分辨率为100m）和地球观测组的夜间灯光图（分辨率为500m）。

![[../../归档/picture/回归分析中涉及的数据的可视化表示.jpg]]

a, 绿线划分外推法的基本单元。b, 橙色多边形代表矢量化屋顶区域，蓝线代表主要道路网络。以上海为例，c, 土地覆盖（建成区红色）表示潜在的建筑分布。d, 棕色值高的人口规模。e, 夜间光强度（数值颜色为棕色）显示了潜在的建筑集中度。数据来源：NNU-SCENS 实验室屋顶区域、OpenStreetMap、Esri Landcover、WorldPop Population 和 EOG夜间灯光图。所有城市行政边界均来自高德地图，卫星图像来自Google Earth。

我们发现所选的解释变量与屋顶面积有很好的相关性（图3）。还进行了敏感性分析，以证明所选变量的有效性（补充说明4和补充表4-6）。我们应用随机森林算法基于划分的数据构建回归模型。该算法的超参数通过10倍交叉验证进行调整（补充表7），最终建立一个可以准确预测屋顶面积的模型。在我们的测试中，与其他模型（补充说明5和补充表8）相比，基于随机森林算法的回归模型提供了更好的准确性（拟合优度，R2）和更少的总体误差（平均绝对误差，MAE）。

将训练好的模型应用于268个城市的非采样区域，得到屋顶面积预测值。为了验证外推结果，在中国六个地理区域中各选择了三个代表性城市，形成包含18个城市、覆盖134,29个单元格的验证数据集。为了获得用于验证的地面实况数据，我们使用深度学习语义分割方法从高分辨率卫星图像中提取建筑物屋顶（补充说明6和补充图1）。根据地面真实数据和外推数据的比较，我们建立的外推模型表现出良好的泛化能力，可以为大规模RPV评估的开发提供精细数据。对于每10km2的小区，MAE仅为0.06km2，大多数小区的误差在-0.05~0.05km2之间。在城市层面，屋顶总面积为2641km2的验证区域的累积误差为-26km2，相对误差仅为-1%。每个城市的相对误差不超过±20%（补充表9和补充图2）。

## **3）当前RPV碳减排潜力评估**

为了阐明决定RPV碳减排潜力的区位条件差异，我们使用K-means++聚类，根据屋顶面积、太阳辐射和电网排放三个代表性指标，将354个城市分为四组。这使我们能够分析所有城市RPV潜力的异质性并了解其原因。使用单因素方差分析（ANOVA）在不同聚类之间进行成对比较（补充表 10）。此外，94%的比较通过了0.01水平的显着性检验，表明聚类结果合理地反映了城市之间的差异。

如图4所示，我们观察到每个集群内的城市有明显的地理聚集，这表明邻近的城市群往往具有相似的RPV应用的区位条件。集群1地理位置分散，包含中国人口规模最大的一些城市，包括上海、北京和天津等直辖市，以及广州、苏州和杭州等省会城市或区域经济中心。人口规模大通常意味着建筑存量大，集群1内城市的平均屋顶面积达498km2，大约是估计平均值的三倍。集群2和集群3的城市主要分布在人口密集的中东部地区，占屋顶总面积的62%。集群2中的城市表现出相对清洁的电力结构，平均电网排放量（693 g CO2/kWh）低于集群 3 中的城市（837 g CO2/kWh）。集群4的城市主要位于中国人口稀少、经济欠发达的西部地区；四个组团中，该组团城市的平均屋顶面积最小（80km2），但太阳辐射强度最高（1667 kWh/m2）。

评估的RPV装机容量、发电量和碳减排潜力如图5所示。2020年，中国354个城市的RPV总减排潜力为40亿吨（BT），接近碳减排量的70%电力和热力部门的排放。城市的潜力范围为0.04至5200万吨 (MT)，平均值为11MT。因此，这项研究有助于更深入地了解城市层面的巨大差异。东南部地区集群 1-3中的城市贡献了89%的RPV碳减排潜力，这可归因于这些地区人口规模大、建筑存量丰富。特别是，碳减排潜力排名靠前的城市都出现在集群1 中，平均潜力为29MT。将这些城市的RPV碳减排潜力与三峡大坝2020年的碳减排潜力进行比较，后者发电量为112TWh，直接减少二氧化碳排放94MT。这表明，集群1中的一些城市，包括潍坊（52MT）、重庆（47MT）和临沂（46MT），其RPV碳减排潜力约为世界最大水电站的一半。由于更高的电网排放和更好的太阳辐射条件，集群 3 中的城市表现出比集群 2 中的城市 (9MT) 更大的平均潜力 (11MT)。集群4中的城市占总研究面积的 40%，通常表现出最佳的日照禀赋，但由于缺乏屋顶面积，平均潜力最低（6MT）。还估算了人均人口和GDP的RPV 碳减排潜力，显示出从东南到西北递增的趋势（补充图3、4）。

## **4）未来RPV碳减排潜力评估**

了解中国RPV碳减排潜力的未来变化对于更深入地了解其对国家双碳目标的贡献非常重要。尽管现有的数据并不能让我们充分考虑可能引起未来变化的所有因素，但我们选择了两个关键因素：城市用地扩张和能源结构转型，并结合文献分析了未来的变化。在本次评估中，我们选择了2030年，即中国计划达到碳排放峰值的一年。

中国快速的城市化、人口增长以及人口可支配收入的增加将导致其建筑存量不断扩大。建筑存量的增加将进一步增强RPV发展的潜力，但其影响尚未得到充分考虑。值得注意的是，中国的城市建筑设计和规划遵循统一的国家标准，城市建筑密度受到政府严格控制。此外，在大多数现有研究中，建筑屋顶面积与建成面积的比率范围为0.15-0.30。因此，在本研究中，我们假设这一比率将在2030年之前保持稳定，从而根据城市土地的扩张来预测屋顶面积的增长。未来城市土地数据来自一项考虑了未来不同社会发展路径的全球研究，表明2020年至2030年中国城市土地扩张率将在9%至14%之间（补充表11）。基于此范围，本研究设定了2020 年至2030年城市土地扩张的低速和高速情景（表1）。

![[../../归档/picture/不同城市用地扩张和电力结构转型情景下屋顶碳减排潜力的未来变化 1.png]]

## **5）开发RPV碳减排潜力**

为了了解如何挖掘中国能源结构转型的理论潜力并帮助实现国家的碳减排目标，我们进行了深入的定量和定性分析（图6）。定量分析以碳减排量和强度为指标，对城市发展RPV的优先顺序进行了四分位数排序。定性分析探讨了当前光伏安装、能源消耗和碳排放方面的理论潜力的发展。以省为单位进行分析，加深了对理论到实践转变的认识。

碳减排量遵循自上而下的视角，政府通常更关心当地的总潜力是否能够支持实现既定宏观目标的目标（图6a）。碳减排强度遵循自下而上的视角，企业和个人通常更关心单位潜力是否可以提供高效益（图6b）。以山西省11个地市为例，运城市贡献的RPV碳减排潜力最大，占全省的18%，更有能力缓解全省碳减排压力。同时，朔州的RPV减排强度最高，比全省平均水平高出4个百分点，在实施RPV项目时更有能力取得更高的环境效益。此外，综合考虑碳减排的总量和强度也很重要。碳减排潜力量和强度均较低的城市（如铜仁、自贡和安顺）可能面临更大的实施RPV的压力（图6c）。

为了论证理论装机容量与现有装机容量之间的差距，使用了2018年全国累计DPV装机容量数据，以及分布式光伏发电中80%的RPV份额。比较显示，73%的省/直辖市的装机潜力已开发不足1%（图6d）。这表明，尽管中国已成为全球光伏发电绝对产量和装机领先国家，但市场进一步拓展的空间仍然很大。为了论证理论发电量与当前用电量的比较，使用了2020年各省用电量数据。结果表明，80%的省/市的发电潜力超过当地用电量的一半（图6e）。然而，一些地区RPV的发展可能不足以补充当地的电力需求。为了对比理论碳减排量与当前碳排放量，我们使用了2019年电力和热力行业的当地碳排放量。结果表明，在北方和东北电网，RPV单位发电量碳排放的减缓将更加明显（图6f）。从电力脱碳的角度来看，在宁夏、山西等煤炭依赖度较高的省市，制造业、重工业密集，发展光伏发电可以更好地助力当地电力转型。

# Discussion

**1）研究区域和城市代表**

本研究对中国城市层面的RPV碳减排潜力进行了全国性评估。基于多源异构地理空间数据和机器学习回归方法，解决了现有估计中普遍面临的关键数据和计算限制。作为评估的一部分，我们创建了：(1)高分辨率10km2网格的全国屋顶面积数据集；(2)全国城市级RPV碳减排潜力数据集。此外，还考虑了城市土地扩张和电力结构转型的情景，以了解到2030年RPV碳减排潜力的变化。介绍了中国装机容量、能源消耗和电网排放的现状，以了解如何充分发挥潜力。尽管有各种旨在促进分布式光伏发展的有利政策，但相对于国家长期目标，地方光伏发电的采用仍然相当有限，需要采取更有针对性的措施，从区域角度提高公众意识。因此，本研究的结果可以通过趋势模拟、影响分析和区域比较来帮助确定当地RPV发展的关键因素。

我们的评估对于应对可持续发展和气候变化的双重挑战具有重要意义。首先，确定了354个城市2020年RPV碳减排总量（4BT），相当于电力热力行业碳排放量的近70%。这凸显了太阳能资源开发的一个重要方面，表明在双碳目标的背景下更多地利用建筑屋顶来开发分布式光伏系统；这对中国有帮助，因为中国可用于光伏安装的土地空间有限。其次，区域分析表明，大约 89% 的潜力位于人口稠密的东南部地区。这表明人口红利较高的东部城市可以率先通过部署光伏发电来实现发电基础设施脱碳。第三，对于人口稀少的西北城市来说，更适合集中式光伏发展。第四，对于煤炭依赖度较高的工业化程度较高的城市，发展光伏发电、加快新能源电力系统建设更为重要和必要。

我们的城市级评估从自上而下和自下而上的不同角度提供了碳减排量和强度的量化指标。这可以帮助地方政府、公司和个人确定适合快速部署 RPV 系统的位置并促进能源正义。该评估还提供了 RPV 潜力的深刻见解和详细数据集，可以改进碳中和情景的未来模型并为重要的国家能源政策奠定基础。这无疑有利于探索可持续、包容的低碳未来的可能性。

本研究的估算结果描绘了中国RPV系统理论上的最大碳减排潜力。在我们的主要分析中，结果基于35%的屋顶可用于安装RPV的假设。在目前的文献中，将屋顶总面积减少到可用屋顶面积通常是通过屋顶比例因子来实现的，屋顶比例因子表示由于方向、坡度和障碍物等导致的屋顶面积的损失。尽管目前使用的转换因子已经涵盖了以上各方面，是对全国平均情况的量化。城市级别的可用性可能会有所不同，为此我们进行了补充研究以提供更多了解（补充说明7和补充表15-17）。此外，我们还提供了RPV碳减排潜力的变化，作为屋顶可用性和电池板效率组合的不确定性分析。

值得注意的是，在以化石燃料发电为主的传统电力系统中，电力输出可以根据每小时、每周和季节性的负荷波动进行调整。然而，太阳能的可用性取决于天气条件，使得这种类型的能源缺乏灵活性。为了提高RPV未来的渗透率，未来的研究需要进一步探索如何提高RPV能源生产的灵活性。例如，将RPV与储能技术相结合，实现夜间持续供电，减轻电网压力。因此，可再生能源之间的互补是增强电网稳定性的另一个可能的解决方案。事实上，中国政府正在不断努力推进光伏系统未来的高效部署。目前中国大部分省份都在推行政策，光伏储能设施的配备比例不低于光伏装机容量的10%（部分城市甚至达到20%）。此外，越来越多的可再生能源试点正在建设中，探索光、风、水一体化的新模式。

经济因素是挖掘RPV技术潜力的另一个重要方面。尽管这项工作的范围不包括对城市规模经济可行性的详细评估，但现有文献提供了基本的理解。2020年，我国商业和工业DPPV系统初始投资成本为3.38 Yuan/W。全投资模式下DPPV系统的平准化能源成本（LCOE）在1800、1500、1200和1000等效利用小时时分别为0.17、0.20、0.26和0.31 Yuan/kWh。在没有补贴的情况下，中国所有344个城市的工商业DPV已实现100%用户侧平价上网，86% 城市的户用DPV已被证明具有经济可行性。此外，中国还实施了一系列大规模举措，系统部署光伏项目，以减轻农村地区的贫困。

尽管存在局限性和缺点，当前的研究为学者们提供了国家级数据集来支持未来的工作。未来的研究可以通过引入更全面的解释变量和更高分辨率的训练数据来提高屋顶面积预测的准确性，从而能够对RPV碳减排潜力进行更详细的国家级评估。为了更好地了解RPV系统未来可以提供的环境效益，对与实现其减排潜力相关的成本进行详细评估也很重要。特别是，光伏系统与城市基础设施的广泛整合对于太阳能资源开发的多样化至关重要，未来的研究可以考虑更多形式的光伏系统。