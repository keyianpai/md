---
title: "软件使用"
date: 2018-07-09T20:31:49+08:00
draft: false
---
heavy hitters problem—items that make up a
large fraction of the population
Analysis of Networks: Privacy in Bayesian
Networks and Problems in Lattice Models
Preserving Privacy in High-Dimensional Data Publishing
#Privacy Preserving GWAS Data Sharing
https://github.com/henripal/sgld
https://docs.google.com/presentation/d/1jDXcH7jcnr1SoWMaH6qZqgZJxvvoqvifs6xk65KEzN0/edit#slide=id.g3cf596d68a_1_192
# Large-Scale Privacy-Preserving Statistical Computations for Distributed Genome-Wide Association Studies
In 2000, the first human genome analysis took 9 months and cost
100 million USD.
# A new way to protect privacy in large-scale genome-wide association studies
https://www.khanacademy.org/math/ap-statistics/chi-square-tests/chi-square-tests-two-way-tables/v/chi-square-test-association-independence
The chi-square test of independence is used to analyze the frequency table (i.e. contengency table) formed by two categorical variables. The chi-square test evaluates whether there is a significant association between the categories of the two variables.
http://www.sthda.com/english/wiki/chi-square-test-of-independence-in-r

#Comparing Population Means under Local Differential Privacy: with Significance and Power
#A New Class of Private Chi-Square Tests
#Preserving Privacy in High-Dimensional Data Publishing
#DPT: Differentially Private Trajectory Synthesis Using Hierarchical Reference Systems

#Analysis of Networks: Privacy in Bayesian Networks and Problems in Lattice Models
#Knowing What to Ask: A Bayesian Active Learning Approach to the Surveying Problem
#diffpriv: An R Package for Easy Differential Privacy
#https://github.com/greenelab
In this paper, we assume that the learner has the ability to guide the instances
it gets, selecting instances that are more likely to lead to more accurate models. This
approach is called active learning

Asking all the participants the same set of questions may
be suboptimal. Instead, we may tailor the next question to
ask a participant based on their responses to the previous
questions. Such a design is based on the active learning
paradigm, where the learning algorithm can interactively
query users so as to best predict the responses to all questions
in the bank.

Kerckhoffs’s Principle [Kerckhoffs, 1883] of “no security
through obscurity”: differential privacy defends against a mechanism-aware
attacker.

.map (PLINK text fileset variant information file)
Variant information file accompanying a .ped text pedigree + genotype table.
A text file with no header file, and one line per variant with the following 3-4 fields:

Chromosome code. PLINK 1.9 also permits contig names here, but most older programs do not.
Variant identifier
Position in morgans or centimorgans (optional; also safe to use dummy value of '0')
Base-pair coordinate

.ped (PLINK/MERLIN/Haploview text pedigree + genotype table)
Original standard text format for sample pedigree information and genotype calls.
Contains no header line, and one line per sample with 2V+6 fields where V is the number of variants. The first six fields are the same as those in a .fam file. The seventh and eighth fields are allele calls for the first variant in the .map file ('0' = no call); the 9th and 10th are allele calls for the second variant; and so on.
Family ID ('FID')
Within-family ID ('IID'; cannot be '0')
Within-family ID of father ('0' if father isn't in dataset)
Within-family ID of mother ('0' if mother isn't in dataset)
Sex code ('1' = male, '2' = female, '0' = unknown)
Phenotype value ('1' = control, '2' = case, '-9'/'0'/non-numeric = missing data if case/control)

Genotyping
microarray that aims to determine the genotype at [Edit:] predetermined loci（基因座）.homozygous（纯合的） at the locus(基因座), then only one probe will bind and fluoresce（荧光）; if the sample is heterozygous（杂合的）, then both probes will bind (to the maternal and paternal chromosomes) and fluoresce
Genotype calling
This more relates to the act of determining the genotype through the examination of the relevant fluorescent intensities during the process of genotyping (above)
cumulant generating function (CGF, or the log of the moment generating function) of the privacy loss random variable
$$K_{\mathcal{M}}(\lambda):=\log\mathbb{E}_{\theta\sim\mathcal{M}(X)}[e^{\lambda\log\frac{\mathcal{M}(X)(\theta)}{\mathcal{M}(X')(\theta)}}]=\log\mathbb{E}_{\theta\sim\mathcal{M}(X)}[{(\frac{\mathcal{M}(X)(\theta)}{\mathcal{M}(X')(\theta)}})^{\lambda}]$$
 (Rényi Differential Privacy)$(\alpha,\epsilon)$-RDP
 $$D_{\alpha}(\mathcal{M}(X)||\mathcal{M}(X')) := \frac{1}{\alpha-1} \log\mathbb{E}_{\theta\sim\mathcal{M}(X')} [{(\frac{\mathcal{M}(X)(\theta)}{\mathcal{M}(X')(\theta)}})^{\alpha}] \leq\epsilon$$
