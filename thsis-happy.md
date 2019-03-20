myopic doer，短视者；
prefrontal cortex，前额皮层；limbic system，边缘系统
PRIVACY-PRESERVING DATA EXPLORATION SOFTWARE TOOLS | GENOME-WIDE ASSOCIATION ANALYSIS
#Enabling Privacy-Preserving GWASs in Heterogeneous Human Populations
time-consuming and burdensome application process
https://github.com/seanken/PrivSTRAT.git
http://bioinformatics.org.au/ws09/presentations/Day3_JStankovich.pdf（卡方检验p13~14）
“Human Genetic Variation” hailed as “Breakthrough of the Year” by
Science magazine in 2007
GWA studies have identified over 200 separate associations with
various complex diseases in the past two years（2009）

Linkage disequilibrium (LD) is the non-independence of alleles at
nearby markers in a population because of a lack of recombinations
between the markers
http://aryee.mgh.harvard.edu/BST227/Lectures/Lecture%205%20-%20Intro%20to%20GWAS.pdf
B and C are in LD
(big B never appears with little C)
cM=centimorgan
PLINK --logistic
gwas chi
#Deep Models Under the GAN: Information Leakage from Collaborative Deep Learning（44）

Our paper shows how unlabeled mass spectral data can be assigned peptide labels using prior models
and how new models can be trained from the generated labels. Such weak, pseudo and self labeling
strategies are not new to the area of machine learning
#Peptide-Spectra Matching from Weak Supervision
The use of deep learning models for mapping sequences to structured outputs
图1显示了用于蛋白质组学的蛋白质鉴定的常用管道的简化示意图，称为液相色谱 - 质谱（LC-MS）。来自复杂生物样品的蛋白质用生化技术分离，并根据其性质分离成不太复杂的混合物（图1a）。将这些蛋白质混合物消化成称为肽（1b）的片段，并根据其生化特性通过液相色谱法进一步分离。将肽单独（有希望地）注射到质谱仪中并片段化成较小的片段。然后测量这些片段的质荷比，以产生片段（1c）的相对强度的直方图。然后，现代LC-MS管道的目标是从这些直方图中推断出原始蛋白质群体
 turn the intensity measurements into a probability distribution by
normalizing the reading
represent the peptide as a sequence of L (possibly modified) amino acids,
x1 · · · xL.
# Differentially Private Matrix Factorization
differential privacy, a cryptographically motivated
definition of privacy
PPCA, randomly samples a k-dimensional subspace from a distribution that
ensures differential privacy and is biased towards high utility.
 matrix Bingham distribution
  Gibbs sampling is a popular Markov Chain Monte Carlo (MCMC) technique in
which samples are generated according to a Markov chain whose stationary distribution is the
density in
#Near-Optimal Algorithms for Differentially-Private Principal Components
- rstiefel R package（Simulation of the matrix Bingham-von Mises-Fisher distribution,
with applications to multivariate and relational data）

- translate the problem of assessing the association between a large number
of variables（gene） and multiple outcomes（pheno） into the statistical problem of simultaneous testing of columns of high-dimensional cross-covariance matrices
GWAS的一个重要目标是探索对复杂疾病的遗传易感性。这些研究已经识别出多种疾病的易感性等位基因所在的相关基因组区域。但GWAS的一个局限在于只关注预先定义好的有限表型域。解决这个问题的一种替代方案是PheWAS，PheWAS研究基因组标记与多种表型之间的关联。像GWAS一样，PheWAS可以发现对某种性状起作用的多个遗传标记。除此之外，PheWAS还能够发现基因组标记对多种性状的作用，从而可以更全面地了解遗传变异与表型网络之间的关系。
multiple testing of the columns of a high-dimensional cross-covariance matrix
- the construction of suitable test statistics for individual hypotheses and establishing the null distribution of these test statistics
- the construction of a good procedure to account for the multiplicity of the tests so that the overall FDR is controlled under dependency
周傲英数据管理与信息系统‚包括：Web数据管理、中文Web基础设施、Web搜索与挖掘；数据流与数据挖掘、复杂事件处理与实时商务智能、不确定数据管理及其应用；数据密集的计算、分布存储与计算、对等计算系统及其数据管理、Web服务计算
薛向阳
金枝software engineering, requirements Engineering, knowledge engineering, and machine learning



we introduce a clustering based approach,
in which we adopt a novel clustering criterion, validation error minimization,
to ensure that the found models are unique and precise. We propose a twostep
algorithm, which uses enhanced dynamic programming and Expectation
Maximization (EM) like methods for clustering.

- 1. Sequential Clustering. Partition the data stream into a number of contiguous
data segments. Each of those data segments, called a section, corresponds
to an occurrence of a model;
- 2. Iterative Clustering. Cluster the sections based on their characteristics (implying
the models they represent). Each of the resulting cluster corresponds
to a unique hidden model.



 custody battle 监护权之争
遗传隐私是指在存储，再利用，以及向第三方提供，显示遗传信息时个人隐私的权利。新技术的出现简化了人类基因组的高通量，低成本测序，但同时也对未来医疗保健提出了重要伦理问题。例如已经有研究指出，可以仅通过匿名基因组学研究参与者的DNA识别他们的身份，这些身份信息与基因组中的疾病易感性信息结合起来构成严重的隐私泄露。而且由于遗传数据自身的特点，不仅参与者本人的隐私信息会被泄露，参与者的亲属的隐私也会随之以不同程度的泄露。

要求个人做出知情同意
## DNA加密
DNA加密是在DNA测序过程中为了保护遗传隐私用计算的方法隐藏或混淆遗传信息的过程。人类基因组既长又复杂，但可以从少量的变异中找到重要的有识别作用的信息。整个人类基因组有32亿碱基对，但个体与个体之间只有0.5%的遗传变异。新兴策略采用不同的方法，如随机化算法和加密方法来去除个体中遗传序列识别个体信息，只保留必要的信息。现在的优先事项是确定哪些方法是健全的，以及政策应如何确保持续保护遗传隐私。

2003年，国家人类基因组研究所及其附属合作伙伴成功测序了第一个完整的人类基因组，这个项目耗资不到30亿美元。[2]四年后，詹姆斯·沃森（James Watson） -  DNA结构的共同发现者之一 - 能够以不到150万美元的价格对他的基因组进行测序。[3]随着基因测序技术的迅速发展，精简调整以适应临床手段，现在可以以更低的成本提供对个体遗传身份的难以置信的洞察力，生物技术竞争者争夺1000美元基因组的称号。[4]遗传物质现在可以从人的唾液，头发，皮肤，血液或其他来源中提取，测序，数字化，储存和用于多种目的。每当数据被数字化和存储时，就有可能发生隐私泄露。[5]虽然现代全基因组测序技术允许前所未有地获取和理解人类基因组，并激发个性化医疗的潜力，但它也引发了道德和隐私风险。

基因测序是产生关于疾病起源，疾病预防和开发有意义的治疗干预的科学知识的首要步骤。许多研究利用大型DNA样本或聚合全基因组数据集来识别与特定疾病或表型相关的基因;因此，对于限制基因组数据库的可访问性还是加强对大规模研究的大力支持存在很大的分歧。例如，如果要对所有遗传学研究实施知情同意条款，则现有遗传数据库不能重新用于新研究 - 所有数据集都需要在每项研究结束时销毁，或者所有参与者需要对每项新研究的权限重新进行授权。[1]由于遗传数据集可以外推到密切相关的家庭成员，这增加了研究过程中所需同意的另一个维度。这从根本上提出了这些限制是否是必要的隐私保护还是阻碍科学进步的问题。

基因测序已经加速了单基因疾病的预后咨询，这需要在新生儿护理中进行快速，鉴别的诊断。[6]然而，医疗使用和研究使用之间经常模糊的区别可能会使这两个领域之间的隐私得到处理变得复杂，因为它们通常需要不同级别的同意并利用不同的政策。


在消费者市场上，人们纷纷涌向Ancestry.com和23andMe，以发现他们的遗产并阐明他们的基因型。由于消费者交易的性质允许这些电子点击包装模型绕过研究和医疗保健中的传统形式的同意，消费者可能无法完全理解将其基因序列数字化和存储的含义。此外，企业隐私政策通常在联邦管辖范围之外运作，使消费者面临信息风险，包括其遗传隐私和自我披露的消费者档案，包括自我披露的家族史，健康状况，种族，民族，社会网络等等。[7]简单地拥有数据库会带来潜在的隐私风险，因为数据存储本身就存在数据泄露和政府征求数据集的可能性。 23andMe已收到联邦调查局（FBI）提出的访问消费者数据集的四项请求，虽然这些请求被拒绝，但这显示出与FBI-Apple加密争议类似的难题。

美国的2008年遗传信息非歧视法案（GINA）;然而，在许多情况下，正式立法的范围和责任是相当不确定的，因为科学似乎正在以比法律更快的速度进行，专业伦理委员会必须填补这一必要的利基。[1]许多批评都针对政策从根本上缺乏对基因组测序中涉及的技术问题的理解，并且没有解决如何在数据泄露的情况下，个人的个人基因组无法被替换，进一步使隐私保护复杂化。

在世界各地，每个国家都有独特的医疗保健和研究框架，产生不同的政策需求 - 在考虑国际基因研究或国际生物库，存储生物样本和DNA信息的数据库时，遗传隐私政策更加复杂。此外，研究和医疗保健并不是唯一需要正式管辖的领域;其他关注领域包括刑事司法系统中的人的遗传隐私以及参与基于私人消费者的基因组测序的人。


全球最大的法医DNA数据库中有91％是国家刑事情报DNA数据库（NDNAD），其中包含来自英格兰和威尔士居民的DNA信息。[10] NDNAD存储犯罪被定罪个人的遗传信息，那些被指控但无罪释放可记录犯罪的人，被捕但从未被控犯有可记录犯罪的人，以及受到反恐控制的人。在数据库中的550万人中，占总人口的10％，其中120万人从未被定罪。[10]在S和Marper诉联合王国案（2008年）的案件中，欧洲人权法院决定政府必须提出足够的理由来对刑事司法系统中人的DNA概况进行差别处理，而不是与未定罪的个人相比。 ;基本上，不得滥用保留的生物材料和DNA信息。[10]该决定强调了当前系统存在的若干问题，这些问题给所涉及的个人带来隐私风险：利用遗传信息存储个人信息，存储具有确定遗传关系的固有能力的DNA概况，以及从根本上说，存储的行为。细胞样本和DNA谱为隐私风险带来了机会。因此，建立了“2012年自由保护法”，以确保正确使用收集的DNA材料并规范其储存和销毁。[10]然而，许多问题仍然存在，因为样本仍然可以无限期地保留在数据库中，无论受影响的个人是否被定罪 - 甚至是少年犯的样本。批评者认为，这种长期保留可能导致受影响个人受到侮辱，并抑制他们重新融入社会，并且还会受到刑事司法系统固有的歧视行为的滥用。[10]


1990年，德国联邦最高法院和德国联邦宪法法院裁定，“德国刑事诉讼法”的各个部分为使用遗传指纹识别识别罪犯和赦免无辜者提供了合理的法律依据。[10]然而，这些决定缺乏关于如何获得生物材料以及如何利用遗传指纹的具体细节;仅明确概述了血液检查和体检的规定。 1998年，德国议会批准建立国家DNA数据库，因为压力越来越大，以防止涉及儿童的性虐待和杀人案件。[10]尽管有人批评信息自决的权利受到了侵犯，但这一决定在2001年被联邦宪法法院的公共利益所支持为宪法和支持。法院确实要求DNA信息和样本必须得到个人可以在未来犯下类似罪行的证据的支持。为解决法律上的不确定性，2005年“法医DNA分析法”引入了一些条款，其中包括在刑事诉讼中使用基于DNA的信息的确切和有限的法律依据。[10]一些部门命令只有在加速调查，消除嫌疑人和法院必须下令遗传指纹识别所必需的DNA样本时才可以使用。自实施以来，每月新增8000套新数据库，这使人们对这种大规模数据收集的必要性以及条款措辞是否提供有效的隐私保护产生了疑问。[10]德国政府最近的一项有争议的决定扩大了DNA拉网的家族搜索范围，以确定性暴力和暴力犯罪者的遗传亲属 - 这一行动之前被德国联邦最高法院认为在2012年没有法律依据。[10 ]

韩国国家法医服务局和韩国检察机关于1991年建立了独立的DNA分析部门，尽管最初公开批评数据收集是在没有考虑所涉及主题的信息隐私的情况下制定的，批评转向支持一系列备受瞩目的案件。[10] 2006年，大会关于DNA信息收集和运作的拟议法案概述了用于存储，控制和销毁DNA样本和DNA信息的犯罪类别。但是，该法案未能通过，因为它无法转化为实际做法中的任何重大变化。所包含的不全面的犯罪类别仅适用于在未经个人同意的情况下获取生物信息，并且销毁所收集样本的协议不明确，使其被滥用。[10] 2009年DNA信息法试图解决这些弱点，包括规定生物敏感信息只能从被定罪的个人，受限制的嫌疑人和犯罪现场收集的规定。遗传指纹识别是针对特定罪行而允许的，包括纵火，谋杀，绑架，强奸或性骚扰，夜间盗窃，盗窃和入室盗窃以及许多其他暴力犯罪。[10]如果有关人员未书面同意，该法案还要求从被定罪的罪犯或嫌疑人那里获取样本的书面保证书。如果有关个人被宣告无罪，无罪释放，他们的起诉被驳回，并且在他们去世时，所有样本必须及时销毁。[10]重要的是，如果收集的样本用于确定犯罪现场的个人，则必须在成功识别后销毁DNA信息。然而，在澄清无罪推定，相当琐碎的样本破坏执法方面，对这项立法仍存在若干瑕疵和批评。

在美国，生物库主要受健康保险流通与责任法案（HIPAA）隐私规则和联邦保护人类受试者政策（共同规则）的管辖。由于这些规则都不是为了规范生物库和分散的监管水平而设想的，因此在应用和执行方面存在许多挑战，联邦法律未能直接解决国际政策以及如何在欧盟以外共享数据 - 美国安全港协议。[11]需要澄清的一个领域是联邦和州法律如何区别地和具体地应用于不同的生物库，研究人员或项目，这种情况由于大多数生物银行是大型实体的一部分，或与其他机构合作，使情况更加复杂化。符合公共和私人利益。大约80％的生物银行都有内部监督委员会，负责监管数据的收集，使用和分发。应用于生物样本样本和数据的可访问性有三种基本访问模型：开放访问（不受任何人限制），分层访问（访问的某些限制取决于项目的性质），或受控访问（严格控制访问）。[ 11] GINA规定禁止健康保险公司要求进行基因检测或为登记目的请求遗传信息，并禁止雇主为任何类型的就业评估（招聘，晋升，终止）申请基因检测或遗传信息。但是，保险公司可以要求遗传信息来确定特定程序的覆盖范围。一些团体也被排除在遵循GINA的规定之外，包括联邦政府雇员，军队和雇员少于15人的雇主的保险公司和雇主。[12]

中国拥有广泛的医院和研究机构网络。目前正在制定一项计划，为现有生物库之间的数据共享创建一个更具凝聚力的框架，该框架以前处于重叠和混乱的监管法律的管辖范围之内。许多生物银行独立运营，或在其他网络的网络内运营，其中最突出的是上海生物银行网络。[13]在这个主要网络下，指南详细说明了具体的去识别政策，并明确表示赞同广泛的同意。最近，中国宪法正式承认个人隐私是一项独立和独立的宪法权利，因此，立法者已经开始制定人类遗传资源条例草案，以组织有关生物银行管理措施，法律责任和违法行为处罚的国家法律。根据这些联邦法律，国际数据共享将受到更严格的监管。[13


隐私权倡导者电子前沿基金会发现，现有立法对确保涉及DNA信息的消费者隐私没有正式管辖权。消费者企业存储的遗传信息不受HIPAA保护;因此，这些公司可以与第三方共享遗传信息，条件取决于他们自己的隐私声明。[15]大多数基因检测公司仅在用户同意的情况下共享匿名的汇总数据。 Ancestry.com和23andMe确实将这些数据出售给研究机构和其他组织，并可以要求逐案同意将非匿名数据发布给其他方，包括雇主或保险公司。 23andMe甚至发出警告，重新识别可能发生并且是可能的。如果消费者明确拒绝研究使用或要求销毁他们的数据，23andMe仍然可以使用他们的消费者识别和行为信息，例如浏览模式和地理位置，用于其他营销服务。[15]

许多计算专家已经开发并正在开发更安全的基因组测序系统，以保护该领域的未来免受错误的管辖，遗传数据的错误应用，以及最重要的是个人的遗传隐私。目前有四个主要的遗传学研究领域正在开发隐私保护技术：

字符串搜索和比较
亲子鉴定，遗传兼容性测试和血统测试是依赖于字符串搜索和比较算法的所有类型的医疗工具。[1]简单地说，这是一种大海捞针方法，在其中搜索数据集以寻找匹配的“字符串”，即感兴趣的序列或模式。随着这些类型的测试变得越来越普遍，并且适应消费者基因组模型，例如智能手机应用程序或时尚DNA测试，当前的隐私保护方法专注于强化该过程并保护医疗保健和私人使用。

聚合数据发布
 现代化的大数据和大规模基因组测试需要处理系统，以便在发布聚合基因组数据时最大限度地降低隐私风险，这实质上意味着确保在基因组数据库中无法识别个体数据。[1]这种差异隐私方法是对基因组数据库安全性的简单评估，许多研究人员对现有基础设施的严格性进行“检查”

 原始基因组数据的比对
 基因组学领域最重要的发展之一是读取映射的能力，其中数百万个短序列可以与参考DNA序列比对，以便有效地处理大数据集。由于这种高容量流程通常在公共和私人计算环境之间划分，因此存在许多相关的风险和阶段，其中遗传隐私特别容易受到攻击;因此，目前的研究重点是如何在不牺牲效率和准确性的情况下在两个不同的数据域内提供安全操作。[1]

 安全基因组查询
个性化医疗和预防性医疗保健的基础是通过比较个体基因组与已知变异来估计对疾病（如乳腺癌或糖尿病）的易感性来评估药物基因组学，以及查询个体之间的生物关系，从而建立基因兼容性。[5]对于疾病风险测试，研究提出了一种隐私保护技术，该技术利用同态加密和安全整数比较，并建议以加密形式存储和处理敏感数据。为了确保隐私，存储和处理单元（SPU）将所有单核苷酸多态性（SNP）存储为真实SNP  - 患者中观察到的SNP  - 具有来自潜在SNP集的冗余内容。[18] [19]另一种解决方案开发了三种协议，使用Yao的乱码电路和带状对齐算法的交叉点来确保计算编辑距离。该解决方案的主要缺点是无法在保持准确性的同时执行大规模计算。[20]

安全的全基因组关联
 研究全基因组关联研究（GWAS）对于确定导致疾病的基因组序列的特定变异非常重要。识别与疾病显着相关的SNP的隐私保护算法基于引入随机噪声来汇总统计数据以保护个人隐私。[21]在另一项研究中，连锁不平衡的性质被用于选择最有用的数据集，同时通过注入噪声最大化保护患者隐私;然而，它可能缺乏有效的疾病关联能力。[22]这些方法的批评者指出，需要大量的噪声来满足小比例SNP的差异隐私，这是进行有效研究的不切实际的方法。[5]

 经过验证的加密存储
 基于多个预期符号，基因组序列的性质需要特定的加密工具来防止低复杂性（重复内容）攻击和KPA（Known-plaintext_attack）。 Cryfa [23]使用打包（减少存储），改组机制（随机化符号位置）和AES密码（Advanced_Encryption_Standard）来安全地存储带有经过身份验证的加密的SAM文件。











# Quantifying Interdependent Risks in Genomic Privacy

 人类基因组测序的快速进展正在导致基因组数据的高可用性。众所周知，这些数据在时间上非常敏感和稳定，并且亲属之间高度相关。在本文中，我们研究了这些家族相关性对亲属基因组隐私的影响。我们基于图形模型和信念传播将问题和详细的有效重建攻击形式化。通过我们的方法，攻击者可以通过显着依赖孟德尔定律，基因组变体之间以及基因组和表型之间的统计关系来推断观察基因组或表型的个体的亲属的基因组。我们根据观察到的变体数量和分享它们的亲属评估这些依赖关系对隐私的影响。我们还研究了在考虑这些不同关系时算法性能如何演变。此外，为了量化由于所提出的推理攻击而导致的基因组隐私水平，我们讨论了基因组隐私度量的可能定义，并比较了它们的价值和进化。基因组数据显示孟德尔疾病和发生严重疾病的可能性，如阿尔茨海默氏症。我们还介绍了健康隐私的量化，特别是对攻击者隐藏疾病易感性程度的衡量标准。我们从谱系评估我们对实际基因组数据的方法，并通过结合从基因组共享网站和在线社交网络收集的数据来显示威胁程度。

 基因组共享网站和在线社交网络收集的数据

 由于分子谱分析的成本急剧下降，生物医学研究人员可以获得越来越多的基因组数据，这是实现更个性化，精确和预测性医疗的关键推动因素。
 由于可用基因组数据的不断增加而产生的一个主要问题是隐私。
 由于基因组数据的不断增加而产生的一个主要问题是隐私。首先，已经证明，即使基因组数据是匿名的，也可以通过各种方式重新识别它们的所有者[Gymrek et al。 2013; Humbert等人。 2015B; Sweeney等人。 2013。其次，越来越多的人在线共享他们的基因组，有时还有他们的真实标识符（例如，在OpenSNP.org上[Greshake等人，2014]）。获取此类敏感数据可能导致在获得保险和就业方面的歧视[Ayday等。 2015年]。

 家庭成员的基因组数据高度相关，导致相互依赖的隐私风险，这些问题更加严重。这些风险已经被Lacks家族的故事所宣传.1然而，鉴于基因组数据共享的趋势，Lacks家族到目前为止并不是唯一一个隐私受到这些相互依赖的风险威胁的家庭。我们通过使用OSN作为收集家庭信息的辅助渠道来显示这种威胁的程度[Humbert et al。 2013。

 在这项工作中，我们量化了基因组隐私中家族相关性产生的相互依赖的风险。关注人群中最常见的变异，单核苷酸多态性（SNP），并考虑到基因组内的统计相关性（称为连锁不平衡），我们量化了一个或多个家庭成员的个体基因组隐私损失。基因组（部分或全部）显露出来。为了实现这一目标，我们设计了有效的推理算法来模拟对抗性重建攻击。我们提出了贝叶斯网络模型，该模型考虑了亲属基因组之间以及基因组和表型之间的统计关系。我们进一步将该模型扩展到因子图表示，以便将基因组内相关性包括在我们的模型中。为了在线性复杂度中推断未知SNP的值，我们使用置信传播算法，在结树（在贝叶斯网络的转换中移除其环）上运行，或在因子图上运行。在后一种情况下，因子图包含循环;算法多次执行，直到概率分布收敛到稳定状态。然后，使用各种指标，我们量化个体的基因组隐私，并显示其家族成员的已发表基因组导致的基因组隐私水平的降低。我们还根据当前的医学知识量化个体对某些严重疾病的（遗传）倾向的健康隐私。我们通过使用谱系的真实基因组数据来评估所提出的推理攻击并显示其效率和准确性。更重要的是，通过使用从基因组共享网站和OSN收集的基因组和表型数据和谱系信息，我们发现推理攻击不会仅威胁到Lacks家族


本文是我们论文的修订版和扩展版[Humbert et al。 2013]，并包含以下额外贡献： - 我们提出了推理攻击的新框架，该框架仅考虑家庭成员之间的基因组相关性。我们证明了这个新框架能够在我们的置信传播算法的单次迭代中实现精确推理。我们还包括其计算复杂性的分析和经验评估。 - 我们在这个新框架中添加了一个新图层，可以将有关亲属表型的其他信息考虑在内，以改善推理攻击。

- 我们通过几个新的实验来更新推理攻击的结果。 - 我们彻底评估各种指标之间的关系，并在不同的设置中得出关于最合适的指标的结论。 - 我们利用OpenSNP用户公开的表型信息结合基因组数据进行新的实验。 - 我们包括性能评估，以及关于所提议的推理攻击的潜在改进的讨论。

2.背景在本节中，我们简要介绍相关的遗传原理，以及一些有效建模数据依赖和运行推理的重要工具。 2.1。基因组学101 DNA是双螺旋结构，由两条互补的聚合物链组成。遗传信息在DNA上编码为核苷酸序列（A，T，G，C）;人类DNA包括大约30亿个核苷酸对。随着DNA测序成本的降低，基因组数据目前主要用于以下两个方面：（i）临床诊断，个性化基因组医学和遗传研究（如全基因组关联研究），以及（ii）直接到 - 消费者基因组学，用于各种疾病的遗传风险评估或用于诸如祖先搜索的娱乐活动。在下文中，我们将简要介绍我们在本文中使用的有关人类基因组和繁殖的一些概念。

2.1.1。单核苷酸多态性。人类共有99.9％的DNA。因此，不需要关注整个DNA结构，而是关注变体。 SNP是人群中最常见的DNA变异。当核苷酸（在DNA上的特定位置）在给定群体的个体之间变化时发生SNP（如图1所示）。人群中大约有5000万个SNP位置.2最近的发现表明，个体对几种疾病的易感性可以从个体的SNP中计算出来[Johnson and O'Donnell 2009]。例如，据报道，载脂蛋白E（ApoE）基因上的两个特定SNP（rs7412和rs429358）表明阿尔茨海默病的风险增加（增加）。 SNP携带有关个人健康的隐私敏感信息;因此，我们将量化健康隐私，重点关注个人发布（或推断）的SNP及其揭示的疾病。

通常可以在给定的SNP位置观察到两种不同的核苷酸（称为等位基因）:( i）主要等位基因是最常观察到的核苷酸，（ii）次要等位基因是稀有核苷酸.3对于每个SNP位置，我们代表主要等位基因为B，次要等位基因为b（其中B和b均在{A，T，G，C}中）。

  此外，每个SNP位置包含两个核苷酸（一个遗传自母亲，一个来自父亲，我们将在下面讨论）。因此，SNP位置的含量可以处于以下状态之一：（i）BB（纯合 - 主要基因型），如果个体从父母双方接收相同的主要等位基因; （ii）Bb（杂合基因型），如果个体从每个父母（一个小的和一个主要的）接受不同的等位基因;或者（iii）bb（纯合子 - 次要基因型），如果个体从父母双方继承相同的次要等位基因。为了简化表示，在本文的其余部分，我们将BB编码为0，Bb编码为1，bb编码为2.最后，每个SNP gi分配一个次要等位基因频率（MAF），pi maf，表示频率，相应SNP的次要等位基因b发生在给定群体中（通常，0 <pi maf <0.5）。

  2.1.2。再生产。孟德尔的第一定律指出，等位基因从父母独立传递给儿童以获得不同的减数分裂（生殖所必需的细胞分裂过程）。对于每个SNP位置，一个孩子从母亲那里继承一个等位基因，从父亲那里继承一个等位基因，如图1所示。父母的每个等位基因被传递给一个等概率为0.5的孩子。设FR（Xi M，Xi F，Xi C）是建模SNP gi的孟德尔遗传的函数，其中M，F和C分别代表母亲，父亲和孩子。我们在表I中说明了孟德尔遗传概率。基于FR（Xi M，Xi F，Xi C），我们可以说，鉴于父母的基因组，儿童的基因组在条件上独立于所有其他祖先的基因组。

  2.1.3。联系不平衡。如前所述，DNA序列在近亲之间高度相关，但DNA中不同SNP之间也存在相关性。连锁不平衡（LD）[Falconer和Mackay 1996]定义了由于群体的遗传历史而在整个基因组中的任何一对SNP之间出现的相关性。由于LD，可以从其他SNP的内容推断出SNP的含量。例如，假设gi和gj彼此在LD中。设（A1，A2）和（B1，B2）分别是SNP gi和gj的潜在等位基因。此外，令（p1，p2）和（q1，q2）分别是由群体统计提供的（A1，A2）和（B1，B2）的等位基因概率。也就是说，给定群体中的个体在SNP gi处具有等位基因A1的概率是p1，等等。如果没有LD（即，如果gi和gj是独立的），则个体在gi和gj处同时具有A1和B1的概率将是p1q1。然而，由于gi和gj之间的相关性，该概率实际上等于p1q1 + D，其中D表示在两个SNP之间的独立假设下计算的概率与给定群体中的概率之间的差异。在表II中，我们说明了（A1，A2）和（B1，B2）的所有可能组合的LD关系。我们注意到D可以是负数或正数，具体取决于LD值。捕获LD的另一个相关度量是相关系数r，表示为r = D /√p1p2q1q2，其中r = 1表示最强的LD关系。



2.2。概率推理在本节中，我们将介绍构成有效推理方法基础的数学模型和算法。 2.2.1。概率图模型。概率图形模型是表示随机变量之间依赖关系的非常合适的模型[Koller和Friedman 2009]。这种基于图的模型可以表达条件依赖性（例如，贝叶斯网络），联合依赖性（例如，马尔可夫随机字段）或两者（例如，链图）。在图形模型中，每个节点表示一个随机变量，箭头表示它们之间的依赖关系。这些模型对于表示大量随机变量的联合分布的因式分解非常有用，然后显着降低了例如边际概率的计算的复杂性。如果图形模型包含循环或循环，则可以通过将变量聚类到单个节点（称为cliques）和构建最大生成树（称为联合或clique树[Jensen和Jensen 1994]）来消除这些。可以表示有向图和无向图的更通用的模型是因子图。与结点树相反，它使得能够在精确推断在计算上难以处理的情况下找到近似解。因子图是一个二分图，其中一组顶点表示随机变量，另一组表示（局部）函数，它们考虑（全局）联合概率函数（基于变量之间的依赖关系）。当且仅当变量是对应于因子节点的本地函数的参数时，变量节点才连接到因子节点。

2.2.2。信仰传播。信念传播[Pearl 1988]是一种用于对图形模型进行推理的消息传递算法。它也被称为sumproduct算法[Kschischang等。 2001]。它通常用于计算以观察到的变量为条件的未观测变量的边际分布。计算边际分布通常很难，因为它可能需要对指数大量的项进行求和。置信传播算法适用于各种类型的图形模型，例如贝叶斯网络或马尔可夫随机场。如果底层图形模型不包含（定向或无向）循环，则置信传播算法会导致精确推断，即给定观察变量的精确后验边际概率。如果图形模型不是树或多树（不是无周期），我们可以将其转换为连接树，然后在其上运行置信传播并获得精确解或执行循环信念传播，从而得出近似解[墨菲等人。 1999年]。当结点树方法在计算上难以处理时，通常使用第二种方法，并且通常给出良好的近似结果。信念传播通常用于人工智能和信息理论。它已在许多应用中证明了经验上的成功，包括LDPC码[Pishro-Nik和Fekri 2004]，声誉管理[Ayday和Fekri 2012a，2012b]和推荐系统[Ayday et al。 2012]。因子图是图形模型的最通用表示，我们将解释它们上的通用置信传播算法。我们假设联合分布g（x1，...，xn）因子成为几个局部函数的乘积，或因素，fa（xa）：

其中A是离散索引集（因子节点），xa是{x1，...，xn}的子集，表示连接到因子节点a的变量节点集。信念传播算法只需在| A |之间传递消息即可因子节点（表示因子f1（x1）到f | A |（x | A |））和二元因子图上的n个变量节点（表示随机变量x1到xn）。从因子节点a到变量节点i的消息ma→i（xi）可以被解释为关于i基于函数fa处于其不同状态的相对概率的陈述。从变量节点i到因子节点a的消息ni→a（xi）可以被解释为关于节点i基于除了基于该函数的信息节点之外的所有信息节点处于不同状态的相对概率的陈述。 F A。消息根据以下规则更新[Pearl 1988; Kschischang等。 2001年]：

3.2。对手模型对手由对手的目标，能力和知识来定义。攻击者的目标是通过使用（i）一个或多个家庭成员的可用基因组数据，（ii）家庭成员之间的家庭关系来计算目标家庭的一个或多个成员的目标SNP的值， （iii）繁殖规则（第2.1.2节），（iv）核苷酸的MAF，和（v）SNP之间的群体LD值。我们注意到（i）和（ii）可以从基因组共享网站和OSN在线收集，并且（iii），（iv）和（v）是公知的信息。请注意，将来，在二倍体基因组的每个拷贝中准确测序和推测个体携带的实际单倍型的可能性越来越大，这将允许更准确地推断亲属的基因型而不仅仅依赖于种群LD模式。 。根据对手的兴趣，可以发起各种攻击。对手可能想通过观察一个或多个其他亲属来推断特定个体的一个特定SNP（目标-SNP靶向相对攻击）或目标家族中多个亲属的一个特定SNP（目标-SNP-多亲属攻击） SNP处于同一位置。此外，对手可能还想通过观察不同位置的SNP来推断同一个体的多个SNP（多个SNP靶向相对攻击）或多个家族成员的多个SNP（多个SNP多个亲属攻击）。亲戚们。本文中介绍的统计推断模型适用于所有这些攻击。

基因组数据包含许多关于其所有者的敏感信息，例如他对敏感疾病的倾向，祖先，物理属性和亲属的基因组数据（导致相互依赖的隐私风险）。个人在网上共享大量信息，其中一些信息可用于推断其基因组数据。因此，需要清楚地了解考虑网上公开可用信息的个体基因组数据的隐私风险。在不损害研究和医疗保健中基因组数据利用的同时保护个体的基因组隐私也至关重要。该项目的两个主要目标是：（i）开发一个新的统一框架，用于量化个体的基因组隐私;（ii）建立一个完整的框架，用于保护现实生活中基因组数据的隐私保护利用，共享和验证威胁模型。https://cordis.europa.eu/project/rcn/203068_en.html

A message from or to a variable vertex is always a function of that particular variable.

# Simulating the Large-Scale Erosion of Genomic Privacy Over Time

迄今为止，DNA测序的成本急剧下降已经引发了超过一百万人的基因型测序。此外，这些人越来越多地公开他们的基因组数据，从而不仅为他们自己创造了独特的隐私威胁，而且由于他们的DNA相似性也为他们的亲属创造了独特的隐私威胁。更一般地，获得对来自给定群体的大部分测序基因型的访问的实体可能能够通过依赖于可用数据来推断甚至未测序个体的基因组。在本文中，我们提出了一个基于模拟的模型，用于量化连续测序和公布个人基因组数据对群体基因组隐私的影响。我们的模拟概率地模拟了个体的数据共享，并且还考虑了地理政治事件（如移民）和跨种族婚姻等社会学趋势对基因组隐私的影响。我们示例性地使用1,000个个体的样本群体来实例化我们的模拟，并且评估在数千个基因组变体或影响表型的变体的子集的不同设置下的隐私的演变。我们的研究结果显示，未来基因组数据的共享率越来越高，对所有老一代人的隐私产生了实质性的负面影响。此外，我们发现混合种群由于其较大的基因组多样性，与较均一的种群相比，随着时间的推移，基因组隐私的侵蚀程度较低。然而，即使没有共享数据，在大量变体上平均的基因组隐私已经非常低，因为仅仅群体等位基因频率已经揭示了关于基因组变体的值的许多信息。通过关注敏感变异的子集，我们观察到群体中更高的遗传多样性。因此，基因组数据共享对于最敏感的变体的隐私可能更加有害

 interracial mating
 Pleotropic effects 多向作用





# De-anonymizing Genomic Databases Using Phenotypic Traits

#Bayesian pedigree inference with small numbers of single nucleotide polymorphisms via a factor-graph representation


重新识别可能是传播和分析人类基因组数据时最广泛研究的隐私风险。在这种攻击中，未经授权的一方查看已经受到某种保护的已发布的人类基因组，以隐藏其捐赠者（例如，患者）的身份信息，并试图恢复所涉及的个体的身份。这种攻击一旦成功，就会对这些捐助者造成严重损害，例如歧视和经济损失。在本节中，我们将回顾现有隐私保护技术中存在的使这种类型的攻击成为可能的弱点。

伪匿名数据。广泛使用的用于保护健康信息的方法是去除显式和准识别属性（例如，姓名和出生日期）。此类修订符合法律要求，以保护传统健康记录的隐私（例如，根据美国健康保险流通与责任法案取消识别）。然而，仅通过去除识别信息不能使基因组数据匿名化。对手总是有风险推断DNA材料供体的表型（即，人的可观察特征，例如眼睛/毛发/皮肤颜色），这将导致供体从基因型（遗传构成）中识别。尽管用于此目的的技术仍然不成熟，但基因组研究和技术的快速发展正在迅速推动我们走向这一目标。此外，通过检查公布的DNA序列附带的背景信息，可以实现重新鉴定[Gitschier 2009; Gymrek等。 2013;海登2013]。例如，Y染色体上的基因组变体与姓氏（男性）相关，可以使用公共生物学数据库找到。其他情况包括通过公共人口统计数据识别个人基因组计划（PGP）参与者[Sweeney等。 2013年，使用公共信息（例如，死亡通知）[Malin 2006]和其他相关攻击[Malin和Sweeney 2004]，从1000基因组计划发布的数据中恢复家庭成员的身份。已经表明，即使是加密安全协议，当用于基因组数据时也会泄漏大量信息[Goodrich 2009]。