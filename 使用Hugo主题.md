---
title: "使用Hugo主题"
date: 2018-07-03T20:31:49+08:00
draft: false
---

* 支持
* 好好
- zhi
- shi

# Privacy in the Genomic Era
由于基因组数据本身所固有的一些特征，对这些数据的使用对个人隐私具有重大意义，这些特征包括：

1. 和性状和某些疾病的关联
1. 标识能力（identification capability）
1. 反应家系关系

另外，直接面向消费者的DNA测试增加了基因数据在缺乏监管的环境下流通的可能性。

# Privacy preserving processing of genomic data: A survey
mapping of a sequence {sequence alignment (mapping)}：A sequencing platform produces randomly ordered short reads. These reads are needed to be put in the correct order using a reference sequence.   
After the mapping procedure, sequenced DNA is aligned to the reference genome ??

# Secure Genomic Testing with Size- and Position-Hiding
Private Substring Matching

- This protocol allows two parties – one with
a digitized genome and the other with a set of DNA markers
– to conduct a test, such that the result is only learned by
the former, and no other information is learned by either
party. In particular, the genome owner does not even learn
the size or the position of the markers, which makes SPHPSM
the first of its kind.

# Evaluating the Strength of Genomic Privacy Metrics

- I measured the strength of privacy metrics by requiring that metrics are monotonic with increasing adversary strength and uncovered serious problems with several existing metrics currently used to measure genomic privacy

# Systematizing Genomic Privacy Research – A Critical Analysis

- focusing on privacy-enhancing technologies used in the context of testing, storing, and sharing genomic data

# Redefining Genomic Privacy: Trust and Empowerment
Blockchains create trust by making trust unnecessary. Their design assures that boxes cannot be removed, and that data in the boxes cannot be changed.

# Privacy-preserving techniques of genomic data—a survey

# Towards Practical Privacy for Genomic Computation

# Deriving genomic diagnoses without revealing patient genomes

- Thousands of monogenic diseases have yielded definitive genomic
diagnoses and potential gene therapy targets
- provide such diagnoses while
preserving participant privacy through the use of secure multiparty computation
-  In multiple real scenarios (small patient cohorts, trio analysis, two-hospital collaboration), we used our methods to identify the causal variant while keeping up to 99.7% of all participants’ most sensitive genomic information private
* Personalized genomics now offers a definitive diagnosis for more than 4500 monogenic diseases and may soon offer diagnosis for all 7000
* fewer than 50 digenic diseases have been identified

In essence, variants found in a control population (common variants) are likely benign, whereas functional rare variants not found in the control population but seen in multiple affected individuals
are likely to cause disease
- Disease-specific “beacons” (that is, web servers
that answer allele-presence queries) are prone
to attacks that can identify individuals participating
in the study
- Frequency-based computation highlights the
fundamental “serve or protect” dilemma of all
genomic data
- introduce a proof-of-concept cryptographic
implementation that both serves and protects
- Although many millions of genomic variants
from all individuals are needed to perform the
computation, only a handful of causal variants
are ultimately of interest for the purpose of a
diagnosis
1. we convert patient genomes into vectors of simple values and show how simple operations on these vectors reveal the causative variant(s)
1. apply a cryptographic method called Yao’s protocol
to perform the desired computation with out revealing any participant’s input

- If we are looking to identify a causal variant, we provide each individual a variant vector of all possible rare missense and nonsense variants in the human genome  
- We ask them to privately denote (using simple code) “true” or “false” next to each variant (to indicate whether they have the specific mutation or not, respectively)   

We define three simple Boolean operations (INTERSECTION, SETDIFF, and MAX) that are useful for patient diagnosis

To quantify the privacy guarantees provided by
our system, we define the “protection quotient”
of a computation to be the fraction of private
information that is exposed neither to the other
participants nor to the entity running the computation
## 在github发布时baseurl一定要改呀

baseurl="https://keyianpai.github.io/"  
复旦ip：202.120.234.85

> 我看论文时在地址栏发现这个，还有[爱教材](http://www.itextbook.cn/)上的网站时会自动已机构身份登陆，上面ip显示的也是这个。

> 当括号是中文时超链接语法会失效，害我找半天
# Are Data Sharing and Privacy Protection Mutually Exclusive?

# Improving power and accuracy of genome-wide association studies via a multi-locus mixed linear model methodology

### 仿真基因数据
  ```R
  sim.ex1 <- generateSNPs(n=100,gene.no=5,block.no=4,block.size=10,
               p.same=0.9,p.different=0.75,
               p.minor=c(0.1,0.4,0.1,0.4),
               n.sample=80,SNPtoBETA=SNPtoBETA)

  ```

`generateSNPs()`函数为参与人数，为基因个数，为每个基因的块数，
### quantitative trait nucleotide (QTN) detection
#### random-SNP-effect mixed linear model (RMLM)
#### multi-locus random-SNP-effect mixed linear model (MRMLM)
#### efficient mixed model analysis (EMMA)
significance threshold $p$ value for
- MRMLM method was 0.0002
- RMLM method was $0.05/m_e$
- EMMA method was $0.05/m$
> RMLM use __modified__ Bonferroni correction for multiple tests, $m_e$ is effective number of markers. EMMA use Bonferroni correction for multiple tests, $m$ is the total number of markers

# Local Differential Privacy for Evolving Data
For large classes of statistics, we can use the sparse vector technique to repeatedly perform computations on a dataset such that the error required for a fixed privacy level grows not with the number of recomputations, but with the number of times the computation’s outcome changes significantly.

## plink的三种格式：bed、fam和bim
PED: pedigree information and genotype calls.谱系信息和基因型信息,每一行是一个人。accompanied by a .map file.  
MAP: 变异信息，每一行是一个变异。

## THRESH  算法
![Image from Gyazo](https://i.gyazo.com/c5b88d3a72eea226891bf696e7be1905.png)
算法每一轮(epoch)都会输出 $\tilde{p}^t$ 作为$p^t$的估计。
算法过程就是在每一轮 $n$ 个个体每个人都会投票（第8行），VOTE调用的输出 $a_i^t$ 就是这个个体根据自己掌握的信息以及一些公开的信息决定他认为总体均值 $p_i^t$ 是否发生了显著变化。然后算法根据投票的结果决定是否更新总体的均值。这样是会使得估计的结果不那么及时，但减少更新次数也就减少了隐私预算的消耗速度。
接下来，如果大多数人都投票认为总体均值 $p_i^t$ 变了，则算法更新总体均值，首先算法设置最近更新轮次为当前轮次（第12行，因为并不是每一轮都会更新总体均值），接着每个个体调用估计算法EST估计自己的局部均值，然后公开这个均值  。
若投票结果认为总体均值 $p_i^t$ 没变化太大，则最近更新轮次为上一轮的最近更新轮次，（接着每个用户在20行发布了按某个分布的抽样值作为局部均值的估计，但也没有被采用，所以不是太清楚这一步的目的，可能是纯粹为了保护隐私吧），既然大家投票认为总体均值未有显著变化，算法采用上一轮总体均值估计值 $\tilde{p}^{t-1}$ 以减少隐私消耗速度。

## 在github发布时baseurl一定要改呀


> 安装了插件Markdown-Preview-Plus支持数学公式试了快捷键Ctrl+Shift+X还是不行，最后在这个插件的设置里将一个选项改成Pandoc才行

> $\tilde{p}^t$  $\hat{p}^t$  $\sim{p}$ $\mathcal{P}$  $\alpha$  
然而带帽子还是不行。。。

> 然而的然而，我又安装了一个Markdown-preview-enhanced，帽子就阔以有啦~
