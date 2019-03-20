# Interactive network visualization in Jupyter notebooks: visJS2jupyter
elucidate,阐发;Autism,自闭症；Candidate-gene screening，基因筛选；sequence alignment，序列比对，overhead ，开销;whole exome sequencing (WES),全外显子组测序；breast invasive carcinoma dataset ，乳腺浸润癌数据集;exon, 外显子；vertebrate，脊椎动物；Escherichia coli ，大肠杆菌；dyspepsia，消化不良；Gastroenterology，胃肠病学；proton pump inhibitors (PPIs)，质子泵抑制剂；peptic ulcer，消化性溃疡；

 on par with ，与...相当；gene promoter ，启动子；
 A genomic window is defined as a CpG island if its GC content>50% and observed-to-expected CG ratio>0.6.
下载基因组注释gtf文件和下载参考基因组序列
https://blog.csdn.net/herokoking/article/details/78292616
CryptoNets  ML Confidential
(\(pt\))
An Introduction to Homomorphic Encryption
for Statistics and Machine Learning
Systematizing Genome Privacy Research:
A Privacy-Enhancing Technologies Perspective
#Privacy-Preserving Processing of Raw Genomic Data DNA encryption
然后对每个读数进行生物信息学处理并定位（比对）其遗传位置
短读的隐私敏感领域是（i）其相对于参考基因组的位置，（ii）其雪茄串（CS），以及（iii）其内容（包括来自{A，T，G的核苷酸， C}）

如果患者携带导致患病细胞（例如癌症）发生特定变异的疾病，则其健康细胞中的DNA序列将与患病的细胞不同。通过仅查看患者的变体调用（而不是他的短读数），可以将这些变化错误地分类为测序错误。
我们假设SAM文件使用假名存储在生物库中;这样，生物库就无法将进行基因测试和进行这些测试的医疗单位（MU）与患者的真实身份联系起来。
Geneticists prefer to store patients’ aligned, raw genomic data, in addition to their variant calls (compact and summarized form of the raw data)
storing the SAM files at a biobank
the storage of the cryptographic keys (of the patients) to
the MK
MU（medical unit）
we use OPE instead of private information retrieval (PIR), searchable encryption , or oblivious RAM (O-RAM) storage techniques for the **privacy preserving retrieval of the short reads**
- the short reads are randomly sampled from the genomes of the patients, and hence the positions of the short reads vary in each patient’s genome
-  implementations of O-RAM introduce high storage overhead to both the client (MU) and the server (biobank)

Furthermore, it is not desirable for the biobank to learn the requested range of nucleotides (as the biobank can infer the nature of the genetic test from this requested range).
The proposed scheme provides the short reads that include the requested range of nucleotides to the MU without revealing the positions of these short reads to the biobank
#HEALER: Homomorphic computation of ExAct
Logistic rEgRession for secure rare disease
variants analysis in GWAS
#Ruichu Cai, Zhifeng Hao, Marianne Winslett, Xiaokui Xiao, Yin Yang, Zhenjie Zhang, Shuigeng Zhou; Deterministic identification of specific individuals from GWAS results
# The Single Nucleotide Polymorphism Database (dbSNP) of Nucleotide Sequence Variation

- The Single Nucleotide Polymorphism database (dbSNP) is a public-domain archive for a broad collection of simple genetic polymorphisms
  - single-base nucleotide substitutions (also known as single nucleotide polymorphisms or SNPs)
  -  small-scale multi-base deletions or insertions (also called deletion insertion polymorphisms or DIPs)
  - retroposable（可重组） element insertions and microsatellite repeat variations (also called short tandem repeats or STRs)
  > short tandem repeats or STRs,短串联重复序列
  - Each dbSNP entry includes the sequence context of the polymorphism (i.e., the surrounding sequence), the occurrence frequency of the polymorphism (by population or individual), and the experimental method(s), protocols, and conditions used to assay（测定） the variation
-  physical mapping, functional analysis, pharmacogenomics, association studies, and evolutionary studies  
   - In the physical mapping of nucleotide sequences, variations are used as positional markers
   - Variations that occur in functional regions of genes or in conserved non-coding regions might cause significant changes in the complement of transcribed sequences
   - The associations between variations and complex genetic traits are more ambiguous than simple, single-gene mutations that lead to a phenotypic change

Flanking sequence The untranscribed regions at the 5′ or 3′ ends of a transcribed gene.

# MEDCO: Enabling Secure and Privacy-Preserving Exploration of Distributed Clinical and Genomic Data
(a) collective homomorphic encryption to provide trust decentralization and end-to-end confidentiality protection
(b) obfuscation techniques to achieve formal notions of privacy, such as differential privacy
> 随着越来越多的临床和基因组数据被数字化，数据分享成为实现个性化医疗承诺的一个基石。一些举措，例如以患者为中心的临床研究网络（PCORNet），eTRIKS /  - TranSMART ，瑞士个人健康网络（SPHN）和于基因组学与健康全球联盟（GA4GH），正在为旨在互连（迄今为止）临床的孤立存储库和基因组数据新的生物医学研究基础设施的打下基础。  
实际上，所有数据的安全性和机密性都依赖于中央存储库阻止外部（黑客）和内部（内部人）攻击的能力。此外，随着健康数据泄露的数量不断增加，临床站点面临巨大的公众压力，以确保患者数据的隐私和安全性得到适当保护，特别是在第三方存储或处理时。因此，临床站点担心采用集中式方法并将其数据外包到单个中央存储库（例如，云），尤其是在要共享的数据时高度敏感或识别（例如，基因组数据）。

the fully decentralized approach solves the single-point-of-failure issue
address the challenge of achieving privacy-preserving, secure and scalable data sharing we introduce MedCo
MedCo distributes the trust among a set of different “storage and processing” units to which clinical sites can securely outsource the storage of their data.
Together, the storage and processing units form a secure, federated and interoperable network that investigators can query for research purposes as if it were a single unified database
> 据我们所知，最近有两项涉及分布式医学数据库中隐私保护查询的工作;它们代表了这项工作所遵循的基于加密的方法的两个主要替代方案：第一个，PRINCESS ，基于可信硬件：网站在AES-GCM下加密所有数据（高级加密标准 - 伽罗瓦计数器模式）并将它们发送到在中央服务器中运行的飞地，具有英特尔SGX处理器;因此，该服务器对敏感数据进行解密和处理，从而实现统计模型的安全计算。与我们的工作相比，PRINCESS在允许的计算方面可以更加通用，但它提出单点故障（中央服务器），和它集中了对飞地和英特尔提供的证明协议的所有信任。此外，内存限制飞地限制了该计划的可扩展性，需要压缩和批处理技术才能启用处理大型基因组数据，MedCo进行扩展好多了。
最近的另一种方法SMCQL [16]基于
安全的双方计算; 它引入了一个框架
用于联合数据库上的私有数据网络查询
相互不信任的政党。 SMCQL具有安全性
查询执行器，实现不同类型的查询
（例如，合并，加入，不同）在分布式数据库上
依赖乱码电路和遗忘RAM（ORAM）
我们通过模拟三个临床站点的网络，在临床肿瘤学用例上实施和测试了MedCo，每个临床站点都将其数据存储外包给不同的SPU


electronic health records(EHR)
> 用例
查询一：皮肤皮肤黑色素瘤患者数量和BRAF基因突变影响600位蛋白质。大约一半的黑素瘤患者在V600E或V600K位置存在BRAF基因突变，可以通过BRAF抑制剂vemurafenib治疗[26]。因此，突变的BRAF黑色素瘤的比例是重要的
诊所或医院的基准
查询二：皮肤皮肤黑色素瘤患者数量和BRAF基因突变及突变（PTEN OR CDKN2A或MAP2K1或MAP2K2基因）。该查询基于用vemurafenib治疗的患者的事实：通过激活MAP激酶途径的突变产生耐药性[27]。当面临耐药性时，找到另一个具有相似突变特征的患者可能会带来临床决策的宝贵信息。
我们使用了8,000名癌症患者的基因组和临床数据，9个临床属性，以及每位患者平均142个基因突变（超过100万个观察结果）
总）。我们将这些数据从Mutation Annotation Format（MAF）导入到i2b2“星型模式”数据模型中。每个突变表示为包含其染色体，位置，参考等位基因和肿瘤等位基因的串联的代码。临床属性用ICD-10 [28]和ICD-O [29]国际术语编码。
初始测试环境包括3个互连的服务器
通过10 Gbps链路，配备两个2.5 GHz的Intel Xeon E5-2680 v3 CPU，支持12个核心上的24个线程和256 GB RAM。每个服务器代表一个SPU，并使用MedCo插件托管i2b2 / SHRINE Web客户端，i2b2配置单元包括SHRINE组件，新的MedCo单元和PostgreSQL中实现的i2b2数据库。
为了测试MedCo的可扩展性，我们将服务器数量增加到9（参见下面的设置S3）。设置我们的
系统和便于其部署，我们使用Docker [30]。
为了评估MedCo的性能，我们考虑了五种不同的实验设置，每次测量平均超过10次独立运行，并显示MedCo在未受保护的i2b2 / SHRINE部署方面的计算和存储开销：
- 增加数据集大小的ETL运行时：我们分析提取，转换和加载所需的时间数据（预处理），包括格式化，初始概率加密，确定性重新加密敏感的本体概念，以及i2b2数据库中的数据加载。
![FireShot Capture 002 -  - https___infoscience.epfl.ch_record_256348_files_TCBB2854776.pdf](/assets/FireShot%20Capture%20002%20-%20%20-%20https___infoscience.epfl.ch_record_256348_files_TCBB2854776.pdf.png)

clinical sites want to securely outsource the storage of their data to a preferred storage and processing unit ($SPU_j$ )
All SPUs are organized together in a peer-to-peer network and form a collective authority
 sample(LETTERS[c(1,3,7,20)], size=10, replace=true)
 有放回的在ACGT中抽样
 Notice that we cannot multiply two encrypted numbers together. This is the limit of Paillier cryptosystem which is a partially homomorphic encryption scheme in contrast to fully homomorphic.
