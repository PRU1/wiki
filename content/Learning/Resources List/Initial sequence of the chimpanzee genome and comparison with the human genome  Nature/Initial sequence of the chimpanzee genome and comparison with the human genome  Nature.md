---
Link: https://www.nature.com/articles/nature04072
---
  

![[41586_2005_Article_BFnature04072_Fig1_HTML.jpg]]

- [The Chimpanzee Sequencing and Analysis Consortium](https://www.nature.com/articles/nature04072#group-1)

## Abstract

Here we present a draft genome sequence of the common chimpanzee (_Pan troglodytes_). Through comparison with the human genome, we have generated a largely complete catalogue of the genetic differences that have accumulated since the human and chimpanzee species diverged from our common ancestor, constituting approximately thirty-five million single-nucleotide changes, five million insertion/deletion events, and various chromosomal rearrangements. We use this catalogue to explore the magnitude and regional variation of mutational forces shaping these two genomes, and the strength of positive and negative selection acting on their genes. In particular, we find that the patterns of evolution in human and chimpanzee protein-coding genes are highly correlated and dominated by the fixation of neutral and slightly deleterious alleles. We also use the chimpanzee genome as an outgroup to investigate human population genetics and identify signatures of selective sweeps in recent human evolution.

## Main

More than a century ago Darwin[1](https://www.nature.com/articles/nature04072#ref-CR1) and Huxley[2](https://www.nature.com/articles/nature04072#ref-CR2) posited that humans share recent common ancestors with the African great apes. Modern molecular studies have spectacularly confirmed this prediction and have refined the relationships, showing that the common chimpanzee (_Pan troglodytes_) and bonobo (_Pan paniscus_ or pygmy chimpanzee) are our closest living evolutionary relatives[3](https://www.nature.com/articles/nature04072#ref-CR3). Chimpanzees are thus especially suited to teach us about ourselves, both in terms of their similarities and differences with human. For example, Goodall's pioneering studies on the common chimpanzee revealed startling behavioural similarities such as tool use and group aggression[4](https://www.nature.com/articles/nature04072#ref-CR4),[5](https://www.nature.com/articles/nature04072#ref-CR5). By contrast, other features are obviously specific to humans, including habitual bipedality, a greatly enlarged brain and complex language[5](https://www.nature.com/articles/nature04072#ref-CR5). Important similarities and differences have also been noted for the incidence and severity of several major human diseases[6](https://www.nature.com/articles/nature04072#ref-CR6).

Genome comparisons of human and chimpanzee can help to reveal the molecular basis for these traits as well as the evolutionary forces that have moulded our species, including underlying mutational processes and selective constraints. Early studies sought to draw inferences from sets of a few dozen genes[7](https://www.nature.com/articles/nature04072#ref-CR7),[8](https://www.nature.com/articles/nature04072#ref-CR8),[9](https://www.nature.com/articles/nature04072#ref-CR9), whereas recent studies have examined larger data sets such as protein-coding exons[10](https://www.nature.com/articles/nature04072#ref-CR10), random genomic sequences[11](https://www.nature.com/articles/nature04072#ref-CR11),[12](https://www.nature.com/articles/nature04072#ref-CR12) and an entire chimpanzee chromosome[13](https://www.nature.com/articles/nature04072#ref-CR13).

Here we report a draft sequence of the genome of the common chimpanzee, and undertake comparative analyses with the human genome. This comparison differs fundamentally from recent comparative genomic studies of mouse, rat, chicken and fish[14](https://www.nature.com/articles/nature04072#ref-CR14),[15](https://www.nature.com/articles/nature04072#ref-CR15),[16](https://www.nature.com/articles/nature04072#ref-CR16),[17](https://www.nature.com/articles/nature04072#ref-CR17). Because these species have diverged substantially from the human lineage, the focus in such studies is on accurate alignment of the genomes and recognition of regions of unusually high evolutionary conservation to pinpoint functional elements. Because the chimpanzee lies at such a short evolutionary distance with respect to human, nearly all of the bases are identical by descent and sequences can be readily aligned except in recently derived, large repetitive regions. The focus thus turns to differences rather than similarities. An observed difference at a site nearly always represents a single event, not multiple independent changes over time. Most of the differences reflect random genetic drift, and thus they hold extensive information about mutational processes and negative selection that can be readily mined with current analytical techniques. Hidden among the differences is a minority of functionally important changes that underlie the phenotypic differences between the two species. Our ability to distinguish such sites is currently quite limited, but the catalogue of human–chimpanzee differences opens this issue to systematic investigation for the first time. We would also hope that, in elaborating the few differences that separate the two species, we will increase pressure to save chimpanzees and other great apes in the wild.

Our results confirm many earlier observations, but notably challenge some previous claims based on more limited data. The genome-wide data also allow some questions to be addressed for the first time. (Here and throughout, we refer to chimpanzee–human comparison as representing hominids and mouse–rat comparison as representing murids—of course, each pair covers only a subset of the clade.) The main findings include:

- Single-nucleotide substitutions occur at a mean rate of 1.23% between copies of the human and chimpanzee genome, with 1.06% or less corresponding to fixed divergence between the species.
    
- Regional variation in nucleotide substitution rates is conserved between the hominid and murid genomes, but rates in subtelomeric regions are disproportionately elevated in the hominids.
    
- Substitutions at CpG dinucleotides, which constitute one-quarter of all observed substitutions, occur at more similar rates in male and female germ lines than non-CpG substitutions.
    
- Insertion and deletion (indel) events are fewer in number than single-nucleotide substitutions, but result in ∼1.5% of the euchromatic sequence in each species being lineage-specific.
    
- There are notable differences in the rate of transposable element insertions: short interspersed elements (SINEs) have been threefold more active in humans, whereas chimpanzees have acquired two new families of retroviral elements.
    
- Orthologous proteins in human and chimpanzee are extremely similar, with ∼29% being identical and the typical orthologue differing by only two amino acids, one per lineage.
    
- The normalized rates of amino-acid-altering substitutions in the hominid lineages are elevated relative to the murid lineages, but close to that seen for common human polymorphisms, implying that positive selection during hominid evolution accounts for a smaller fraction of protein divergence than suggested in some previous reports.
    
- The substitution rate at silent sites in exons is lower than the rate at nearby intronic sites, consistent with weak purifying selection on silent sites in mammals.
    
- Analysis of the pattern of human diversity relative to hominid divergence identifies several loci as potential candidates for strong selective sweeps in recent human history.
    

In this paper, we begin with information about the generation, assembly and evaluation of the draft genome sequence. We then explore overall genome evolution, with the aim of understanding mutational processes at work in the human genome. We next focus on the evolution of protein-coding genes, with the aim of characterizing the nature of selection. Finally, we briefly discuss initial insights into human population genetics.

In recognition of its strong community support, we will refer to chimpanzee chromosomes using the orthologous numbering nomenclature proposed by ref. [18](https://www.nature.com/articles/nature04072#ref-CR18), which renumbers the chromosomes of the great apes from the International System for Human Cytogenetic Nomenclature (ISCN; 1978) standard to directly correspond to their human orthologues, using the terms 2A and 2B for the two ape chromosomes corresponding to human chromosome 2.

## Genome sequencing and assembly

We sequenced the genome of a single male chimpanzee (Clint; Yerkes pedigree number C0471; [Supplementary Table S1](https://www.nature.com/articles/nature04072#MOESM1)), a captive-born descendant of chimpanzees from the West Africa subspecies _Pan troglodytes verus_, using a whole-genome shotgun (WGS) approach[19](https://www.nature.com/articles/nature04072#ref-CR19),[20](https://www.nature.com/articles/nature04072#ref-CR20). The data were assembled using both the PCAP and ARACHNE programs[21](https://www.nature.com/articles/nature04072#ref-CR21),[22](https://www.nature.com/articles/nature04072#ref-CR22) (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome sequencing and assembly’ and [Supplementary Tables S2–S6](https://www.nature.com/articles/nature04072#MOESM1)). The former was a _de_ _novo_ assembly, whereas the latter made limited use of human genome sequence (NCBI build 34)[23](https://www.nature.com/articles/nature04072#ref-CR23),[24](https://www.nature.com/articles/nature04072#ref-CR24) to facilitate and confirm contig linking. The ARACHNE assembly has slightly greater continuity ([Table 1](https://www.nature.com/articles/nature04072#Tab1)) and was used for analysis in this paper. The draft genome assembly—generated from ∼3.6-fold sequence redundancy of the autosomes and ∼1.8-fold redundancy of both sex chromosomes—covers ∼94% of the chimpanzee genome with >98% of the sequence in high-quality bases. A total of 50% of the sequence (N50) is contained in contigs of length greater than 15.7 kilobases (kb) and supercontigs of length greater than 8.6 megabases (Mb). The assembly represents a consensus of two haplotypes, with one allele from each heterozygous position arbitrarily represented in the sequence.

**Table 1 Chimpanzee assembly statistics**

**Assessment of quality and coverage.** The chimpanzee genome assembly was subjected to rigorous quality assessment, based on comparison to finished chimpanzee bacterial artificial chromosomes (BACs) and to the human genome (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome sequencing and assembly’ and [Supplementary Tables S7–S16](https://www.nature.com/articles/nature04072#MOESM1)).

Nucleotide-level accuracy is high by several measures. About 98% of the chimpanzee genome sequence has quality scores[25](https://www.nature.com/articles/nature04072#ref-CR25) of at least 40 (Q40), corresponding to an error rate of ≤10-4. Comparison of the WGS sequence to 1.3 Mb of finished BACs from the sequenced individual is consistent with this estimate, giving a high-quality discrepancy rate of 3 × 10-4 substitutions and 2 × 10-4 indels, which is no more than expected given the heterozygosity rate (see below), as 50% of the polymorphic alleles in the WGS sequence will differ from the single-haplotype BACs. Comparison of protein-coding regions aligned between the WGS sequence, the recently published sequence of chimpanzee chromosome 21 (ref. [13](https://www.nature.com/articles/nature04072#ref-CR13); formerly chromosome 22 (ref. [18](https://www.nature.com/articles/nature04072#ref-CR18))) and the human genome also revealed no excess of substitutions in the WGS sequence (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome sequencing and assembly’). Thus, by restricting our analysis to high-quality bases, the nucleotide-level accuracy of the WGS assembly is essentially equal to that of ‘finished’ sequence.

Structural accuracy is also high based on comparison with finished BACs from the primary donor and other chimpanzees, although the relatively low level of sequence redundancy limits local contiguity. On the basis of comparisons with the primary donor, some small supercontigs (most <5 kb) have not been positioned within large supercontigs (∼1 event per 100 kb); these are not strictly errors but nonetheless affect the utility of the assembly. There are also small, undetected overlaps (all <1 kb) between consecutive contigs (∼1.2 events per 100 kb) and occasional local misordering of small contigs (∼0.2 events per 100 kb). No misoriented contigs were found. Comparison with the finished chromosome 21 sequence yielded similar discrepancy rates (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome sequencing and assembly’).

The most problematic regions are those containing recent segmental duplications. Analysis of BAC clones from duplicated (_n_ = 75) and unique (_n_ = 28) regions showed that the former tend to be fragmented into more contigs (1.6-fold) and more supercontigs (3.2-fold). Discrepancies in contig order are also more frequent in duplicated than unique regions (∼0.4 versus ∼0.1 events per 100 kb). The rate is twofold higher in duplicated regions with the highest sequence identity (> 98%). If we restrict the analysis to older duplications (≤ 98% identity) we find fewer assembly problems: 72% of those that can be mapped to the human genome are shared as duplications in both species. These results are consistent with the described limitations of current WGS assembly for regions of segmental duplication[26](https://www.nature.com/articles/nature04072#ref-CR26). Detailed analysis of these rapidly changing regions of the genome is being performed with more directed approaches[27](https://www.nature.com/articles/nature04072#ref-CR27).

### Chimpanzee polymorphisms

The draft sequence of the chimpanzee genome also facilitates genome-wide studies of genetic diversity among chimpanzees, extending recent work[28](https://www.nature.com/articles/nature04072#ref-CR28),[29](https://www.nature.com/articles/nature04072#ref-CR29),[30](https://www.nature.com/articles/nature04072#ref-CR30),[31](https://www.nature.com/articles/nature04072#ref-CR31). We sequenced and analysed sequence reads from the primary donor, four other West African and three central African chimpanzees (_Pan troglodytes troglodytes_) to discover polymorphic positions within and between these individuals ([Supplementary Table S17](https://www.nature.com/articles/nature04072#MOESM1)).

A total of 1.66 million high-quality single-nucleotide polymorphisms (SNPs) were identified, of which 1.01 million are heterozygous within the primary donor, Clint. Heterozygosity rates were estimated to be 9.5 × 10-4 for Clint, 8.0 × 10-4 among West African chimpanzees and 17.6 × 10-4 among central African chimpanzees, with the variation between West and central African chimpanzees being 19.0 × 10-4. The diversity in West African chimpanzees is similar to that seen for human populations[32](https://www.nature.com/articles/nature04072#ref-CR32), whereas the level for central African chimpanzees is roughly twice as high.

The observed heterozygosity in Clint is broadly consistent with West African origin, although there are a small number of regions of distinctly higher heterozygosity. These may reflect a small amount of central African ancestry, but more likely reflect undetected regions of segmental duplications present only in chimpanzees.

## Genome evolution

We set out to study the mutational events that have shaped the human and chimpanzee genomes since their last common ancestor. We explored changes at the level of single nucleotides, small insertions and deletions, interspersed repeats and chromosomal rearrangements. The analysis is nearly definitive for the smallest changes, but is more limited for larger changes, particularly lineage-specific segmental duplications, owing to the draft nature of the genome sequence.

### Nucleotide divergence

Best reciprocal nucleotide-level alignments of the chimpanzee and human genomes cover ∼2.4 gigabases (Gb) of high-quality sequence, including 89 Mb from chromosome X and 7.5 Mb from chromosome Y.

_Genome-wide rates._ We calculate the genome-wide nucleotide divergence between human and chimpanzee to be 1.23%, confirming recent results from more limited studies[12](https://www.nature.com/articles/nature04072#ref-CR12),[33](https://www.nature.com/articles/nature04072#ref-CR33),[34](https://www.nature.com/articles/nature04072#ref-CR34). The differences between one copy of the human genome and one copy of the chimpanzee genome include both the sites of fixed divergence between the species and some polymorphic sites within each species. By correcting for the estimated coalescence times in the human and chimpanzee populations (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome evolution’), we estimate that polymorphism accounts for 14–22% of the observed divergence rate and thus that the fixed divergence is ∼1.06% or less.

Nucleotide divergence rates are not constant across the genome, as has been seen in comparisons of the human and murid genomes[16](https://www.nature.com/articles/nature04072#ref-CR16),[17](https://www.nature.com/articles/nature04072#ref-CR17),[24](https://www.nature.com/articles/nature04072#ref-CR24),[35](https://www.nature.com/articles/nature04072#ref-CR35),[36](https://www.nature.com/articles/nature04072#ref-CR36). The average divergence in 1-Mb segments fluctuates with a standard deviation of 0.25% (coefficient of variation = 0.20), which is much greater than the 0.02% expected assuming a uniform divergence rate ([Fig. 1a](https://www.nature.com/articles/nature04072#Fig1); see also [Supplementary Fig. S1](https://www.nature.com/articles/nature04072#MOESM1)).

**Figure 1:** **Human-chimpanzee divergence in 1-Mb segments across the genome.**

![[41586_2005_Article_BFnature04072_Fig1_HTML 1.jpg]]

**a**, Distribution of divergence of the autosomes (blue), the X chromosome (red) and the Y chromosome (green). **b**, Distribution of variation by chromosome, shown as a box plot. The edges of the box correspond to quartiles; the notches to the standard error of the median; and the vertical bars to the range. The X and Y chromosomes are clear outliers, but there is also high local variation within each of the autosomes.

Regional variation in divergence could reflect local variation in either mutation rate or other evolutionary forces. Among the latter, one important force is genetic drift, which can cause substantial differences in divergence time across loci when comparing closely related species, as the divergence time for orthologues is the sum of two terms: _t_1, the time since speciation, and _t_2, the coalescence time for orthologues within the common ancestral population[37](https://www.nature.com/articles/nature04072#ref-CR37). Whereas _t_1 is constant across loci (∼6–7 million years[38](https://www.nature.com/articles/nature04072#ref-CR38)), _t_2 is a random variable that fluctuates across loci (with a mean that depends on population size and here may be on the order of 1–2 million years[39](https://www.nature.com/articles/nature04072#ref-CR39)). However, because of historical recombination, the characteristic scale of such fluctuations will be on the order of tens of kilobases, which is too small to account for the variation observed for 1-Mb regions[40](https://www.nature.com/articles/nature04072#ref-CR40) (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome evolution’). Other potential evolutionary forces are positive or negative selection. Although it is more difficult to quantify the expected contributions of selection in the ancestral population[41](https://www.nature.com/articles/nature04072#ref-CR41),[42](https://www.nature.com/articles/nature04072#ref-CR42),[43](https://www.nature.com/articles/nature04072#ref-CR43), it is clear that the effects would have to be very strong to explain the large-scale variation observed across mammalian genomes[16](https://www.nature.com/articles/nature04072#ref-CR16),[44](https://www.nature.com/articles/nature04072#ref-CR44). There is tentative evidence from in-depth analysis of divergence and diversity that natural selection is not the major contributor to the large-scale patterns of genetic variability in humans[45](https://www.nature.com/articles/nature04072#ref-CR45),[46](https://www.nature.com/articles/nature04072#ref-CR46),[47](https://www.nature.com/articles/nature04072#ref-CR47). For these reasons, we suggest that the large-scale variation in the human–chimpanzee divergence rate primarily reflects regional variation in mutation rate.

_Chromosomal variation in divergence rate._ Variation in divergence rate is evident even at the level of whole chromosomes ([Fig. 1b](https://www.nature.com/articles/nature04072#Fig1)). The most striking outliers are the sex chromosomes, with a mean divergence of 1.9% for chromosome Y and 0.94% for chromosome X. The likely explanation is a higher mutation rate in the male compared with female germ line[48](https://www.nature.com/articles/nature04072#ref-CR48). Indeed, the ratio of the male/female mutation rates (denoted _α_) can be estimated by comparing the divergence rates among the sex chromosomes and the autosomes and correcting for ancestral polymorphism as a function of population size of the most recent common ancestor (MRCA; see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome evolution’). Estimates for _α_ range from 3 to 6, depending on the chromosomes compared and the assumed ancestral population size ([Supplementary Table S18](https://www.nature.com/articles/nature04072#MOESM1)). This is significantly higher than recent estimates of _α_ for the murids (∼1.9) (ref. ref. [17](https://www.nature.com/articles/nature04072#ref-CR17)) and resolves a recent controversy based on smaller data sets[12](https://www.nature.com/articles/nature04072#ref-CR12),[24](https://www.nature.com/articles/nature04072#ref-CR24),[49](https://www.nature.com/articles/nature04072#ref-CR49),[50](https://www.nature.com/articles/nature04072#ref-CR50).

The higher mutation rate in the male germ line is generally attributed to the 5–6-fold higher number of cell divisions undergone by male germ cells[48](https://www.nature.com/articles/nature04072#ref-CR48). We reasoned that this would affect mutations resulting from DNA replication errors (the rate should scale with the number of cell divisions) but not mutations resulting from DNA damage such as deamination of methyl CpG to TpG (the rate should scale with time). Accordingly, we calculated _α_ separately for CpG sites, obtaining a value of ∼2 from the comparison of rates between autosomes and chromosome X. This intermediate value is a composite of the rates of CpG loss and gain, and is consistent with roughly equal rates of CpG to TpG transitions in the male and female germ line[51](https://www.nature.com/articles/nature04072#ref-CR51),[52](https://www.nature.com/articles/nature04072#ref-CR52).

Significant variation in divergence rates is also seen among autosomes ([Fig. 1b](https://www.nature.com/articles/nature04072#Fig1); _P_ < 3 × 10-15, Kruskal–Wallis test over 1-Mb windows), confirming earlier observations based on low-coverage WGS sampling[12](https://www.nature.com/articles/nature04072#ref-CR12). Additional factors thus influence the rate of divergence between chimpanzee and human chromosomes. These factors are likely to act at length scales significantly shorter than a chromosome, because the standard deviation across autosomes (0.21%) is comparable to the standard deviation seen in 1-Mb windows across the genome (0.13–0.35%). We therefore sought to understand local factors that contribute to variation in divergence rate.

_Contribution of CpG dinucleotides._ Sites containing CpG dinucleotides in either species show a substantially elevated divergence rate of 15.2% per base; they account for 25.2% of all substitutions while constituting only 2.1% of all aligned bases. The divergence at CpG sites represents both the loss of ancestral CpGs and the creation of new CpGs. The former process is known to occur at a rapid rate per base due to frequent methylation of cytosines in a CpG context and their frequent deamination[53](https://www.nature.com/articles/nature04072#ref-CR53),[54](https://www.nature.com/articles/nature04072#ref-CR54), whereas the latter process probably proceeds at a rate more typical of other nucleotide substitutions. Assuming that loss and creation of CpG sites are close to equilibrium, the mutation rate for bases in a CpG dinucleotide must be 10–12-fold higher than for other bases (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome evolution’ and ref. [51](https://www.nature.com/articles/nature04072#ref-CR51)).

Because of the high rate of CpG substitutions, regional divergence rates would be expected to correlate with regional CpG density. CpG density indeed varies across 1-Mb windows (mean = 2.1%, coefficient of variation = 0.44 compared with 0.0093 expected under a Poisson distribution), but only explains 4% of the divergence rate variance. In fact, regional CpG and non-CpG divergence is highly correlated (_r_ = 0.88; [Supplementary Fig. S2](https://www.nature.com/articles/nature04072#MOESM1)), suggesting that higher-order effects modulate the rates of two very different mutation processes (see also ref. [47](https://www.nature.com/articles/nature04072#ref-CR47)).

_Increased divergence in distal regions._ The most striking regional pattern is a consistent increase in divergence towards the ends of most chromosomes ([Fig. 2](https://www.nature.com/articles/nature04072#Fig2)). The terminal 10 Mb of chromosomes (including distal regions and proximal regions of acrocentric chromosomes) averages 15% higher divergence than the rest of the genome (Mann–Whitney _U_-test; _P_ < 10-30), with a sharp increase towards the telomeres. The phenomenon correlates better with physical distance than relative position along the chromosomes and may partially explain why smaller chromosomes tend to have higher divergence ([Supplementary Fig. S3](https://www.nature.com/articles/nature04072#MOESM1); see also ref. [15](https://www.nature.com/articles/nature04072#ref-CR15)). These observations suggest that large-scale chromosomal structure, directly or indirectly, influences regional divergence patterns. The cause of this effect is unclear, but these regions (∼15% of the genome) are notable in having high local recombination rate, high gene density and high G + C content.

**Figure 2:** **Regional variation in divergence rates.**

![[41586_2005_Article_BFnature04072_Fig2_HTML.jpg]]

Human–chimpanzee divergence (blue), G + C content (green) and human recombination rates173 (red) in sliding 1-Mb windows for human and chimpanzee chromosome 1. Divergence and G + C content are noticeably elevated near the 1p telomere, a trend that holds for most subtelomeric regions (see text). Internally on the chromosome, regions of low G + C content and high divergence often correspond to the dark G bands.

_Correlation with chromosome banding._ Another interesting pattern is that divergence increases with the intensity of Giemsa staining in cytogenetically defined chromosome bands, with the regions corresponding to Giemsa dark bands (G bands) showing 10% higher divergence than the genome-wide average (Mann–Whitney _U_-test; _P_ < 10-14) (see [Fig. 2](https://www.nature.com/articles/nature04072#Fig2)). In contrast to terminal regions, these regions (17% of the genome) tend to be gene poor, (G + C)-poor and low in recombination[55](https://www.nature.com/articles/nature04072#ref-CR55),[56](https://www.nature.com/articles/nature04072#ref-CR56). The elevated divergence seen in two such different types of regions suggests that multiple mechanisms are at work, and that no single known factor, such as G + C content or recombination rate, is an adequate predictor of regional variation in the mammalian genome by itself ([Fig. 3](https://www.nature.com/articles/nature04072#Fig3)). Elucidation of the relative contributions of these and other mechanisms will be important for formulating accurate models for population genetics, natural selection, divergence times and the evolution of genome-wide sequence composition[57](https://www.nature.com/articles/nature04072#ref-CR57).

**Figure 3:** **Divergence rates versus G + C content for 1-Mb segments across the autosomes.**

![[41586_2005_Article_BFnature04072_Fig3_HTML.jpg]]

Conditional on recombination rate, the relationship between divergence and G + C content varies. In regions with recombination rates less than 0.8 cM Mb-1 (blue), there is an inverse relationship, where high divergence regions tend to be (G + C)-poor and low divergence regions tend to be (G + C)-rich. In regions with recombination rates greater than 2.0 cM Mb-1, whether within 10 Mb (red) or proximal (green) of chromosome ends, both divergence and G + C content are uniformly high.

_Correlation with regional variation in the murid genome._ Given that sequence divergence shows regional variation in both hominids (human–chimpanzee) and murids (mouse–rat), we asked whether the regional rates are positively correlated between orthologous regions. Such a correlation would suggest that the divergence rate is driven, in part, by factors that have been conserved over the ∼75 million years since rodents, humans and apes shared a common ancestor. Comparative analysis of the human and murid genomes has suggested such a correlation[58](https://www.nature.com/articles/nature04072#ref-CR58),[59](https://www.nature.com/articles/nature04072#ref-CR59),[60](https://www.nature.com/articles/nature04072#ref-CR60), but the chimpanzee sequence provides a direct opportunity to compare independent evolutionary processes between two mammalian clades.

We compared the local divergence rates in hominids and murids across major orthologous segments in the respective genomes ([Fig. 4](https://www.nature.com/articles/nature04072#Fig4)). For orthologous segments that are non-distal in both hominids and murids, there is a strong correlation between the divergence rates (_r_ = 0.5, _P_ < 10-11). In contrast, orthologous segments that are centred within 10 Mb of a hominid telomere have disproportionately high divergence rates and G + C content relative to the murids (Mann–Whitney _U_-test; _P_ < 10-11 and _P_ < 10-4), implying that the elevation in these regions is, at least partially, lineage specific. The same general effect is observed (albeit less pronounced) if CpG dinucleotides are excluded ([Supplementary Fig. S4](https://www.nature.com/articles/nature04072#MOESM1)). Increased divergence and G + C content might be explained by ‘biased gene conversion’[61](https://www.nature.com/articles/nature04072#ref-CR61) due to the high hominid recombination rates in these distal regions. Segments that are distal in murids do not show elevated divergence rates, which is consistent with this model, because the recombination rates of distal regions are not as elevated in mouse and rat[62](https://www.nature.com/articles/nature04072#ref-CR62).

**Figure 4:** **Disproportionately elevated divergence and G + C content near hominid telomeres.**

![[41586_2005_Article_BFnature04072_Fig4_HTML.jpg]]

Scatter plot of the ratio of human–chimpanzee divergence over mouse–rat divergence versus the ratio of human G + C content over mouse G + C content across 199 syntenic blocks for which more than 1 Mb of sequence could be aligned between all four species. Blocks for which the centre is within 10 Mb of a telomere in hominids only (green) or in hominids and murids (magenta), but not in murids only (light blue), show a significant trend towards higher ratios than internal blocks (dark blue). Blocks on the X chromosome (red) tend to show a lower divergence ratio than autosomal blocks, consistent with a smaller difference between autosomal and X divergence in murids than in hominids (lower _α_).

Taken together, these observations suggest that sequence divergence rate is influenced by both conserved factors (stable across mammalian evolution) and lineage-specific factors (such as proximity to the telomere or recombination rate, which may change with chromosomal rearrangements).

### Insertions and deletions

We next studied the indel events that have occurred in the human and chimpanzee lineages by aligning the genome sequences to identify length differences. We will refer below to all events as insertions relative to the other genome, although they may represent insertions or deletions relative to the genome of the common ancestor.

The observable insertions fall into two classes: (1) ‘completely covered’ insertions, occurring within continuous sequence in both species; and (2) ‘incompletely covered’ insertions, occurring within sequence containing one or more gaps in the chimpanzee, but revealed by a clear discrepancy between the species in sequence length. Different methods are needed for reliable identification of modest-sized insertions (1 base to 15 kb) and large insertions (> 15 kb), with the latter only being reliably identifiable in the human genome (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome evolution’).

The analysis of modest-sized insertions reveals ∼32 Mb of human-specific sequence and ∼35 Mb of chimpanzee-specific sequence, contained in ∼5 million events in each species ([Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome evolution’ and [Supplementary Fig. S5](https://www.nature.com/articles/nature04072#MOESM1)). Nearly all of the human insertions are completely covered, whereas only half of the chimpanzee insertions are completely covered. Analysis of the completely covered insertions shows that the vast majority are small (45% of events cover only 1 base pair (bp), 96% are <20 bp and 98.6% are <80 bp), but that the largest few contain most of the sequence (with the ∼70,000 indels larger than 80 bp comprising 73% of the affected base pairs) ([Fig. 5](https://www.nature.com/articles/nature04072#Fig5)). The latter indels >80 bp fall into three categories: (1) about one-quarter are newly inserted transposable elements; (2) more than one-third are due to microsatellite and satellite sequences; (3) and the remainder are assumed to be mostly deletions in the other genome.

**Figure 5:** **Length distribution of small indel events, as determined using bounded sequence gaps.**

![[41586_2005_Article_BFnature04072_Fig5_HTML.jpg]]

Sequences present in chimpanzee but not in human (blue) or present in human but not in chimpanzee (red) are shown. The prominent spike around 300 nucleotides corresponds to SINE insertion events. Most of the indels are smaller than 20 bp, but larger indels account for the bulk of lineage-specific sequence in the two genomes.

The analysis of larger insertions (> 15 kb) identified 163 human regions containing 8.3 Mb of human-specific sequence in total ([Fig. 6](https://www.nature.com/articles/nature04072#Fig6)). These cases include 34 regions that involve exons from known genes, which are discussed in a subsequent section. Although we have no direct measure of large insertions in the chimpanzee genome, it appears likely that the situation is similar.

Both the total number of candidate human insertions/chimpanzee deletions (blue) and the number of bases altered (red) are shown.

![[41586_2005_Article_BFnature04072_Fig6_HTML.jpg]]

On the basis of this analysis, we estimate that the human and chimpanzee genomes each contain 40–45 Mb of species-specific euchromatic sequence, and the indel differences between the genomes thus total ∼90 Mb. This difference corresponds to ∼3% of both genomes and dwarfs the 1.23% difference resulting from nucleotide substitutions; this confirms and extends several recent studies[63](https://www.nature.com/articles/nature04072#ref-CR63),[64](https://www.nature.com/articles/nature04072#ref-CR64),[65](https://www.nature.com/articles/nature04072#ref-CR65),[66](https://www.nature.com/articles/nature04072#ref-CR66),[67](https://www.nature.com/articles/nature04072#ref-CR67). Of course, the number of indel events is far fewer than the number of substitution events (∼5 million compared with ∼35 million, respectively).

### Transposable element insertions

We next used the catalogue of lineage-specific transposable element copies to compare the activity of transposons in the human and chimpanzee lineages ([Table 2](https://www.nature.com/articles/nature04072#Tab2)).

**Table 2 Transposable element activity in human and chimpanzee lineages**

_Endogenous retroviruses._ Endogenous retroviruses (ERVs) have become all but extinct in the human lineage, with only a single retrovirus (human endogenous retrovirus K (HERV-K)) still active[24](https://www.nature.com/articles/nature04072#ref-CR24). HERV-K was found to be active in both lineages, with at least 73 human-specific insertions (7 full length and 66 solo long terminal repeats (LTRs)) and at least 45 chimpanzee-specific insertions (1 full length and 44 solo LTRs). A few other ERV classes persisted in the human genome beyond the human–chimpanzee split, leaving ∼9 human-specific insertions (all solo LTRs, including five HERV9 elements) before dying out.

Against this background, it was surprising to find that the chimpanzee genome has two active retroviral elements (PtERV1 and PtERV2) that are unlike any older elements in either genome; these must have been introduced by infection of the chimpanzee germ line. The smaller family (PtERV2) has only a few dozen copies, which nonetheless represent multiple (∼5–8) invasions, because the sequence differences among reconstructed subfamilies are too great (∼8%) to have arisen by mutation since divergence from human. It is closely related to a baboon endogenous retrovirus (BaEV, 88% ORF2 product identity) and a feline endogenous virus (ECE-1, 86% ORF2 product identity). The larger family (PtERV1) is more homogeneous and has over 200 copies. Whereas older ERVs, like HERV-K, are primarily represented by solo LTRs resulting from LTR–LTR recombination, more than half of the PtERV1 copies are still full length, probably reflecting the young age of the elements. PtERV1-like elements are present in the rhesus monkey, olive baboon and African great apes but not in human, orang-utan or gibbon, suggesting separate germline invasions in these species[68](https://www.nature.com/articles/nature04072#ref-CR68).

_Higher Alu activity in humans._ SINE (Alu) elements have been threefold more active in humans than chimpanzee (∼7,000 compared with ∼2,300 lineage-specific copies in the aligned portion), refining the rather broad range (2–7-fold) estimated in smaller studies[13](https://www.nature.com/articles/nature04072#ref-CR13),[67](https://www.nature.com/articles/nature04072#ref-CR67),[69](https://www.nature.com/articles/nature04072#ref-CR69). Most chimpanzee-specific elements belong to a subfamily (AluYc1) that is very similar to the source gene in the common ancestor. By contrast, most human-specific Alu elements belong to two new subfamilies (AluYa5 and AluYb8) that have evolved since the chimpanzee–human divergence and differ substantially from the ancestral source gene[69](https://www.nature.com/articles/nature04072#ref-CR69). It seems likely that the resurgence of Alu elements in humans is due to these potent new source genes. However, based on an examination of available finished sequence, the baboon shows a 1.6-fold higher Alu activity relative to human new insertions, suggesting that there may also have been a general decline in activity in the chimpanzee[67](https://www.nature.com/articles/nature04072#ref-CR67).

Some of the human-specific Alu elements are highly diverged (92 with >5% divergence), which would seem to suggest that they are much older than the human–chimpanzee split. Possible explanations include: gene conversion by nearby older elements; processed pseudogenes arising from a spurious transcription of an older element; precise excision from the chimpanzee genome; or high local mutation rate. In any case, the presence of such anomalies suggests that caution is warranted in the use of single-repeat elements as homoplasy-free phylogenetic markers.

_New Alu elements target (A + T)-rich DNA in human and chimpanzee genomes._ Older SINE elements are preferentially found in gene-rich, (G + C)-rich regions, whereas younger SINE elements are found in gene-poor, (A + T)-rich regions where long interspersed element (LINE)-1 (L1) copies also accumulate[24](https://www.nature.com/articles/nature04072#ref-CR24),[70](https://www.nature.com/articles/nature04072#ref-CR70). The latter distribution is consistent with the fact that Alu retrotransposition is mediated by L1 (ref. [71](https://www.nature.com/articles/nature04072#ref-CR71)). Murid genomes revealed no change in SINE distribution with age[17](https://www.nature.com/articles/nature04072#ref-CR17).

The human pattern might reflect either preferential retention of SINEs in (G + C)-rich regions, due to selection or mutation bias, or a recent change in Alu insertion preferences. With the availability of the chimpanzee genome, it is possible to classify the youngest Alu copies more accurately and thus begin to distinguish these possibilities.

Analysis shows that lineage-specific SINEs in both human and chimpanzee are biased towards (A + T)-rich regions, as opposed to even the most recent copies in the MRCA ([Fig. 7](https://www.nature.com/articles/nature04072#Fig7)). This indicates that SINEs are indeed preferentially retained in (G + C)-rich DNA, but comparison with a more distant primate is required to formally rule out the possibility that the insertion bias of SINEs did not change just before speciation.

**Figure 7:** **Correlation of Alu age and distribution by G + C content.**

![[41586_2005_Article_BFnature04072_Fig7_HTML.jpg]]

Alu elements that inserted after human–chimpanzee divergence are densest in the (G + C)-poor regions of the genome (peaking at 36–40% G + C), whereas older copies, common to both genomes, crowd (G + C)-rich regions. The figure is similar to figure 23 of ref. 24, but the use of chimpanzee allows improved separation of young and old elements, leading to a sharper transition in the pattern.

_Equal activity of L1 in both species._ The human and chimpanzee genomes both show ∼2,000 lineage-specific L1 elements, contrary to previous estimates based on small samples that L1 activity is 2–3-fold higher in chimpanzee[72](https://www.nature.com/articles/nature04072#ref-CR72).

Transcription from L1 source genes can sometimes continue into 3′ flanking regions, which can then be co-transposed[73](https://www.nature.com/articles/nature04072#ref-CR73),[74](https://www.nature.com/articles/nature04072#ref-CR74). Human–chimpanzee comparison revealed that ∼15% of the species-specific insertions appear to have carried with them at least 50 bp of flanking sequence (followed by a poly(A) tail and a target site duplication). In principle, incomplete reverse transcription could result in insertions of the flanking sequence only (without any L1 sequence), mobilizing gene elements such as exons, but we found no evidence of this.

_Retrotransposed gene copies._ The L1 machinery also mediates retrotransposition of host messenger RNAs, resulting in many intronless (processed) pseudogenes in the human genome[75](https://www.nature.com/articles/nature04072#ref-CR75),[76](https://www.nature.com/articles/nature04072#ref-CR76),[77](https://www.nature.com/articles/nature04072#ref-CR77). We identified 163 lineage-specific retrotransposed gene copies in human and 246 in chimpanzee ([Supplementary Table S19](https://www.nature.com/articles/nature04072#MOESM1)). Correcting for incomplete sequence coverage of the chimpanzee genome, we estimate that there are ∼200 and ∼300 processed gene copies in human and chimpanzee, respectively. Processed genes thus appear to have arisen at a rate of ∼50 per million years since the divergence of human and chimpanzee; this is lower than the estimated rate for early primate evolution[75](https://www.nature.com/articles/nature04072#ref-CR75), perhaps reflecting the overall decrease in L1 activity. As expected[78](https://www.nature.com/articles/nature04072#ref-CR78), ribosomal protein genes constitute the largest class in both species. The second largest class in chimpanzee corresponds to zinc finger C2H2 genes, which are not a major class in the human genome.

_The retrotransposon SVA and distribution of CpG islands by transposable elements._ The third most active element since speciation has been SVA, which created about 1,000 copies in each lineage. SVA is a composite element (∼1.5–2.5 kb) consisting of two Alu fragments, a tandem repeat and a region apparently derived from the 3′ end of a HERV-K transcript; it is probably mobilized by L1 (refs [79](https://www.nature.com/articles/nature04072#ref-CR79), [80](https://www.nature.com/articles/nature04072#ref-CR80)). This element is of particular interest because each copy carries a sequence that satisfies the definition of a CpG island[81](https://www.nature.com/articles/nature04072#ref-CR81) and contains potential transcription factor binding sites; the dispersion of 1,000 SVA copies could therefore be a source of regulatory differences between chimpanzee and human ([Supplementary Table S20](https://www.nature.com/articles/nature04072#MOESM1)). At least three human genes contain SVA insertions near their promoters ([Supplementary Table S21](https://www.nature.com/articles/nature04072#MOESM1)), one of which has been found to be differentially expressed between the two species[82](https://www.nature.com/articles/nature04072#ref-CR82),[83](https://www.nature.com/articles/nature04072#ref-CR83), but additional investigations will be required to determine whether the SVA insertion directly caused this difference.

_Homologous recombination between interspersed repeats._ Human–chimpanzee comparison also makes it possible to study homologous recombination between nearby repeat elements as a source of genomic deletions. We found 612 deletions (totalling 2 Mb) in the human genome that appear to have resulted from recombination between two nearby Alu elements present in the common ancestor; there are 914 such events in the chimpanzee genome. (The events are not biased to (A + T)-rich DNA and thus would not explain the preferential loss of Alu elements in such regions discussed above.) Similarly, we found 26 and 48 instances involving adjacent L1 copies and 8 and 22 instances involving retroviral LTRs in human and chimpanzee, respectively. None of the repeat-mediated deletions removed an orthologous exon of a known human gene in chimpanzee.

The genome comparison allows one to estimate the dependency of homologous recombination on divergence and distance. Homologous recombination seems to occur between quite (> 25%) diverged copies ([Fig. 8](https://www.nature.com/articles/nature04072#Fig8)), whereas the number of recombination events (_n_) varies inversely with the distance (_d_, in bases) between the copies (as _n_ ≈ 6 × 106 _d_-1.7; _r_2 = 0.9).

**Figure 8:** **Dependency of homologous recombination between Alu elements on divergence and distance.**

![[41586_2005_Article_BFnature04072_Fig8_HTML.jpg]]

**a**, Whereas homologous recombination occurs between quite divergent (Smith–Waterman score <1,000), closely spaced copies, more distant recombination seems to favour a better match between the recombining repeats. **b**, The frequency of Alu–Alu-mediated recombination falls markedly as a function of distance between the recombining copies. The first three points (magenta) involve recombination between left or right arms of one Alu inserted into another. The high number of occurrences at a distance of 300–400 nucleotides is due to the preference of integration in the A-rich tail; exclusion of this point does not change the parameters of the equation.

### Large-scale rearrangements

Finally, we examined the chimpanzee genome sequence for information about large-scale genomic alterations. Cytogenetic studies have shown that human and chimpanzee chromosomes differ by one chromosomal fusion, at least nine pericentric inversions, and in the content of constitutive heterochromatin[84](https://www.nature.com/articles/nature04072#ref-CR84). Human chromosome 2 resulted from a fusion of two ancestral chromosomes that remained separate in the chimpanzee lineage (chromosomes 2A and 2B in the revised nomenclature[18](https://www.nature.com/articles/nature04072#ref-CR18), formerly chimpanzee chromosomes 12 and 13); the precise fusion point has been mapped and its duplication structure described in detail[85](https://www.nature.com/articles/nature04072#ref-CR85),[86](https://www.nature.com/articles/nature04072#ref-CR86). In accord with this, alignment of the human and chimpanzee genome sequences shows a break in continuity at this point.

We searched the chimpanzee genome sequence for the precise locations of the 18 breakpoints corresponding to the 9 pericentric inversions ([Supplementary Table S22](https://www.nature.com/articles/nature04072#MOESM1)). By mapping paired-end sequences from chimpanzee large insert clones to the human genome, we were able to identify 13 of the breakpoints within the assembly from discordant end alignments. The positions of five breakpoints (on chromosomes 4, 5 and 12) were tested by fluorescence _in situ_ hybridization (FISH) analysis and all were confirmed. Also, the positions of three previously mapped inversion breakpoints (on chromosomes 15 and 18) matched closely those found in the assembly[87](https://www.nature.com/articles/nature04072#ref-CR87),[88](https://www.nature.com/articles/nature04072#ref-CR88). The paired-end analysis works well in regions of unique sequence, which constitute the bulk of the genome, but is less effective in regions of recent duplication owing to ambiguities in mapping of the paired-end sequences. Beyond the known inversions, we also found suggestive evidence of many additional smaller inversions, as well as older segmental duplications (< 98% identity; [Supplementary Fig. S6](https://www.nature.com/articles/nature04072#MOESM1)). However, both smaller inversions and more recent segmental duplications will require further investigations.

## Gene evolution

We next sought to use the chimpanzee sequence to study the role of natural selection in the evolution of human protein-coding genes. Genome-wide comparisons can shed light on many central issues, including: the magnitude of positive and negative selection; the variation in selection across different lineages, chromosomes, gene families and individual genes; and the complete loss of genes within a lineage.

We began by identifying a set of 13,454 pairs of human and chimpanzee genes with unambiguous 1:1 orthology for which it was possible to generate high-quality sequence alignments covering virtually the entire coding region (ref. [Supplementary Information](https://www.nature.com/articles/nature04072#ref-CR1) ‘Gene evolution’ and Table S23). The list contains a large fraction of the entire complement of human genes, although it under-represents gene families that have undergone recent local expansion (such as olfactory receptors and immunoglobulins). To facilitate comparison with the murid lineage, we also compiled a set of 7,043 human, chimpanzee, mouse and rat genes with unambiguous 1:1:1:1 orthology and high-quality sequence alignments ([Supplementary Table S24](https://www.nature.com/articles/nature04072#MOESM1)).

### Average rates of evolution

To assess the rate of evolution for each gene, we estimated _K_A, the number of coding base substitutions that result in amino acid change as a fraction of all such possible sites (the non-synonymous substitution rate). Because the background mutation rate varies across the genome, it is crucial to normalize _K_A for comparisons between genes. A striking illustration of this variation is the fact that the mean _K_A is 37% higher in the rapidly diverging distal 10 Mb of chromosomes than in the more proximal regions. Classically, the background rate is estimated by _K_S, the synonymous substitution rate (coding base substitutions that, because of codon redundancy, do not result in amino acid change). Because a typical gene has only a few synonymous changes between humans and chimpanzees, and not infrequently is zero, we exploited the genome sequence to estimate the local intergenic/intronic substitution rate, _K_I, where appropriate. _K_A and _K_S were also estimated for each lineage separately using mouse and rat as outgroups ([Fig. 9](https://www.nature.com/articles/nature04072#Fig9)).

**Figure 9:** **Human–chimpanzee–mouse–rat tree with branch-specific** _**K**_**A****/**_**K**_**S** **(**_**ω**_ **) values.**

![[41586_2005_Article_BFnature04072_Fig9_HTML.jpg]]

**a**, Evolutionary tree. The branch lengths are proportional to the absolute rates of amino acid divergence. **b**, Maximum-likelihood estimates of the rates of evolution in protein-coding genes for humans, chimpanzees, mice and rats. In the text, _ω_hominid is the _K_A/_K_S of the combined human and chimpanzee branches and _ω_murid of the combined mouse and rat branches. The slight difference between _ω_human and _ω_chimpanzee is not statistically significant; masking of some heterozygous bases in the chimpanzee sequence may contribute to the observed difference (see Supplementary Information ‘Gene evolution’).

The _K_A/_K_S ratio is a classical measure of the overall evolutionary constraint on a gene, where _K_A/_K_S≪1 indicates that a substantial proportion of amino acid changes must have been eliminated by purifying selection. Under the assumption that synonymous substitutions are neutral, _K_A/_K_S > 1 implies, but is not a necessary condition for, adaptive or positive selection. The _K_A/_K_I ratio has the same interpretation. The ratios will sometimes be denoted below by _ω_ with an appropriate subscript (for example, _ω_human) to indicate the branch of the evolutionary tree under study.

_Evolutionary constraint on amino acid sites within the hominid lineage._ Overall, human and chimpanzee genes are extremely similar, with the encoded proteins identical in the two species in 29% of cases. The median number of non-synonymous and synonymous substitutions per gene are two and three, respectively. About 5% of the proteins show in-frame indels, but these tend to be small (median = 1 codon) and to occur in regions of repeated sequence. The close similarity of human and chimpanzee genes necessarily limits the ability to make strong inferences about individual genes, but there is abundant data to study important sets of genes.

The _K_A/_K_S ratio for the human–chimpanzee lineage (_ω_hominid) is 0.23. The value is much lower than some recent estimates based on limited sequence data (ranging as high as 0.63 (ref. [7](https://www.nature.com/articles/nature04072#ref-CR7))), but is consistent with an estimate (0.22) from random expressed-sequence-tag (EST) sequencing[45](https://www.nature.com/articles/nature04072#ref-CR45). Similarly, _K_A/_K_I was also estimated as 0.23.

Under the assumption that synonymous mutations are selectively neutral, the results imply that 77% of amino acid alterations in hominid genes are sufficiently deleterious as to be eliminated by natural selection. Because synonymous mutations are not entirely neutral (see below), the actual proportion of amino acid alterations with deleterious consequences may be higher. Consistent with previous studies[8](https://www.nature.com/articles/nature04072#ref-CR8), we find that _K_A/_K_S of human polymorphisms with frequencies up to 15% is significantly higher than that of human–chimpanzee differences and more common polymorphisms ([Table 3](https://www.nature.com/articles/nature04072#Tab3)), implying that at least 25% of the deleterious amino acid alterations may often attain readily detectable frequencies and thus contribute significantly to the human genetic load.

**Table 3 Comparison of** _**K**_**A****/**_**K**_**S** **for divergence and human diversity**

_Evolutionary constraint on synonymous sites within hominid lineage._ We next explored the evolutionary constraints on synonymous sites, specifically fourfold degenerate sites. Because such sites have no effect on the encoded protein, they are often considered to be selectively neutral in mammals.

We re-examined this assumption by comparing the divergence at fourfold degenerate sites with the divergence at nearby intronic sites. Although overall divergence rates are very similar at fourfold degenerate and intronic sites, direct comparison is misleading because the former have a higher frequency of the highly mutable CpG dinucleotides (9% compared with 2%). When CpG and non-CpG sites are considered separately, we find that both CpG sites and non-CpG sites show markedly lower divergence in exonic synonymous sites than in introns (∼50% and ∼30% lower, respectively). This result resolves recent conflicting reports based on limited data sets[45](https://www.nature.com/articles/nature04072#ref-CR45),[89](https://www.nature.com/articles/nature04072#ref-CR89) by showing that such sites are indeed under constraint.

The constraint does not seem to result from selection on the usage of preferred codons, which has been detected in lower organisms[90](https://www.nature.com/articles/nature04072#ref-CR90) such as bacteria[91](https://www.nature.com/articles/nature04072#ref-CR91), yeast[92](https://www.nature.com/articles/nature04072#ref-CR92) and flies[93](https://www.nature.com/articles/nature04072#ref-CR93). In fact, divergence at fourfold degenerate sites increases slightly with codon usage bias (Kendall's _τ_ = 0.097, _P_ < 10-14). Alternatively, the observed constraint at synonymous sites might reflect ‘background selection’—that is, the indirect effect of purifying selection at amino acid sites causing reduced diversity and thereby reduced divergence at closely linked sites[42](https://www.nature.com/articles/nature04072#ref-CR42). Given the low rate of recombination in hominid genomes (a 1 kb region experiences only ∼1 crossover per 100,000 generations or 2 million years), such background selection should extend beyond exons to include nearby intronic sites[94](https://www.nature.com/articles/nature04072#ref-CR94). However, when the divergence rate is plotted relative to exon–intron boundaries, we find that the rate jumps sharply within a short region of ∼7 bp at the boundary ([Fig. 10](https://www.nature.com/articles/nature04072#Fig10)). This pattern strongly suggests that the action of purifying selection at synonymous sites is direct rather than indirect, suggesting that other signals, for example those involved in splice site selection, may be embedded in the coding sequence and therefore constrain synonymous sites.

**Figure 10:** **Purifying selection on synonymous sites.**

![[41586_2005_Article_BFnature04072_Fig10_HTML.jpg]]

Mean divergence around exon boundaries at non-CpG, exonic, fourfold degenerate sites and intronic sites, relative to the closest mRNA splice junction. The divergence rate at exonic, fourfold degenerate sites is significantly lower than at nearby intronic sites (Mann–Whitney _U_-test; _P_ < 10-27), suggesting that purifying selection limits the rate of synonymous codon substitutions.

_Comparison with murids._ An accurate estimate of _K_A/_K_S makes it possible to study how evolutionary constraint varies across clades. It was predicted more than 30 years ago[95](https://www.nature.com/articles/nature04072#ref-CR95) that selection against deleterious mutations would depend on population size, with mutations being strongly selected only if they reduce fitness by _s_≫1/4_N_ (where _N_ is effective population size). This would predict that genes would be under stronger purifying selection in murids than hominids, owing to their presumed larger population size. Initial analyses (involving fewer than 50 genes[96](https://www.nature.com/articles/nature04072#ref-CR96)) suggested a strong effect, but the wide variation in estimates of _K_A/_K_S in hominids[7](https://www.nature.com/articles/nature04072#ref-CR7),[8](https://www.nature.com/articles/nature04072#ref-CR8),[97](https://www.nature.com/articles/nature04072#ref-CR97) and murids[98](https://www.nature.com/articles/nature04072#ref-CR98) has complicated this analysis[45](https://www.nature.com/articles/nature04072#ref-CR45).

Using the large collection of 7,043 orthologous quartets, we calculated mean _K_A/_K_S values for the various branches of the four-species evolutionary tree (human, chimpanzee, mouse and rat; [Fig. 9](https://www.nature.com/articles/nature04072#Fig9)). The _K_A/_K_S ratio for hominids is 0.20. (This is slightly lower than the value of 0.23 obtained with all human–chimpanzee orthologues, probably reflecting slightly greater constraint on the class of proteins with clear orthologues across hominids and murids.)

The _K_A/_K_S ratio is markedly lower for murids than for hominids (_ω_murid ≈ 0.13 compared with _ω_hominid ≈ 0.20) ([Fig. 9](https://www.nature.com/articles/nature04072#Fig9)). This implies that there is an ∼35% excess of the amino-acid-changing mutations in the two hominids, relative to the two murids. Excess amino acid divergence may be explained by either increased adaptive evolution or relaxation of evolutionary constraints. As shown in the next section, the latter seems to be the principal explanation.

_Relaxed constraints in human evolution._ The _K_A/_K_S ratio can be used to make inferences about the role of positive selection in human evolution[99](https://www.nature.com/articles/nature04072#ref-CR99),[100](https://www.nature.com/articles/nature04072#ref-CR100). Because alleles under positive selection spread rapidly through a population, they will be found less frequently as common human polymorphisms than as human–chimpanzee differences[8](https://www.nature.com/articles/nature04072#ref-CR8). Positive selection can thus be detected by comparing the _K_A/_K_S ratio for common human polymorphisms with the _K_A/_K_S ratio for hominid divergence. These ratios have been estimated as _ω_polymorphism ≈ 0.20 based on an initial collection of common SNPs in human genes and _ω_divergence ≈ 0.34 based on comparison of human and Old World monkey genes[8](https://www.nature.com/articles/nature04072#ref-CR8). Thus, the proportion of amino acid changes attributable to positive selection was inferred to be ∼35% (ref. ref. [8](https://www.nature.com/articles/nature04072#ref-CR8)). This would imply a huge quantitative role for positive selection in human evolution.

With the availability of extensive data for both human polymorphism and human–chimpanzee divergence, we repeated this analysis (using the same set of genes for both estimates). We find that _ω_polymorphism ≈ 0.21–0.23 and _ω_divergence ≈ 0.23 are statistically indistinguishable ([Table 3](https://www.nature.com/articles/nature04072#Tab3)). Although some of the amino acid substitutions in human and chimpanzee evolution must surely reflect positive selection, the results indicate that the proportion of changes fixed by positive selection seems to be much lower than the previous estimate[8](https://www.nature.com/articles/nature04072#ref-CR8). (Because the previous results involved comparison to Old World monkeys, it is possible that they reflect strong positive selection earlier in primate evolution; however, we suspect that they reflect the fact that relatively few genes were studied and that different genes were used to study polymorphism and divergence.)

Relaxed negative selection pressures thus primarily explain the excess amino acid divergence in hominid genes relative to murids. Moreover, because both _ω_human and _ω_chimpanzee are similarly elevated this explanation applies equally to both lineages.

We next sought to study variation in the evolutionary rate of genes within the hominid lineage by searching for unusually high or low levels of constraint for genes and sets of genes.

### Rapid evolution in individual genes

We searched for individual genes that have accumulated amino acid substitutions faster than expected given the neutral substitution rate; we considered these genes as potentially being under strong positive selection. A total of 585 of the 13,454 human–chimpanzee orthologues (4.4%) have observed _K_A/_K_I > 1 (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Gene evolution’). However, given the low divergence, the _K_A/_K_I statistic has large variance. Simulations show that estimates of _K_A/_K_I > 1 would be expected to occur simply by chance in at least 263 cases if purifying selection is allowed to act non-uniformly across genes ([Supplementary Fig. S7](https://www.nature.com/articles/nature04072#MOESM1)).

Nonetheless, this set of 585 genes may be enriched for genes that are under positive selection. The most extreme outliers include glycophorin C, which mediates one of the _Plasmodium falciparum_ invasion pathways in human erythrocytes[101](https://www.nature.com/articles/nature04072#ref-CR101); granulysin, which mediates antimicrobial activity against intracellular pathogens such as _Mycobacterium tuberculosis_[102](https://www.nature.com/articles/nature04072#ref-CR102); as well as genes that have previously been shown to be undergoing adaptive evolution, such as the protamines and semenogelins involved in reproduction[103](https://www.nature.com/articles/nature04072#ref-CR103) and the Mas-related gene family involved in nociception[104](https://www.nature.com/articles/nature04072#ref-CR104). With similar follow-up studies on candidates from this list, one may be able to draw conclusions about positive selection on other individual genes. In subsequent sections, we examine the rate of divergence for sets of related genes with the aim of detecting subtler signals of accelerated evolution.

### Variation in evolutionary rate across physically linked genes

We explored how the rate of evolution varies regionally across the genome. Several studies of mammalian gene evolution have noted that the rate of amino acid substitution shows local clustering, with proteins encoded by nearby genes evolving at correlated rates[16](https://www.nature.com/articles/nature04072#ref-CR16),[105](https://www.nature.com/articles/nature04072#ref-CR105),[106](https://www.nature.com/articles/nature04072#ref-CR106),[107](https://www.nature.com/articles/nature04072#ref-CR107).

_Variation across chromosomes._ On the basis of an analysis of ∼100 genes[108](https://www.nature.com/articles/nature04072#ref-CR108), it was recently reported that the normalized rate of protein evolution is greater on the nine chromosomes that underwent major structural rearrangement during human evolution (chromosomes 1, 2, 5, 9, 12, 15, 16, 17 and 18); it was suggested that such rearrangements led to reduced gene flow and accelerated adaptive evolution. A subsequent study of a collection of chimpanzee ESTs gave contradictory results[109](https://www.nature.com/articles/nature04072#ref-CR109),[110](https://www.nature.com/articles/nature04072#ref-CR110). With our larger data set, we re-examined this issue and found no evidence of accelerated evolution on chromosomes with major rearrangements, even if we considered each rearrangement separately ([Supplementary Table S25](https://www.nature.com/articles/nature04072#MOESM1)).

Among all hominid chromosomes, the most extreme outlier is chromosome X with a mean _K_A/_K_I of 0.32. The higher mean seems to reflect a skewed distribution at both high and low values, with the median value (0.17) being more in line with other chromosomes (0.15). The excess of low values may reflect greater purifying selection at some genes, owing to the hemizygosity of chromosome X in males. The excess of high values may reflect increased adaptive selection also resulting from hemizygosity, if a considerable proportion of advantageous alleles are recessive[111](https://www.nature.com/articles/nature04072#ref-CR111). Interestingly, the higher _K_A/_K_I value on the X chromosome versus autosomes is largely restricted to genes expressed in testis[83](https://www.nature.com/articles/nature04072#ref-CR83).

_Variation in local gene clusters._ We next searched for genomic neighbourhoods with an unusually high density of rapidly evolving genes. Specifically, we calculated the median _K_A/_K_I for sliding windows of ten orthologues and identified extreme outliers (_P_ < 0.001 compared to random ordering of genes; see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Gene evolution’). A total of 16 such neighbourhoods were found, which greatly exceeds random expectation ([Table 4](https://www.nature.com/articles/nature04072#Tab4)). Repeating the analysis with larger windows (25, 50 and 100 orthologues) did not identify additional rapidly diverging regions.

**Table 4 Rapidly diverging gene clusters in human and chimpanzee**

In nearly all cases, the regions contain local clusters of phylogenetically and functionally related genes. The rapid diversification of gene families, postulated by ref. [112](https://www.nature.com/articles/nature04072#ref-CR112), can thus be readily discerned even at the relatively close distance of human–chimpanzee divergence. Most of the clusters are associated with functional categories such as host defence and chemosensation (see below). Examples include the epidermal differentiation complex encoding proteins that help form the cornified layer of the skin barrier ([Supplementary Fig. S8](https://www.nature.com/articles/nature04072#MOESM1)), the WAP-domain cluster encoding secreted protease inhibitors with antibacterial activity, and the Siglec cluster encoding _CD33_-related genes. Rapid evolution in these clusters does not seem to be unique to either human or chimpanzee[113](https://www.nature.com/articles/nature04072#ref-CR113),[114](https://www.nature.com/articles/nature04072#ref-CR114).

### Variation in evolutionary rate across functionally related genes

We next studied variation in the evolutionary rate of functional categories of genes, based on the Gene Ontology (GO) classification[115](https://www.nature.com/articles/nature04072#ref-CR115).

_Rapidly and slowly evolving categories within the hominid lineage._ We started by searching for sets of functionally related genes with exceptionally high or low constraint in humans and chimpanzees. For each of the 809 categories with at least 20 genes, _K_A/_K_S was calculated by concatenating the gene sequences. The category-specific ratios were compared to the average across all orthologues to identify extreme outliers using a metric based on the binomial test ([Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Gene evolution’ and [Supplementary Tables S26–S29](https://www.nature.com/articles/nature04072#MOESM1)). The numbers of observed outliers below a specific threshold (test statistic <0.001) were then compared to the expected distribution of outliers given randomly permuted annotations.

A total of 98 categories showed elevated _K_A/_K_S ratios at the specified threshold ([Table 5](https://www.nature.com/articles/nature04072#Tab5)). Only 30 would be expected by chance, indicating that most (but not all) of these categories undergo significantly accelerated evolution relative to the genome-wide average (_P_ < 10-4). The rapidly evolving categories within the hominid lineage are primarily related to immunity and host defence, reproduction, and olfaction, which are the same categories known to be undergoing rapid evolution within the broader mammalian lineage, as well as more distantly related species[15](https://www.nature.com/articles/nature04072#ref-CR15),[16](https://www.nature.com/articles/nature04072#ref-CR16),[116](https://www.nature.com/articles/nature04072#ref-CR116). Hominids thus seem to be typical of mammals in this respect (but see below).

**Table 5 GO categories with the highest divergence rates in hominids**

A total of 251 categories showed significantly low _K_A/_K_S ratios (compared with ∼32 expected by chance; _P_ < 10-4). These include a wide range of processes including intracellular signalling, metabolism, neurogenesis and synaptic transmission, which are evidently under stronger-than-average purifying selection. More generally, genes expressed in the brain show significantly stronger average constraint than genes expressed in other tissues[83](https://www.nature.com/articles/nature04072#ref-CR83).

_Differences between hominid and murid lineages._ Having found gene categories that show substantial variation in absolute evolutionary rate within hominids, we next examined variation in relative rates between murids and hominids. The _K_A/_K_S of each of the GO categories are highly correlated between the hominid and murid orthologue pairs, suggesting that the selective pressures acting on particular functional categories have been largely proportional in recent hominid and recent murid evolution ([Fig. 11](https://www.nature.com/articles/nature04072#Fig11)). However, there are several categories with significantly accelerated non-synonymous divergence on each of the lineages, which might represent functions that have undergone lineage-specific positive selection or a lineage-specific relaxation of constraint ([Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Gene evolution’ and [Supplementary Tables S30–S39](https://www.nature.com/articles/nature04072#MOESM1)).

**Figure 11:** **Hominid and murid** _**K**_**A****/**_**K**_**S** **(**_**ω**_ **) in GO categories with more than 20 analysed genes.**

![[41586_2005_Article_BFnature04072_Fig11_HTML.jpg]]

GO categories with putatively accelerated (test statistic <0.001; see Methods) non-synonymous divergence on the hominid lineages (red) and on the murid lineages (orange) are highlighted. Owing to the hierarchical nature of GO, the categories do not all represent independent data points. A non-redundant list of significant categories is provided in Table 8 and a complete list in Supplementary Table S30.

A total of 59 categories (compared with 11 expected at random, _P_ < 0.0003) show evidence of accelerated non-synonymous divergence in the murid lineage. These are dominated by functions and processes related to host defence, such as immune response and lymphocyte activation. Examples include genes encoding interleukins and various T-cell surface antigens (_Cd4_, _Cd8_, _Cd80_). Combined with the recent observation that genes involved in host defence have undergone gene family expansion in murids[16](https://www.nature.com/articles/nature04072#ref-CR16),[17](https://www.nature.com/articles/nature04072#ref-CR17), this suggests that the immune system has undergone extensive lineage-specific innovation in murids. Additional categories that also show relative acceleration in murids include chromatin-associated proteins and proteins involved in DNA repair. These categories may have similarly undergone stronger adaptive evolution in murids or, alternatively, they may contain fewer sites for mutations with slightly deleterious effects (with the result that the _K_A/_K_S ratios are less affected by the differences in population size[96](https://www.nature.com/articles/nature04072#ref-CR96),[117](https://www.nature.com/articles/nature04072#ref-CR117)).

Another 58 categories (versus 14 expected at random, _P_ < 0.0005) show evidence of accelerated evolution in hominids, with the set dominated by genes encoding proteins involved in transport (for example, ion transport), synaptic transmission, spermatogenesis and perception of sound ([Table 6](https://www.nature.com/articles/nature04072#Tab6)). Notably, some outliers include genes with brain-related functions, compatible with a recent finding[118](https://www.nature.com/articles/nature04072#ref-CR118). Potential positive selection on spermatogenesis genes in the hominids was also recently noted[119](https://www.nature.com/articles/nature04072#ref-CR119). However, as above, it is possible that these categories could have more sites for slightly deleterious mutations and thus be more affected by population size differences. Sequence information from more species and from individuals within species will be necessary to distinguish between the possible explanations.

**Table 6 GO categories with accelerated divergence rates in hominids relative to murids**

_Differences between the human and chimpanzee lineage._ One of the most interesting questions is perhaps whether certain categories have undergone accelerated evolution in humans relative to chimpanzees, because such genes might underlie unique aspects of human evolution.

As was done for hominids and murids above, we compared non-synonymous divergence for each category to search for relative acceleration in either lineage ([Fig. 12](https://www.nature.com/articles/nature04072#Fig12)). Seven categories show signs of accelerated evolution on the human lineage relative to chimpanzee, but this is only slightly more than the four expected at random (_P_ < 0.22). Intriguingly, the single strongest outlier is ‘transcription factor activity’, with the 348 human genes studied having accumulated 47% more amino acid changes than their chimpanzee orthologues. Genes with accelerated divergence in human include homeotic, forkhead and other transcription factors that have key roles in early development. However, given the small number of changes involved, additional data will be required to confirm this trend. There was no excess of accelerated categories on the chimpanzee lineage.

**Figure 12:** **Human and chimpanzee** _**K**_**A****/**_**K**_**S** **(**_**ω**_ **) in GO categories with more than 20 analysed genes.**

![[41586_2005_Article_BFnature04072_Fig12_HTML.jpg]]

GO categories with putatively accelerated (test statistic <0.001; see Methods) non-synonymous divergence on the human lineage (red) and on the chimpanzee lineage (orange) are highlighted. The variance of these estimates is larger than that seen in the hominid–murid comparison owing to the small number of lineage-specific substitutions. Owing to the hierarchical nature of the GO ontology, the categories do not all represent independent data points. A complete list of categories is provided in Supplementary Table S30.

We also compared human genes with and without disease associations, including mental retardation, for differences in mutation rate when compared to chimpanzee. Briefly, no significant differences were observed in either the background mutation rate or in the ratio of human-specific changes to chimpanzee-specific amino acid changes (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Gene evolution’ and [Supplementary Tables S40 and S41](https://www.nature.com/articles/nature04072#MOESM1)).

We thus find minimal evidence of acceleration unique to either the human or chimpanzee lineage across broad functional categories. This is not simply due to general lack of power resulting from the small number of changes since the divergence of human and chimpanzee, because one can detect acceleration of categories in either hominid relative to either murid. For example, 29 accelerated categories versus 9 expected at random (_P_ < 0.02) can be detected on the human lineage, and 40 categories versus 11 expected at random (_P_ < 0.007) on the chimpanzee lineage, relative to mouse. But the outliers are largely the same for both human and chimpanzee, indicating that the fraction of amino acid mutations that have contributed to human- and chimpanzee-specific patterns of evolution must be small relative to the fraction that have contributed to a common hominid and, to a large extent, mammalian pattern of evolution.

It was recently reported[10](https://www.nature.com/articles/nature04072#ref-CR10) that several functional categories are enriched for genes with evidence of positive selection in the human lineage or the chimpanzee lineage, and that these categories are largely different between the two lineages. These results and ours differ in ways that will require further investigation. With the potential exception of some developmental regulators, the categories that ref. [10](https://www.nature.com/articles/nature04072#ref-CR10) reported as showing the strongest enrichment of positive selection in one lineage (including cell adhesion, ion transport and perception of sound) are among those that we show as having accelerated divergence in both human and chimpanzee. This suggests that positive selection and relaxation of constraints may be correlated, or alternatively, that the results of ref. [10](https://www.nature.com/articles/nature04072#ref-CR10) may be enriched for false positives in categories that have experienced particularly strong relaxation of constraints in the hominids. Data from additional primates, as well as advances in analytical methods, will be necessary to distinguish between these alternatives. At present, strong evidence of positive selection unique to the human lineage is thus limited to a handful of genes[120](https://www.nature.com/articles/nature04072#ref-CR120).

Our analysis above largely omitted genes belonging to large gene families, because gene family expansion makes it difficult to define 1:1:1:1 orthologues across hominids and murids. One of the largest such families, the olfactory receptors, is known to be undergoing rapid divergence in primates. Directed study of these genes in the draft assembly has suggested that more than 100 functional human olfactory receptors are likely to be under no evolutionary constraint[121](https://www.nature.com/articles/nature04072#ref-CR121). Our analysis also omitted the majority of very recently duplicated genes owing to their lower coverage in the current chimpanzee assembly. However, recent human-specific duplications can be readily identified from the finished human genome sequence, and have previously been shown to be highly enriched for the same categories found to have high absolute rates of evolution in 1:1 orthologues here; that is, olfaction, immunity and reproduction[23](https://www.nature.com/articles/nature04072#ref-CR23).

### Gene disruptions in human and chimpanzee

Whereas most genes have undergone only subtle substitutions in their amino acid sequence, a few dozen have suffered more marked changes. We found a total of 53 known or predicted human genes that are either deleted entirely (36) or partially (17) in chimpanzee ([Supplementary Table S42](https://www.nature.com/articles/nature04072#MOESM1)). We have so far tested and confirmed 15 of these cases by polymerase chain reaction (PCR) or Southern blotting. An additional eight genes have sustained large deletions (> 15 kb) entirely within an intron. Some genes may have been missed in this count owing to limitations of the draft genome sequence. In addition, some genes may have suffered chain termination mutations or altered reading frames in chimpanzee, but accurate identification of these will require higher-quality sequence. The sensitivity of the reciprocal analysis of genes disrupted in human is currently limited by the small number of independently predicted gene models for the chimpanzee. Some of the gene disruptions may be related to interesting biological differences between the species, as discussed below.

### Genetic basis for human- and chimpanzee-specific biology

Given the substantial number of neutral mutations, only a small subset of the observed gene differences is likely to be responsible for the key phenotypic changes in morphology, physiology and behavioural complexity between humans and chimpanzees. Determining which differences are in this evolutionarily important subset and inferring their functional consequences will require additional types of evidence, including information from clinical observations and model systems[122](https://www.nature.com/articles/nature04072#ref-CR122). We describe some novel examples of genetic changes for which plausible functional or physiological consequences can be suggested.

_Apoptosis._ Mouse and human are known to differ with respect to an important mediator of apoptosis, caspase-12 (refs [123–125](https://www.nature.com/articles/nature04072#ref-CR123)). The protein triggers apoptosis in response to perturbed calcium homeostasis in mice, but humans seem to lack this activity owing to several mutations in the orthologous gene that together affect the protein produced by all known splice forms; the mutations include a premature stop codon and a disruption of the SHG box required for enzymatic activity of caspases. By contrast, the chimpanzee gene encodes an intact open reading frame and SHG box, indicating that the functional loss occurred in the human lineage. Intriguingly, loss-of-function mutations in mice confer increased resistance to amyloid-induced neuronal apoptosis without causing obvious developmental or behavioural defects[126](https://www.nature.com/articles/nature04072#ref-CR126). The loss of function in humans may contribute to the human-specific pathology of Alzheimer's disease, which involves amyloid-induced neurotoxicity and deranged calcium homeostasis.

_Inflammatory response._ Human and chimpanzee show a notable difference with respect to important mediators of immune and inflammatory responses. Three genes (_IL1F7_, _IL1F8_ and _ICEBERG_) that act in a common pathway involving the caspase-1 gene all appear to be deleted in chimpanzee. _ICEBERG_ is thought to repress caspase-1-mediated generation of pro-inflammatory _IL1_ cytokines, and its absence in chimpanzee may point to species-specific modulation of the interferon-γ- and lipopolysaccharide-induced inflammatory response[127](https://www.nature.com/articles/nature04072#ref-CR127).

_Parasite resistance._ Similarly, we found that two members of the primate-specific APOL gene cluster (_APOL1_ and _APOL4_) have been deleted from the chimpanzee genome. The APOL1 protein is associated with the high-density lipoprotein fraction in serum and has recently been proposed to be the lytic factor responsible for resistance to certain subspecies of _Trypanosoma brucei_, the parasite that causes human sleeping sickness and the veterinary disease nagana[128](https://www.nature.com/articles/nature04072#ref-CR128). The loss of the _APOL1_ gene in chimpanzees could thus explain the observation that human, gorilla and baboon possess the trypanosome lytic factor, whereas the chimpanzee does not[129](https://www.nature.com/articles/nature04072#ref-CR129).

_Sialic acid biology related proteins._ Sialic acids are cell-surface sugars that mediate many biological functions[130](https://www.nature.com/articles/nature04072#ref-CR130). Of 54 genes involved in sialic acid biology, 47 were suitable for analysis. We confirmed and extended findings on several that have undergone human-specific changes, including disruptions, deletions and domain-specific functional changes[113](https://www.nature.com/articles/nature04072#ref-CR113),[131](https://www.nature.com/articles/nature04072#ref-CR131),[132](https://www.nature.com/articles/nature04072#ref-CR132). Human- and chimpanzee-specific changes were also found in otherwise evolutionarily conserved sialyl motifs in four sialyl transferases (_ST6GAL1_, _ST6GALNAC3_, _ST6GALNAC4_ and _ST8SIA2_), suggesting changes in donor and/or acceptor binding[130](https://www.nature.com/articles/nature04072#ref-CR130). Lineage-specific changes were found in a complement factor H (_HF1_) sialic acid binding domain associated with human disease[133](https://www.nature.com/articles/nature04072#ref-CR133). Human _SIGLEC11_ has undergone gene conversion with a nearby pseudogene, correlating with acquisition of human-specific brain expression and altered binding properties[134](https://www.nature.com/articles/nature04072#ref-CR134).

### Human disease alleles

We next sought to identify putative functional differences between the species by searching for instances in which a human disease-causing allele appears to be the wild-type allele in the chimpanzee. Starting from 12,164 catalogued disease variants in 1,384 human genes, we identified 16 cases in which the altered sequence in a disease allele matched the chimpanzee sequence, and had plausible support in the literature ([Table 7](https://www.nature.com/articles/nature04072#Tab7); see also [Supplementary Table S43](https://www.nature.com/articles/nature04072#MOESM1)). Upon re-sequencing in seven chimpanzees, 15 cases were confirmed homozygous in all individuals, whereas one (_PON1_ I102V) appears to be a shared polymorphism ([Supplementary Table S44](https://www.nature.com/articles/nature04072#MOESM1)).

**Table 7 Candidate human disease variants found in chimpanzee**

Six cases represent _de novo_ human mutations associated with simple mendelian disorders. Similar cases have also been found in comparisons of more distantly related mammals[135](https://www.nature.com/articles/nature04072#ref-CR135), as well as between insects[136](https://www.nature.com/articles/nature04072#ref-CR136), and have been interpreted as a consequence of a relatively high rate of compensatory mutations. If compensatory mutations are more likely to be fixed by positive selection than by neutral drift[136](https://www.nature.com/articles/nature04072#ref-CR136), then the variants identified here might point towards adaptive differences between humans and chimpanzees. For example, the ancestral Thr 29 allele of cationic trypsinogen (_PRSS1_) causes autosomal dominant pancreatitis in humans[137](https://www.nature.com/articles/nature04072#ref-CR137), suggesting that the human-specific Asn 29 allele may represent a digestion-related molecular adaptation[138](https://www.nature.com/articles/nature04072#ref-CR138).

The remaining ten cases represent common human polymorphisms that have been reported to be associated with complex traits, including coronary artery disease and diabetes mellitus. In all of these cases we confirmed that the disease-associated allele in humans is indeed the ancestral allele by showing that it is carried not only by chimpanzee but also by outgroups such as the macaque. These ancestral alleles may thus have become human-specific risk factors due to changes in human physiology or environment, and the polymorphisms may represent ongoing adaptations. For example, _PPARG_ Pro 12 is the wild-type allele in chimpanzee but has been clearly associated with increased risk of type 2 diabetes in human[139](https://www.nature.com/articles/nature04072#ref-CR139). It is tempting to speculate that this allele may represent an ancestral ‘thrifty’ genotype[140](https://www.nature.com/articles/nature04072#ref-CR140).

The current results must be interpreted with caution, because few complex disease associations have been firmly established. The fact that the human disease allele is the wild-type allele in chimpanzee may actually indicate that some of the putative associations are spurious and not causal. However, this approach can be expected to become increasingly fruitful as the quality and completeness of the disease mutation databases improve.

## Human population genetics

The chimpanzee has a special role in informing studies of human population genetics, a field that is undergoing rapid expansion and acquiring new relevance to human medical genetics[141](https://www.nature.com/articles/nature04072#ref-CR141). The chimpanzee sequence allows recognition of those human alleles that represent the ancestral state and the derived state. It also allows estimates of local mutation rates, which serve as an important baseline in searching for signs of natural selection.

### Ancestral and derived alleles

Of ∼7.2 million SNPs mapped to the human genome in the current public database, we could assign the alleles as ancestral or derived in 80% of the cases according to which allele agrees with the chimpanzee genome sequence[142](https://www.nature.com/articles/nature04072#ref-CR142) (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’). For the remaining cases, no assignment could be made because of the following: the orthologous chimpanzee base differed from both human alleles (1.2%); was polymorphic in the chimpanzee sequences obtained (0.4%); or could not be reliably identified with the current draft sequence of the chimpanzee (18.8%), with many of these occurring in repeated or segmentally duplicated sequence. The first two cases arise presumably because a second mutation occurred in the chimpanzee lineage. It should be possible to resolve most of these cases by examining a close outgroup such as gorilla or orang-utan.

Mutations in the chimpanzee may also lead to the erroneous assignment of human alleles as derived alleles. This error rate can be estimated as the probability of a second mutation resulting in the chimpanzee sequence matching the derived allele (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’). The estimated error rate for typical SNPs is 0.5%, owing to the low nucleotide substitution rate. The exceptions are those SNPs for which the human alleles are CpG and TpG and the chimpanzee sequence is TpG. For these, a non-negligible fraction may have arisen by two independent deamination events within an ancestral CpG dinucleotide, which are well-known mutational hotspots[51](https://www.nature.com/articles/nature04072#ref-CR51) (also see above). Human SNPs in a CpG context for which the orthologous chimpanzee sequence is TpG account for 12% of the total, and have an estimated error rate of 9.8%. Across all SNPs, the average error rate, _ɛ_, is thus estimated to be ∼1.6%.

We compared the distribution of allele frequencies for ancestral and derived alleles using a database of allele frequencies for ∼120,000 SNPs (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’). As expected, ancestral alleles tend to have much higher frequencies than derived alleles ([Supplementary Fig. S9](https://www.nature.com/articles/nature04072#MOESM1)). Nonetheless, a significant proportion of derived alleles have high frequencies: 9.1% of derived alleles have frequency ≥80%.

An elegant result in population genetics states that, for a randomly interbreeding population of constant size, the probability that an allele is ancestral is equal to its frequency[143](https://www.nature.com/articles/nature04072#ref-CR143). We explored the extent to which this simple theoretical expectation fits the human population. We tabulated the proportion _p_a(_x_) of ancestral alleles for various frequencies of _x_ and compared this with the prediction _p_a(_x_) = _x_ ([Fig. 13](https://www.nature.com/articles/nature04072#Fig13)).

**Figure 13:** **The observed fraction of ancestral alleles in 1% bins of observed frequency.**

![[41586_2005_Article_BFnature04072_Fig13_HTML.jpg]]

The solid line shows the regression (_b_ = 0.83). The dotted line shows the theoretical relationship _p_a(_x_) = _x_. Note that because each variant yields a derived and an ancestral allele, the data are necessarily symmetrical about 0.5.

The data lie near the predicted line, but the observed slope (0.83) is substantially less than 1. One explanation for this deviation is that some ancestral alleles are incorrectly assigned (an error rate of _ɛ_ would artificially decrease the slope by a factor of 1–2_ɛ_). However, with _ɛ_ estimated to be only 1.6%, errors can only explain a small part of the deviation. The most likely explanation is the presence of bottlenecks during human history, which tend to flatten the distribution of allele frequencies. Theoretical calculations indicate that a recent bottleneck would decrease the slope by a factor of (1 - _b_), where _b_ is the inbreeding coefficient induced by the bottleneck (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’ and [Supplementary Fig. S10](https://www.nature.com/articles/nature04072#MOESM1)). This suggests that measurements of the slope in different human groups may shed light on population-specific bottlenecks. Consistent with this, preliminary analyses of allele frequencies in several regions for SNPs obtained by systematic uniform sampling indicate that the slope is significantly lower than 1 in European and Asian samples and close to 1 in an African sample (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’ and [Supplementary Fig. S11](https://www.nature.com/articles/nature04072#MOESM1)).

### Signatures of strong selective sweeps in recent human history

The pattern of human genetic variation holds substantial information about selection events that have shaped our species. Strong positive selection creates the distinctive signature of a ‘selective sweep’, whereby a rare allele rapidly rises to fixation and carries the haplotype on which it occurs to high frequency (the ‘hitchhiking’ effect). The surrounding region should show two distinctive signatures: a significant reduction of overall diversity, and an excess of derived alleles with high frequency in the population owing to hitchhiking of derived alleles on the selected haplotype (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’). The pattern might be detectable for up to 250,000 years after a selective sweep has ended[144](https://www.nature.com/articles/nature04072#ref-CR144). Notably, the chimpanzee genome provides crucial baseline information required for accurate assessment of both signatures.

The size of the interval affected by a selective sweep is expected to scale roughly with _s_, the selective advantage due to the mutation. Simulations can be used to study the distribution of the interval size (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’). With _s_ = 1%, the interval over which heterozygosity falls by 50% has a modal size of 600 kb and a probability of greater than 10% of exceeding 1 Mb.

We undertook an initial scan for large regions (> 1 Mb) with the two signatures suggestive of strong selective sweeps in recent human history. We began by identifying regions in which the observed human diversity rate was much lower than the expectation based on the observed divergence rate with chimpanzee. The human diversity rate was measured as the number of occurrences from a database of 1.92 million SNPs identified by shotgun sequencing in a panel of African–American individuals (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome sequencing and assembly’). The comparison with the chimpanzee eliminates regions in which low diversity simply reflects a low mutation rate in the region. Regions were identified based on a simple statistical procedure (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’). Six genomic regions stand out as clear outliers that show significantly reduced diversity relative to divergence ([Table 8](https://www.nature.com/articles/nature04072#Tab8); see also [Supplementary Fig. S12](https://www.nature.com/articles/nature04072#MOESM1)).

**Table 8 Human regions with strongest signal of selection based on diversity relative to divergence**

We next tested whether these six regions show a high proportion of SNPs with high-frequency derived alleles (defined here as alleles with frequency ≥80%). Within each region, we focused on the 1-Mb interval with the greatest discrepancy between diversity and divergence and compared it to 1-Mb regions throughout the genome. For the database of 120,000 SNPs with allele frequencies discussed above, the typical 1-Mb region in the human genome contains ∼40 SNPs, and the proportion _p_h of SNPs with high-frequency derived alleles is ∼9.1%. All six regions identified by our scan for reduced diversity have a higher than average fraction of high-frequency derived alleles; all six fall within the top 10% genome-wide and three fall within the top 1%. Although this is not definitive evidence for any particular region, the joint probability of all six regions randomly scoring in the top 10% is 10-6. The results indicate that the six regions are candidates for strong selective sweeps during the past 250,000 years[144](https://www.nature.com/articles/nature04072#ref-CR144). The regions differ notably with respect to gene content, ranging from one containing 57 annotated genes (chromosome 22) to another with no annotated genes whatsoever (chromosome 4). We have no evidence to implicate any individual functional element as a target of recent selection at this point, but the regions contain a number of interesting candidates for follow-up studies. Intriguingly, the chromosome 4 gene desert, which flanks a proto-cadherin gene and is conserved across vertebrates[15](https://www.nature.com/articles/nature04072#ref-CR15), has been implicated in two independent studies as being associated with obesity[145](https://www.nature.com/articles/nature04072#ref-CR145),[146](https://www.nature.com/articles/nature04072#ref-CR146).

In addition to the six regions, one further genomic region deserves mention: an interval of 7.6 Mb on chromosome 7q (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Human population genetics’). The interval contains several regions with high scores in the diversity-divergence analysis (including the seventh highest score overall) as well as in the proportion of high-frequency derived alleles. The region contains the _FOXP2_ and _CFTR_ genes. The former has been the subject of much interest as a possible target for selection during human evolution[147](https://www.nature.com/articles/nature04072#ref-CR147) and the latter as a target of selection in European populations[148](https://www.nature.com/articles/nature04072#ref-CR148).

Convincing proof of past selection will require careful analysis of the precise pattern of genetic variation in the region and the identification of a likely target of selection. Nonetheless, our findings suggest that the approach outlined here may help to unlock some of the secrets of recent human evolution through a combination of within-species and cross-species comparison.

## Discussion

Our knowledge of the human genome is greatly advanced by the availability of a second hominid genome. Some questions can be directly answered by comparing the human and chimpanzee sequences, including estimates of regional mutation rates and average selective constraints on gene classes. Other questions can be addressed in conjunction with other large data sets, such as issues in human population genetics for which the chimpanzee genome provides crucial controls. For still other questions, the chimpanzee genome simply provides a starting point for further investigation.

The hardest such question is: what makes us human? The challenge lies in the fact that most evolutionary change is due to neutral drift. Adaptive changes comprise only a small minority of the total genetic variation between two species. As a result, the extent of phenotypic variation between organisms is not strictly related to the degree of sequence variation. For example, gross phenotypic variation between human and chimpanzee is much greater than between the mouse species _Mus musculus_ and _Mus spretus_, although the sequence difference in the two cases is similar. On the other hand, dogs show considerable phenotypic variation despite having little overall sequence variation (∼0.15%). Genomic comparison markedly narrows the search for the functionally important differences between species, but specific biological insights will be needed to sift the still-large list of candidates to separate adaptive changes from neutral background.

Our comparative analysis suggests that the patterns of molecular evolution in the hominids are typical of a broader class of mammals in many ways, but distinctive in certain respects. As with the murids, the most rapidly evolving gene families are those involved in reproduction and host defence. In contrast to the murids, however, hominids appear to experience substantially weaker negative selection; this probably reflects their smaller population size. Consequently, hominids accumulate deleterious mutations that would be eliminated by purifying selection in murids. This may be both an advantage and a disadvantage. Although decreased purifying selection may tend to erode overall fitness, it may also allow hominids to ‘explore’ larger regions of the fitness landscape and thereby achieve evolutionary adaptations that can only be reached by passing through intermediate states of inferior fitness[149](https://www.nature.com/articles/nature04072#ref-CR149),[150](https://www.nature.com/articles/nature04072#ref-CR150).

Although the analyses presented here focus on protein-coding sequences, the chimpanzee genome sequence also allows systematic analysis of the recent evolution of gene regulatory elements for the first time. Initial analysis of both gene expression patterns and promoter regions suggest that their overall patterns of evolution closely mirror that of protein-coding regions. In an accompanying paper[83](https://www.nature.com/articles/nature04072#ref-CR83), we show that the rates of change in gene expression among different tissues in human and chimpanzee correlate with the nucleotide divergence in the putative proximal promoters and even more interestingly with the average level of constraint on proteins in the same tissues. Another study[151](https://www.nature.com/articles/nature04072#ref-CR151) has similarly used the chimpanzee sequence described here to show that gene promoter regions are also evolving under markedly less constraint in hominids than in murids.

The draft chimpanzee sequence here is sufficient for initial analyses, but it is still imperfect and incomplete. Definitive studies of gene and genome evolution—including pseudogene formation, gene family expansion and segmental duplication—will require high-quality finished sequence. In this regard, we note that efforts are already underway to construct a BAC-based physical map and to increase the shotgun sequence coverage to approximately sixfold redundancy. The added coverage alone will not affect the analysis greatly, but plans are in place to produce finished sequence for difficult to sequence and important segments of the genome.

Our close biological relatedness to chimpanzees not only allows unique insights into human biology, it also creates ethical obligations. Although the genome sequence was acquired without harm to chimpanzees, the availability of the sequence may increase pressure to use chimpanzees in experimentation. We strongly oppose reducing the protection of chimpanzees and instead advocate the policy positions suggested by an accompanying paper[152](https://www.nature.com/articles/nature04072#ref-CR152). Furthermore, the existence of chimpanzees and other great apes in their native habitats is increasingly threatened by human civilization. More effective policies are urgently needed to protect them in the wild. We hope that elaborating how few differences separate our species will broaden recognition of our duty to these extraordinary primates that stand as our siblings in the family of life.

## Methods

### Sequencing and assembly

Approximately 22.5 million sequence reads were derived from both ends of inserts (paired end reads) from 4-, 10-, 40- and 180-kb clones, all prepared from primary blood lymphocyte DNA. Genomic resources available from the source animal include a lymphoid cell line (S006006) and genomic DNA (NS06006) at Coriell Cell Repositories ([http://locus.umdnj.edu/ccr/](http://locus.umdnj.edu/ccr/)), as well as a BAC library (CHORI-251)[153](https://www.nature.com/articles/nature04072#ref-CR153) (see also [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1) ‘Genome sequencing and assembly’).

### Genome alignment

BLASTZ[154](https://www.nature.com/articles/nature04072#ref-CR154) was used to align non-repetitive chimpanzee regions against repeat-masked human sequence. BLAT[155](https://www.nature.com/articles/nature04072#ref-CR155) was subsequently used to align the more repetitive regions. The combined alignments were chained[156](https://www.nature.com/articles/nature04072#ref-CR156) and only best reciprocal alignments were retained for further analysis.

### Insertions and deletions

Small insertion/deletion (indel) events (< 15 kb) were parsed directly from the BLASTZ genome alignment by counting the number and size of alignment gaps between bases within the same contig. Sites of large-scale indels (> 15 kb) were detected from discordant placements of paired sequence reads against the human assembly. Size thresholds were obtained from both human fosmid alignments on human sequence (40 ± 2.58 kb) and chimpanzee plasmid alignments against human chromosome 21 (4.5 ± 1.84 kb). Indels were inferred by two or more pairs surpassing these thresholds by more than two standard deviations and the absence of sequence data within the discordancy.

### Gene annotation

A total of 19,277 human RefSeq transcripts[157](https://www.nature.com/articles/nature04072#ref-CR157), representing 16,045 distinct genes, were indirectly aligned to the chimpanzee sequence via the genome alignment. After removing low-quality sequences and likely alignment artefacts, an initial catalogue containing 13,454 distinct 1:1 human–chimpanzee orthologues was created for the analyses described here. A subset of 7,043 of these genes with unambiguous mouse and rat orthologues were realigned using Clustal W[158](https://www.nature.com/articles/nature04072#ref-CR158) for the lineage-specific analyses. Updated gene catalogues can be obtained from [http://www.ensembl.org](http://www.ensembl.org/).

### Rates of divergence

Nucleotide divergence rates were estimated using baseml with the REV model. Non-CpG rates were estimated from all sites that did not overlap a CG dinucleotide in either human or chimpanzee. _K_A and _K_S were estimated jointly for each orthologue using codeml with the F3x4 codon frequency model and no additional constraints, except for the comparison of divergent and polymorphic substitutions where _K_A/_K_S for both was estimated as (_ΔA_/_N_A)/(_ΔS_/_N_S), with _N_S/_N_A, the ratio of synonymous to non-synonymous sites, estimated as 0.36 from the orthologue alignments. Unless otherwise specified, _K_A/_K_S for a set of genes was calculated by summing the number of substitutions and the number of sites to obtain _K_A and _K_S for the concatenated set before taking the ratio. Hominid and murid pairwise rates were estimated independently from codons aligned across all four species. Human and chimpanzee lineage-specific _K_A and _K_S were estimated on an unrooted tree with both mouse and rat included. Lineage-specific rates were also estimated by parsimony, with essentially identical results (see [Supplementary Information](https://www.nature.com/articles/nature04072#MOESM1)). _K_I was estimated from all interspersed repeats within 250 kb of the mid-point of each gene.

### Accelerated evolution in GO categories

The binomial probability of observing _X_ or more non-synonymous substitutions, given a total of _X_ + _Y_ substitutions and the expected proportion _x_ from all orthologues, was calculated by summing substitutions across the orthologues in each GO category. For the absolute rate test, _Y_ = the number of synonymous substitutions in orthologues in the same category. For the relative rate tests, _Y_ = the number of non-synonymous substitutions on the opposite lineage. Note that this binomial probability is simply a metric designed to identify potentially accelerated categories, it is not a _P_-value that can be used to reject directly the null hypothesis of no acceleration in that particular category. For each test, the observed number of categories with a binomial probability less than 0.001 was compared to the expected distribution of such outliers by repeating the procedure 10,000 times on randomly permuted GO annotations. The significance of the number of observed outliers _n_ was estimated as the proportion of random trials yielding _n_ or more outliers.

### Detection of selective sweeps

The observed number of human SNPs, _u_i, human bases, _m_i, human–chimpanzee substitutions, _v_i, and chimpanzee bases, _n_i, within each set of non-overlapping 1-Mb windows along the human genome were used to generate two random numbers, _x_i (adjusted human diversity) and _y_i (adjusted human–chimpanzee divergence), from the two beta-distributions:

where _a_ = 1, _b_ = 1,000, _c_ = 1 and _d_ = 100. These numbers were then fit to a linear regression:

A _P_-value for each window was calculated for each window based on (_x__i_, _y__i_) and the regression line. This was repeated 100 times and the average of the _P_-values taken as the _P_-value for diversity given divergence in each window. Overlapping windows with _P_ < 0.1 containing at least one window of _P_ < 0.05 were coalesced and scored as the sum of their -log(_p_) scores.

## The Chimpanzee Sequencing and Analysis Consortium

Tarjei S. Mikkelsen1,2, LaDeana W. Hillier3, Evan E. Eichler4, Michael C. Zody1, David B. Jaffe1, Shiaw-Pyng Yang3, Wolfgang Enard5, Ines Hellmann5, Kerstin Lindblad-Toh1, Tasha K. Altheide6, Nicoletta Archidiacono7, Peer Bork8,9, Jonathan Butler1, Jean L. Chang1, Ze Cheng4, Asif T. Chinwalla3, Pieter deJong10, Kimberley D. Delehaunty3, Catrina C. Fronick3, Lucinda L. Fulton3, Yoav Gilad11, Gustavo Glusman12, Sante Gnerre1, Tina A. Graves3, Toshiyuki Hayakawa6, Karen E. Hayden13, Xiaoqiu Huang14, Hongkai Ji15, W. James Kent16, Mary-Claire King4, Edward J. Kulbokas, III1, Ming K. Lee4, Ge Liu13, Carlos Lopez-Otin17, Kateryna D. Makova18, Orna Man19, Elaine R. Mardis3, Evan Mauceli1, Tracie L. Miner3, William E. Nash3, Joanne O. Nelson3, Svante Pääbo5, Nick J. Patterson1, Craig S. Pohl3, Katherine S. Pollard16, Kay Prüfer5, Xose S. Puente17, David Reich1,20, Mariano Rocchi7, Kate Rosenbloom16, Maryellen Ruvolo21, Daniel J. Richter1, Stephen F. Schaffner1, Arian F. A. Smit12, Scott M. Smith3, Mikita Suyama8, James Taylor18, David Torrents8, Eray Tuzun4, Ajit Varki6, Gloria Velasco17, Mario Ventura7, John W. Wallis3, Michael C. Wendl3, Richard K. Wilson3, Eric S. Lander1,22,23,24, Robert H. Waterston4

Affiliations for participants: 1Broad Institute of MIT and Harvard, 320 Charles Street, Cambridge, Massachusetts 02141, USA. 2Division of Health Sciences and Technology, Massachusetts Institute of Technology, 77 Massachusetts Avenue, Cambridge, Massachusetts 02139, USA. 3Genome Sequencing Center, Washington University School of Medicine, Campus Box 8501, 4444 Forest Park Avenue, St Louis, Missouri 63108, USA. 4Genome Sciences, University of Washington School of Medicine, 1705 NE Pacific Street, Seattle, Washington 98195, USA. 5Max Planck Institute of Evolutionary Anthropology, Deutscher Platz 6, D-04103 Leipzig, Germany. 6University of California, San Diego, 9500 Gilman Drive, La Jolla, California 92093, USA. 7Department of Genetics and Microbiology, University of Bari, 70126 Bari, Italy. 8EMBL, Meyerhofstrasse 1, Heidelberg D-69117, Germany. 9Max Delbrück Center for Molecular Medicine (MDC), Bobert-Rössle-Strasse 10, D-13125 Berlin, Germany. 10Children's Hospital Oakland Research Institute, 747 52nd Street, Oakland, California 94609, USA. 11Department of Genetics, Yale University School of Medicine, 333 Cedar Street, New Haven, Connecticut 06520, USA. 12Institute for Systems Biology, 1441 North 34th Street, Seattle, Washington 98103, USA. 13Department of Genetics, Case Western Reserve University, 10900 Euclid Avenue, Cleveland, Ohio 44106, USA. 14Department of Computer Science, Iowa State University, 226 Atanasoff Hall, Ames, Iowa 50011, USA. 15Department of Statistics, Harvard University, 1 Oxford Street, Cambridge, Massachusetts 02138, USA. 16University of California, Santa Cruz, Center for Biomolecular Science and Engineering, 1156 High Street, Santa Cruz, California 95064, USA. 17Departamento de Bioquimica y Biologia Molecular, Instituto Universitario de Oncologia del Principado de Asturias, Universidad de Oviedo, C/Fernando Bongera s/n, 33006 Oviedo, Spain. 18The Pennsylvania State University, Center for Comparative Genomics and Bioinformatics and Department of Biology, University Park, Pennsylvania 16802, USA. 19Department of Structural Biology, Weizmann Institute of Science, Rehovot 76100, Israel. 20Department of Genetics, Harvard Medical School, Boston, Massachusetts 02115, USA. 21Departments of Anthropology and of Organismic and Evolutionary Biology, Harvard University, 11 Divinity Avenue, Cambridge, Massachusetts 02138, USA. 22Department of Systems Biology, Harvard Medical School, Boston, Massachusetts 02115, USA. 23Whitehead Institute for Biomedical Research, Cambridge, Massachusetts 02142, USA. 24Department of Biology, Massachusetts Institute of Technology, Cambridge, Massachusetts 02139, USA.

## References

1. Darwin, C. _The Descent of Man, and Selection in Relation to Sex_ (D Appleton and Company, New York, 1871)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20Descent%20of%20Man%2C%20and%20Selection%20in%20Relation%20to%20Sex&publication_year=1871&author=Darwin%2CC)
    
2. Huxley, T. H. _Evidence as to Man's Place in Nature_ (Williams and Norgate, London, 1863)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Evidence%20as%20to%20Man%27s%20Place%20in%20Nature&publication_year=1863&author=Huxley%2CTH)
    
3. Goodman, M. The genomic record of humankind's evolutionary roots. _Am. J. Hum. Genet._ **64**, 31–39 (1999)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1377699) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20genomic%20record%20of%20humankind%27s%20evolutionary%20roots&journal=Am.%20J.%20Hum.%20Genet.&volume=64&pages=31-39&publication_year=1999&author=Goodman%2CM)
    
4. Goodall, J. Tool-using and aimed throwing in a community of free-living chimpanzees. _Nature_ **201**, 1264–1266 (1964)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Tool-using%20and%20aimed%20throwing%20in%20a%20community%20of%20free-living%20chimpanzees&journal=Nature&volume=201&pages=1264-1266&publication_year=1964&author=Goodall%2CJ)
    
5. Whiten, A. et al. Cultures in chimpanzees. _Nature_ **399**, 682–685 (1999)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Cultures%20in%20chimpanzees&journal=Nature&volume=399&pages=682-685&publication_year=1999&author=Whiten%2CA)
    
6. Olson, M. V. & Varki, A. Sequencing the chimpanzee genome: insights into human evolution and disease. _Nature Rev. Genet._ **4**, 20–28 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Sequencing%20the%20chimpanzee%20genome%3A%20insights%20into%20human%20evolution%20and%20disease&journal=Nature%20Rev.%20Genet.&volume=4&pages=20-28&publication_year=2003&author=Olson%2CMV&author=Varki%2CA)
    
7. Eyre-Walker, A. & Keightley, P. D. High genomic deleterious mutation rates in hominids. _Nature_ **397**, 344–347 (1999)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=High%20genomic%20deleterious%20mutation%20rates%20in%20hominids&journal=Nature&volume=397&pages=344-347&publication_year=1999&author=Eyre-Walker%2CA&author=Keightley%2CPD)
    
8. Fay, J. C., Wyckoff, G. J. & Wu, C. I. Positive and negative selection on the human genome. _Genetics_ **158**, 1227–1234 (2001)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1461725) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Positive%20and%20negative%20selection%20on%20the%20human%20genome&journal=Genetics&volume=158&pages=1227-1234&publication_year=2001&author=Fay%2CJC&author=Wyckoff%2CGJ&author=Wu%2CCI)
    
9. King, M. C. & Wilson, A. C. Evolution at two levels in humans and chimpanzees. _Science_ **188**, 107–116 (1975)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Evolution%20at%20two%20levels%20in%20humans%20and%20chimpanzees&journal=Science&volume=188&pages=107-116&publication_year=1975&author=King%2CMC&author=Wilson%2CAC)
    
10. Clark, A. G. et al. Inferring nonneutral evolution from human-chimp-mouse orthologous gene trios. _Science_ **302**, 1960–1963 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Inferring%20nonneutral%20evolution%20from%20human-chimp-mouse%20orthologous%20gene%20trios&journal=Science&volume=302&pages=1960-1963&publication_year=2003&author=Clark%2CAG)
    
11. Hellmann, I. et al. Selection on human genes as revealed by comparisons to chimpanzee cDNA. _Genome Res._ **13**, 831–837 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430916) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Selection%20on%20human%20genes%20as%20revealed%20by%20comparisons%20to%20chimpanzee%20cDNA&journal=Genome%20Res.&doi=10.1101%2Fgr.944903&volume=13&pages=831-837&publication_year=2003&author=Hellmann%2CI)
    
12. Ebersberger, I., Metzler, D., Schwarz, C. & Paabo, S. Genomewide comparison of DNA sequences between humans and chimpanzees. _Am. J. Hum. Genet._ **70**, 1490–1497 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC379137) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genomewide%20comparison%20of%20DNA%20sequences%20between%20humans%20and%20chimpanzees&journal=Am.%20J.%20Hum.%20Genet.&volume=70&pages=1490-1497&publication_year=2002&author=Ebersberger%2CI&author=Metzler%2CD&author=Schwarz%2CC&author=Paabo%2CS)
    
13. Watanabe, H. et al. DNA sequence and comparative analysis of chimpanzee chromosome 22. _Nature_ **429**, 382–388 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=DNA%20sequence%20and%20comparative%20analysis%20of%20chimpanzee%20chromosome%2022&journal=Nature&volume=429&pages=382-388&publication_year=2004&author=Watanabe%2CH)
    
14. Jaillon, O. et al. Genome duplication in the teleost fish _Tetraodon nigroviridis_ reveals the early vertebrate proto-karyotype. _Nature_ **431**, 946–957 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genome%20duplication%20in%20the%20teleost%20fish%20Tetraodon%20nigroviridis%20reveals%20the%20early%20vertebrate%20proto-karyotype&journal=Nature&volume=431&pages=946-957&publication_year=2004&author=Jaillon%2CO)
    
15. Hillier, L. W. et al. Sequence and comparative analysis of the chicken genome provide unique perspectives on vertebrate evolution. _Nature_ **432**, 695–716 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Sequence%20and%20comparative%20analysis%20of%20the%20chicken%20genome%20provide%20unique%20perspectives%20on%20vertebrate%20evolution&journal=Nature&volume=432&pages=695-716&publication_year=2004&author=Hillier%2CLW)
    
16. Mouse Genome Sequencing Consortium, Initial sequencing and comparative analysis of the mouse genome. _Nature_ **420**, 520–562 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Initial%20sequencing%20and%20comparative%20analysis%20of%20the%20mouse%20genome&journal=Nature&volume=420&pages=520-562&publication_year=2002)
    
17. Rat Genome Sequencing Project Consortium. Genome sequence of the Brown Norway rat yields insights into mammalian evolution. _Nature_ **428**, 493–521 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genome%20sequence%20of%20the%20Brown%20Norway%20rat%20yields%20insights%20into%20mammalian%20evolution&journal=Nature&volume=428&pages=493-521&publication_year=2004)
    
18. McConkey, E. H. Orthologous numbering of great ape and human chromosomes is essential for comparative genomics. _Cytogenet. Genome Res._ **105**, 157–158 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Orthologous%20numbering%20of%20great%20ape%20and%20human%20chromosomes%20is%20essential%20for%20comparative%20genomics&journal=Cytogenet.%20Genome%20Res.&volume=105&pages=157-158&publication_year=2004&author=McConkey%2CEH)
    
19. Sanger, F., Coulson, A. R., Hong, G. F., Hill, D. F. & Petersen, G. B. Nucleotide sequence of bacteriophage lambda DNA. _J. Mol. Biol._ **162**, 729–773 (1982)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Nucleotide%20sequence%20of%20bacteriophage%20lambda%20DNA&journal=J.%20Mol.%20Biol.&volume=162&pages=729-773&publication_year=1982&author=Sanger%2CF&author=Coulson%2CAR&author=Hong%2CGF&author=Hill%2CDF&author=Petersen%2CGB)
    
20. Myers, G. Whole-genome DNA sequencing. _Comput. Sci. Eng._ **1**, 33–43 (1999)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Whole-genome%20DNA%20sequencing.&journal=Comput.%20Sci.%20Eng.&volume=1&pages=33-43&publication_year=1999&author=Myers%2CG)
    
21. Huang, X., Wang, J., Aluru, S., Yang, S. P. & Hillier, L. PCAP: a whole-genome assembly program. _Genome Res._ **13**, 2164–2170 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC403719) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=PCAP%3A%20a%20whole-genome%20assembly%20program&journal=Genome%20Res.&volume=13&pages=2164-2170&publication_year=2003&author=Huang%2CX&author=Wang%2CJ&author=Aluru%2CS&author=Yang%2CSP&author=Hillier%2CL)
    
22. Jaffe, D. B. et al. Whole-genome sequence assembly for mammalian genomes: Arachne 2. _Genome Res._ **13**, 91–96 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430950) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Whole-genome%20sequence%20assembly%20for%20mammalian%20genomes%3A%20Arachne%202&journal=Genome%20Res.&volume=13&pages=91-96&publication_year=2003&author=Jaffe%2CDB)
    
23. International Human Genome Sequencing Consortium. Finishing the euchromatic sequence of the human genome. _Nature_ **431**, 931–945 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Finishing%20the%20euchromatic%20sequence%20of%20the%20human%20genome&journal=Nature&volume=431&pages=931-945&publication_year=2004)
    
24. International Human Genome Sequencing Consortium. Initial sequencing and analysis of the human genome. _Nature_ **409**, 860–920 (2001)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Initial%20sequencing%20and%20analysis%20of%20the%20human%20genome&journal=Nature&volume=409&pages=860-920&publication_year=2001)
    
25. Ewing, B., Hillier, L., Wendl, M. C. & Green, P. Base-calling of automated sequencer traces using phred. I. Accuracy assessment. _Genome Res._ **8**, 175–185 (1998)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Base-calling%20of%20automated%20sequencer%20traces%20using%20phred.%20I.%20Accuracy%20assessment&journal=Genome%20Res.&volume=8&pages=175-185&publication_year=1998&author=Ewing%2CB&author=Hillier%2CL&author=Wendl%2CMC&author=Green%2CP)
    
26. She, X. et al. Shotgun sequence assembly and recent segmental duplications within the human genome. _Nature_ **431**, 927–930 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Shotgun%20sequence%20assembly%20and%20recent%20segmental%20duplications%20within%20the%20human%20genome&journal=Nature&volume=431&pages=927-930&publication_year=2004&author=She%2CX)
    
27. Cheng, Z. et al. A genome-wide comparison of recent chimpanzee and human segmental duplications. _Nature_ doi:10.1038/nature04000 (this issue)
28. Fischer, A., Wiebe, V., Paabo, S. & Przeworski, M. Evidence for a complex demographic history of chimpanzees. _Mol. Biol. Evol._ **21**, 799–808 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Evidence%20for%20a%20complex%20demographic%20history%20of%20chimpanzees&journal=Mol.%20Biol.%20Evol.&volume=21&pages=799-808&publication_year=2004&author=Fischer%2CA&author=Wiebe%2CV&author=Paabo%2CS&author=Przeworski%2CM)
    
29. Yu, N. et al. Low nucleotide diversity in chimpanzees and bonobos. _Genetics_ **164**, 1511–1518 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1462640) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Low%20nucleotide%20diversity%20in%20chimpanzees%20and%20bonobos&journal=Genetics&volume=164&pages=1511-1518&publication_year=2003&author=Yu%2CN)
    
30. Kaessmann, H., Wiebe, V., Weiss, G. & Paabo, S. Great ape DNA sequences reveal a reduced diversity and an expansion in humans. _Nature Genet._ **27**, 155–156 (2001)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Great%20ape%20DNA%20sequences%20reveal%20a%20reduced%20diversity%20and%20an%20expansion%20in%20humans&journal=Nature%20Genet.&volume=27&pages=155-156&publication_year=2001&author=Kaessmann%2CH&author=Wiebe%2CV&author=Weiss%2CG&author=Paabo%2CS)
    
31. Kitano, T., Schwarz, C., Nickel, B. & Paabo, S. Gene diversity patterns at 10 X-chromosomal loci in humans and chimpanzees. _Mol. Biol. Evol._ **20**, 1281–1289 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Gene%20diversity%20patterns%20at%2010%20X-chromosomal%20loci%20in%20humans%20and%20chimpanzees&journal=Mol.%20Biol.%20Evol.&volume=20&pages=1281-1289&publication_year=2003&author=Kitano%2CT&author=Schwarz%2CC&author=Nickel%2CB&author=Paabo%2CS)
    
32. The International SNP Map Working Group. A map of human genome sequence variation containing 1.42 million single nucleotide polymorphisms. _Nature_ **409**, 928–933 (2001)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20map%20of%20human%20genome%20sequence%20variation%20containing%201.42%20million%20single%20nucleotide%20polymorphisms&journal=Nature&volume=409&pages=928-933&publication_year=2001)
    
33. Chen, F. C. & Li, W. H. Genomic divergences between humans and other hominoids and the effective population size of the common ancestor of humans and chimpanzees. _Am. J. Hum. Genet._ **68**, 444–456 (2001)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1235277) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genomic%20divergences%20between%20humans%20and%20other%20hominoids%20and%20the%20effective%20population%20size%20of%20the%20common%20ancestor%20of%20humans%20and%20chimpanzees&journal=Am.%20J.%20Hum.%20Genet.&volume=68&pages=444-456&publication_year=2001&author=Chen%2CFC&author=Li%2CWH)
    
34. Fujiyama, A. et al. Construction and analysis of a human-chimpanzee comparative clone map. _Science_ **295**, 131–134 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Construction%20and%20analysis%20of%20a%20human-chimpanzee%20comparative%20clone%20map&journal=Science&volume=295&pages=131-134&publication_year=2002&author=Fujiyama%2CA)
    
35. Hardison, R. C. et al. Covariation in frequencies of substitution, deletion, transposition, and recombination during eutherian evolution. _Genome Res._ **13**, 13–26 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430971) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Covariation%20in%20frequencies%20of%20substitution%2C%20deletion%2C%20transposition%2C%20and%20recombination%20during%20eutherian%20evolution&journal=Genome%20Res.&volume=13&pages=13-26&publication_year=2003&author=Hardison%2CRC)
    
36. Webster, M. T., Smith, N. G., Lercher, M. J. & Ellegren, H. Gene expression, synteny, and local similarity in human noncoding mutation rates. _Mol. Biol. Evol._ **21**, 1820–1830 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Gene%20expression%2C%20synteny%2C%20and%20local%20similarity%20in%20human%20noncoding%20mutation%20rates&journal=Mol.%20Biol.%20Evol.&volume=21&pages=1820-1830&publication_year=2004&author=Webster%2CMT&author=Smith%2CNG&author=Lercher%2CMJ&author=Ellegren%2CH)
    
37. Rosenberg, H. F. & Feldmann, M. W. _The Relationship Between Coalescence Times and Population Divergence Times_ (Oxford Univ. Press, Oxford, 2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20Relationship%20Between%20Coalescence%20Times%20and%20Population%20Divergence%20Times&publication_year=2002&author=Rosenberg%2CHF&author=Feldmann%2CMW)
    
38. Vignaud, P. et al. Geology and palaeontology of the Upper Miocene Toros-Menalla hominid locality, Chad. _Nature_ **418**, 152–155 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Geology%20and%20palaeontology%20of%20the%20Upper%20Miocene%20Toros-Menalla%20hominid%20locality%2C%20Chad&journal=Nature&volume=418&pages=152-155&publication_year=2002&author=Vignaud%2CP)
    
39. Wall, J. D. Estimating ancestral population sizes and divergence times. _Genetics_ **163**, 395–404 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1462435) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Estimating%20ancestral%20population%20sizes%20and%20divergence%20times&journal=Genetics&volume=163&pages=395-404&publication_year=2003&author=Wall%2CJD)
    
40. Reich, D. E. et al. Human genome sequence variation and the influence of gene history, mutation and recombination. _Nature Genet._ **32**, 135–142 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Human%20genome%20sequence%20variation%20and%20the%20influence%20of%20gene%20history%2C%20mutation%20and%20recombination&journal=Nature%20Genet.&volume=32&pages=135-142&publication_year=2002&author=Reich%2CDE)
    
41. Maynard Smith, J. M. & Haigh, J. The hitch-hiking effect of a favourable gene. _Genet. Res._ **23**, 23–35 (1974)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20hitch-hiking%20effect%20of%20a%20favourable%20gene&journal=Genet.%20Res.&volume=23&pages=23-35&publication_year=1974&author=Maynard%20Smith%2CJM&author=Haigh%2CJ)
    
42. Hudson, R. R. & Kaplan, N. L. Deleterious background selection with recombination. _Genetics_ **141**, 1605–1617 (1995)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1206891) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Deleterious%20background%20selection%20with%20recombination&journal=Genetics&volume=141&pages=1605-1617&publication_year=1995&author=Hudson%2CRR&author=Kaplan%2CNL)
    
43. Charlesworth, B. The effect of background selection against deleterious mutations on weakly selected, linked variants. _Genet. Res._ **63**, 213–227 (1994)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20effect%20of%20background%20selection%20against%20deleterious%20mutations%20on%20weakly%20selected%2C%20linked%20variants&journal=Genet.%20Res.&volume=63&pages=213-227&publication_year=1994&author=Charlesworth%2CB)
    
44. Birky, C. W. Jr & Walsh, J. B. Effects of linkage on rates of molecular evolution. _Proc. Natl Acad. Sci. USA_ **85**, 6414–6418 (1988)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC281982) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Effects%20of%20linkage%20on%20rates%20of%20molecular%20evolution&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=85&pages=6414-6418&publication_year=1988&author=Birky%2CCW&author=Walsh%2CJB)
    
45. Hellmann, I., Ebersberger, I., Ptak, S. E., Paabo, S. & Przeworski, M. A neutral explanation for the correlation of diversity with recombination rates in humans. _Am. J. Hum. Genet._ **72**, 1527–1535 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1180312) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20neutral%20explanation%20for%20the%20correlation%20of%20diversity%20with%20recombination%20rates%20in%20humans&journal=Am.%20J.%20Hum.%20Genet.&volume=72&pages=1527-1535&publication_year=2003&author=Hellmann%2CI&author=Ebersberger%2CI&author=Ptak%2CSE&author=Paabo%2CS&author=Przeworski%2CM)
    
46. Lercher, M. J. & Hurst, L. D. Human SNP variability and mutation rate are higher in regions of high recombination. _Trends Genet._ **18**, 337–340 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Human%20SNP%20variability%20and%20mutation%20rate%20are%20higher%20in%20regions%20of%20high%20recombination&journal=Trends%20Genet.&volume=18&pages=337-340&publication_year=2002&author=Lercher%2CMJ&author=Hurst%2CLD)
    
47. Hellmann, I. et al. Why do human diversity levels vary at a megabase scale? _Genome Res._ **15**, 1222–1231 (2005)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1199536) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Why%20do%20human%20diversity%20levels%20vary%20at%20a%20megabase%20scale%3F&journal=Genome%20Res.&volume=15&pages=1222-1231&publication_year=2005&author=Hellmann%2CI)
    
48. Li, W. H., Yi, S. & Makova, K. Male-driven evolution. _Curr. Opin. Genet. Dev._ **12**, 650–656 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Male-driven%20evolution&journal=Curr.%20Opin.%20Genet.%20Dev.&volume=12&pages=650-656&publication_year=2002&author=Li%2CWH&author=Yi%2CS&author=Makova%2CK)
    
49. Bohossian, H. B., Skaletsky, H. & Page, D. C. Unexpectedly similar rates of nucleotide substitution found in male and female hominids. _Nature_ **406**, 622–625 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Unexpectedly%20similar%20rates%20of%20nucleotide%20substitution%20found%20in%20male%20and%20female%20hominids&journal=Nature&volume=406&pages=622-625&publication_year=2000&author=Bohossian%2CHB&author=Skaletsky%2CH&author=Page%2CDC)
    
50. Makova, K. D. & Li, W. H. Strong male-driven evolution of DNA sequences in humans and apes. _Nature_ **416**, 624–626 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Strong%20male-driven%20evolution%20of%20DNA%20sequences%20in%20humans%20and%20apes&journal=Nature&volume=416&pages=624-626&publication_year=2002&author=Makova%2CKD&author=Li%2CWH)
    
51. Hwang, D. G. & Green, P. Bayesian Markov chain Monte Carlo sequence analysis reveals varying neutral substitution patterns in mammalian evolution. _Proc. Natl Acad. Sci. USA_ **101**, 13994–14001 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC521089) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Bayesian%20Markov%20chain%20Monte%20Carlo%20sequence%20analysis%20reveals%20varying%20neutral%20substitution%20patterns%20in%20mammalian%20evolution&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=101&pages=13994-14001&publication_year=2004&author=Hwang%2CDG&author=Green%2CP)
    
52. Taylor, J., Tyekucheva, S., Zody, M., Ciaromonte, F. & Makova, K. D. Strong and weak male mutation bias at different sites in the primate genomes: Insights from the human-chimpanzee comparison. _Mol. Biol. Evol._ (submitted)
53. Bulmer, M., Wolfe, K. H. & Sharp, P. M. Synonymous nucleotide substitution rates in mammalian genes: implications for the molecular clock and the relationship of mammalian orders. _Proc. Natl Acad. Sci. USA_ **88**, 5974–5978 (1991)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC52004) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Synonymous%20nucleotide%20substitution%20rates%20in%20mammalian%20genes%3A%20implications%20for%20the%20molecular%20clock%20and%20the%20relationship%20of%20mammalian%20orders&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=88&pages=5974-5978&publication_year=1991&author=Bulmer%2CM&author=Wolfe%2CKH&author=Sharp%2CPM)
    
54. Ehrlich, M., Zhang, X. Y. & Inamdar, N. M. Spontaneous deamination of cytosine and 5-methylcytosine residues in DNA and replacement of 5-methylcytosine residues with cytosine residues. _Mutat. Res._ **238**, 277–286 (1990)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Spontaneous%20deamination%20of%20cytosine%20and%205-methylcytosine%20residues%20in%20DNA%20and%20replacement%20of%205-methylcytosine%20residues%20with%20cytosine%20residues&journal=Mutat.%20Res.&volume=238&pages=277-286&publication_year=1990&author=Ehrlich%2CM&author=Zhang%2CXY&author=Inamdar%2CNM)
    
55. Craig, J. M. & Bickmore, W. A. Chromosome bands—flavours to savour. _Bioessays_ **15**, 349–354 (1993)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Chromosome%20bands%E2%80%94flavours%20to%20savour&journal=Bioessays&volume=15&pages=349-354&publication_year=1993&author=Craig%2CJM&author=Bickmore%2CWA)
    
56. Holmquist, G. P. Chromosome bands, their chromatin flavors, and their functional features. _Am. J. Hum. Genet._ **51**, 17–37 (1992)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1682890) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Chromosome%20bands%2C%20their%20chromatin%20flavors%2C%20and%20their%20functional%20features&journal=Am.%20J.%20Hum.%20Genet.&volume=51&pages=17-37&publication_year=1992&author=Holmquist%2CGP)
    
57. Ellegren, H., Smith, N. G. & Webster, M. T. Mutation rate variation in the mammalian genome. _Curr. Opin. Genet. Dev._ **13**, 562–568 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Mutation%20rate%20variation%20in%20the%20mammalian%20genome&journal=Curr.%20Opin.%20Genet.%20Dev.&volume=13&pages=562-568&publication_year=2003&author=Ellegren%2CH&author=Smith%2CNG&author=Webster%2CMT)
    
58. Cooper, G. M., Brudno, M., Green, E. D., Batzoglou, S. & Sidow, A. Quantitative estimates of sequence divergence for comparative analyses of mammalian genomes. _Genome Res._ **13**, 813–820 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430923) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Quantitative%20estimates%20of%20sequence%20divergence%20for%20comparative%20analyses%20of%20mammalian%20genomes&journal=Genome%20Res.&volume=13&pages=813-820&publication_year=2003&author=Cooper%2CGM&author=Brudno%2CM&author=Green%2CED&author=Batzoglou%2CS&author=Sidow%2CA)
    
59. Cooper, G. M. et al. Characterization of evolutionary rates and constraints in three mammalian genomes. _Genome Res._ **14**, 539–548 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC383297) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Characterization%20of%20evolutionary%20rates%20and%20constraints%20in%20three%20mammalian%20genomes&journal=Genome%20Res.&volume=14&pages=539-548&publication_year=2004&author=Cooper%2CGM)
    
60. Yang, S. et al. Patterns of insertions and their covariation with substitutions in the rat, mouse, and human genomes. _Genome Res._ **14**, 517–527 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC383295) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Patterns%20of%20insertions%20and%20their%20covariation%20with%20substitutions%20in%20the%20rat%2C%20mouse%2C%20and%20human%20genomes&journal=Genome%20Res.&volume=14&pages=517-527&publication_year=2004&author=Yang%2CS)
    
61. Birdsell, J. A. Integrating genomics, bioinformatics, and classical genetics to study the effects of recombination on genome evolution. _Mol. Biol. Evol._ **19**, 1181–1197 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Integrating%20genomics%2C%20bioinformatics%2C%20and%20classical%20genetics%20to%20study%20the%20effects%20of%20recombination%20on%20genome%20evolution&journal=Mol.%20Biol.%20Evol.&volume=19&pages=1181-1197&publication_year=2002&author=Birdsell%2CJA)
    
62. Jensen-Seaman, M. I. et al. Comparative recombination rates in the rat, mouse, and human genomes. _Genome Res._ **14**, 528–538 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC383296) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Comparative%20recombination%20rates%20in%20the%20rat%2C%20mouse%2C%20and%20human%20genomes&journal=Genome%20Res.&volume=14&pages=528-538&publication_year=2004&author=Jensen-Seaman%2CMI)
    
63. Fortna, A. et al. Lineage-specific gene duplication and loss in human and great ape evolution. _PLoS Biol._ **2**, E207 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC449870) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Lineage-specific%20gene%20duplication%20and%20loss%20in%20human%20and%20great%20ape%20evolution&journal=PLoS%20Biol.&volume=2&publication_year=2004&author=Fortna%2CA)
    
64. Britten, R. J. Divergence between samples of chimpanzee and human DNA sequences is 5%, counting indels. _Proc. Natl Acad. Sci. USA_ **99**, 13633–13635 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC129726) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Divergence%20between%20samples%20of%20chimpanzee%20and%20human%20DNA%20sequences%20is%205%25%2C%20counting%20indels&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=99&pages=13633-13635&publication_year=2002&author=Britten%2CRJ)
    
65. Frazer, K. A. et al. Genomic DNA insertions and deletions occur frequently between humans and nonhuman primates. _Genome Res._ **13**, 341–346 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430260) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genomic%20DNA%20insertions%20and%20deletions%20occur%20frequently%20between%20humans%20and%20nonhuman%20primates&journal=Genome%20Res.&volume=13&pages=341-346&publication_year=2003&author=Frazer%2CKA)
    
66. Locke, D. P. et al. Large-scale variation among human and great ape genomes determined by array comparative genomic hybridization. _Genome Res._ **13**, 347–357 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430292) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Large-scale%20variation%20among%20human%20and%20great%20ape%20genomes%20determined%20by%20array%20comparative%20genomic%20hybridization&journal=Genome%20Res.&volume=13&pages=347-357&publication_year=2003&author=Locke%2CDP)
    
67. Liu, G. et al. Analysis of primate genomic variation reveals a repeat-driven expansion of the human genome. _Genome Res._ **13**, 358–368 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430288) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Analysis%20of%20primate%20genomic%20variation%20reveals%20a%20repeat-driven%20expansion%20of%20the%20human%20genome&journal=Genome%20Res.&volume=13&pages=358-368&publication_year=2003&author=Liu%2CG)
    
68. Yohn, C. T. et al. Lineage-specific expansions of retroviral insertions within the genomes of African great apes but not humans and orangutans. _PLoS Biol._ **3**, 1–11 (2005)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Lineage-specific%20expansions%20of%20retroviral%20insertions%20within%20the%20genomes%20of%20African%20great%20apes%20but%20not%20humans%20and%20orangutans&journal=PLoS%20Biol.&volume=3&pages=1-11&publication_year=2005&author=Yohn%2CCT)
    
69. Hedges, D. J. et al. Differential alu mobilization and polymorphism among the human and chimpanzee lineages. _Genome Res._ **14**, 1068–1075 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC419785) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Differential%20alu%20mobilization%20and%20polymorphism%20among%20the%20human%20and%20chimpanzee%20lineages&journal=Genome%20Res.&volume=14&pages=1068-1075&publication_year=2004&author=Hedges%2CDJ)
    
70. Smit, A. F. Interspersed repeats and other mementos of transposable elements in mammalian genomes. _Curr. Opin. Genet. Dev._ **9**, 657–663 (1999)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Interspersed%20repeats%20and%20other%20mementos%20of%20transposable%20elements%20in%20mammalian%20genomes&journal=Curr.%20Opin.%20Genet.%20Dev.&volume=9&pages=657-663&publication_year=1999&author=Smit%2CAF)
    
71. Dewannieux, M., Esnault, C. & Heidmann, T. LINE-mediated retrotransposition of marked Alu sequences. _Nature Genet._ **35**, 41–48 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=LINE-mediated%20retrotransposition%20of%20marked%20Alu%20sequences&journal=Nature%20Genet.&volume=35&pages=41-48&publication_year=2003&author=Dewannieux%2CM&author=Esnault%2CC&author=Heidmann%2CT)
    
72. Mathews, L. M., Chi, S. Y., Greenberg, N., Ovchinnikov, I. & Swergold, G. D. Large differences between LINE-1 amplification rates in the human and chimpanzee lineages. _Am. J. Hum. Genet._ **72**, 739–748 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1180250) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Large%20differences%20between%20LINE-1%20amplification%20rates%20in%20the%20human%20and%20chimpanzee%20lineages&journal=Am.%20J.%20Hum.%20Genet.&volume=72&pages=739-748&publication_year=2003&author=Mathews%2CLM&author=Chi%2CSY&author=Greenberg%2CN&author=Ovchinnikov%2CI&author=Swergold%2CGD)
    
73. Pickeral, O. K., Makalowski, W., Boguski, M. S. & Boeke, J. D. Frequent human genomic DNA transduction driven by LINE-1 retrotransposition. _Genome Res._ **10**, 411–415 (2000)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC310862) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Frequent%20human%20genomic%20DNA%20transduction%20driven%20by%20LINE-1%20retrotransposition&journal=Genome%20Res.&volume=10&pages=411-415&publication_year=2000&author=Pickeral%2COK&author=Makalowski%2CW&author=Boguski%2CMS&author=Boeke%2CJD)
    
74. Goodier, J. L., Ostertag, E. M. & Kazazian, H. H. Jr Transduction of 3′-flanking sequences is common in L1 retrotransposition. _Hum. Mol. Genet._ **9**, 653–657 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Transduction%20of%203%E2%80%B2-flanking%20sequences%20is%20common%20in%20L1%20retrotransposition&journal=Hum.%20Mol.%20Genet.&volume=9&pages=653-657&publication_year=2000&author=Goodier%2CJL&author=Ostertag%2CEM&author=Kazazian%2CHH)
    
75. Zhang, Z., Harrison, P. M., Liu, Y. & Gerstein, M. Millions of years of evolution preserved: a comprehensive catalog of the processed pseudogenes in the human genome. _Genome Res._ **13**, 2541–2558 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC403796) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Millions%20of%20years%20of%20evolution%20preserved%3A%20a%20comprehensive%20catalog%20of%20the%20processed%20pseudogenes%20in%20the%20human%20genome&journal=Genome%20Res.&volume=13&pages=2541-2558&publication_year=2003&author=Zhang%2CZ&author=Harrison%2CPM&author=Liu%2CY&author=Gerstein%2CM)
    
76. Torrents, D., Suyama, M., Zdobnov, E. & Bork, P. A genome-wide survey of human pseudogenes. _Genome Res._ **13**, 2559–2567 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC403797) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20genome-wide%20survey%20of%20human%20pseudogenes&journal=Genome%20Res.&volume=13&pages=2559-2567&publication_year=2003&author=Torrents%2CD&author=Suyama%2CM&author=Zdobnov%2CE&author=Bork%2CP)
    
77. Esnault, C., Maestre, J. & Heidmann, T. Human LINE retrotransposons generate processed pseudogenes. _Nature Genet._ **24**, 363–367 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Human%20LINE%20retrotransposons%20generate%20processed%20pseudogenes&journal=Nature%20Genet.&volume=24&pages=363-367&publication_year=2000&author=Esnault%2CC&author=Maestre%2CJ&author=Heidmann%2CT)
    
78. Zhang, Z., Harrison, P. & Gerstein, M. Identification and analysis of over 2000 ribosomal protein pseudogenes in the human genome. _Genome Res._ **12**, 1466–1482 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC187539) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Identification%20and%20analysis%20of%20over%202000%20ribosomal%20protein%20pseudogenes%20in%20the%20human%20genome&journal=Genome%20Res.&volume=12&pages=1466-1482&publication_year=2002&author=Zhang%2CZ&author=Harrison%2CP&author=Gerstein%2CM)
    
79. Ostertag, E. M., Goodier, J. L., Zhang, Y. & Kazazian, H. H. Jr SVA elements are nonautonomous retrotransposons that cause disease in humans. _Am. J. Hum. Genet._ **73**, 1444–1451 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1180407) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=SVA%20elements%20are%20nonautonomous%20retrotransposons%20that%20cause%20disease%20in%20humans&journal=Am.%20J.%20Hum.%20Genet.&volume=73&pages=1444-1451&publication_year=2003&author=Ostertag%2CEM&author=Goodier%2CJL&author=Zhang%2CY&author=Kazazian%2CHH)
    
80. Shen, L. et al. Structure and genetics of the partially duplicated gene RP located immediately upstream of the complement C4A and the C4B genes in the HLA class III region. Molecular cloning, exon-intron structure, composite retroposon, and breakpoint of gene duplication. _J. Biol. Chem._ **269**, 8466–8476 (1994)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Structure%20and%20genetics%20of%20the%20partially%20duplicated%20gene%20RP%20located%20immediately%20upstream%20of%20the%20complement%20C4A%20and%20the%20C4B%20genes%20in%20the%20HLA%20class%20III%20region.%20Molecular%20cloning%2C%20exon-intron%20structure%2C%20composite%20retroposon%2C%20and%20breakpoint%20of%20gene%20duplication&journal=J.%20Biol.%20Chem.&volume=269&pages=8466-8476&publication_year=1994&author=Shen%2CL)
    
81. Takai, D. & Jones, P. A. Comprehensive analysis of CpG islands in human chromosomes 21 and 22. _Proc. Natl Acad. Sci. USA_ **99**, 3740–3745 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC122594) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Comprehensive%20analysis%20of%20CpG%20islands%20in%20human%20chromosomes%2021%20and%2022&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=99&pages=3740-3745&publication_year=2002&author=Takai%2CD&author=Jones%2CPA)
    
82. Enard, W. et al. Intra- and interspecific variation in primate gene expression patterns. _Science_ **296**, 340–343 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Intra-%20and%20interspecific%20variation%20in%20primate%20gene%20expression%20patterns&journal=Science&volume=296&pages=340-343&publication_year=2002&author=Enard%2CW)
    
83. Khaitovich, P. et al. Parallel patterns of evolution in the genomes and transcriptomes of humans and chimpanzees. _Science_(in the press)
84. Yunis, J. J., Sawyer, J. R. & Dunham, K. The striking resemblance of high-resolution G-banded chromosomes of man and chimpanzee. _Science_ **208**, 1145–1148 (1980)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20striking%20resemblance%20of%20high-resolution%20G-banded%20chromosomes%20of%20man%20and%20chimpanzee&journal=Science&volume=208&pages=1145-1148&publication_year=1980&author=Yunis%2CJJ&author=Sawyer%2CJR&author=Dunham%2CK)
    
85. Fan, Y., Linardopoulou, E., Friedman, C., Williams, E. & Trask, B. J. Genomic structure and evolution of the ancestral chromosome fusion site in 2q13-2q14.1 and paralogous regions on other human chromosomes. _Genome Res._ **12**, 1651–1662 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC187548) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genomic%20structure%20and%20evolution%20of%20the%20ancestral%20chromosome%20fusion%20site%20in%202q13-2q14.1%20and%20paralogous%20regions%20on%20other%20human%20chromosomes&journal=Genome%20Res.&volume=12&pages=1651-1662&publication_year=2002&author=Fan%2CY&author=Linardopoulou%2CE&author=Friedman%2CC&author=Williams%2CE&author=Trask%2CBJ)
    
86. Fan, Y., Newman, T., Linardopoulou, E. & Trask, B. J. Gene content and function of the ancestral chromosome fusion site in human chromosome 2q13-2q14.1 and paralogous regions. _Genome Res._ **12**, 1663–1672 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC187549) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Gene%20content%20and%20function%20of%20the%20ancestral%20chromosome%20fusion%20site%20in%20human%20chromosome%202q13-2q14.1%20and%20paralogous%20regions&journal=Genome%20Res.&volume=12&pages=1663-1672&publication_year=2002&author=Fan%2CY&author=Newman%2CT&author=Linardopoulou%2CE&author=Trask%2CBJ)
    
87. Locke, D. P. et al. Refinement of a chimpanzee pericentric inversion breakpoint to a segmental duplication cluster. _Genome Biol._ **4**, R50 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC193642) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Refinement%20of%20a%20chimpanzee%20pericentric%20inversion%20breakpoint%20to%20a%20segmental%20duplication%20cluster&journal=Genome%20Biol.&volume=4&publication_year=2003&author=Locke%2CDP)
    
88. Dennehey, B. K., Gutches, D. G., McConkey, E. H. & Krauter, K. S. Inversion, duplication, and changes in gene context are associated with human chromosome 18 evolution. _Genomics_ **83**, 493–501 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Inversion%2C%20duplication%2C%20and%20changes%20in%20gene%20context%20are%20associated%20with%20human%20chromosome%2018%20evolution&journal=Genomics&volume=83&pages=493-501&publication_year=2004&author=Dennehey%2CBK&author=Gutches%2CDG&author=McConkey%2CEH&author=Krauter%2CKS)
    
89. Subramanian, S. & Kumar, S. Neutral substitutions occur at a faster rate in exons than in noncoding DNA in primate genomes. _Genome Res._ **13**, 838–844 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430942) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Neutral%20substitutions%20occur%20at%20a%20faster%20rate%20in%20exons%20than%20in%20noncoding%20DNA%20in%20primate%20genomes&journal=Genome%20Res.&volume=13&pages=838-844&publication_year=2003&author=Subramanian%2CS&author=Kumar%2CS)
    
90. Duret, L. Detecting genomic features under weak selective pressure: the example of codon usage in animals and plants. _Bioinformatics_ **18** (suppl. 2), S91 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Detecting%20genomic%20features%20under%20weak%20selective%20pressure%3A%20the%20example%20of%20codon%20usage%20in%20animals%20and%20plants&journal=Bioinformatics&volume=18&issue=suppl.%202&publication_year=2002&author=Duret%2CL)
    
91. Sharp, P. M. & Li, W. H. Codon usage in regulatory genes in _Escherichia coli_ does not reflect selection for ‘rare’ codons. _Nucleic Acids Res._ **14**, 7737–7749 (1986)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC311793) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Codon%20usage%20in%20regulatory%20genes%20in%20Escherichia%20coli%20does%20not%20reflect%20selection%20for%20%E2%80%98rare%E2%80%99%20codons&journal=Nucleic%20Acids%20Res.&volume=14&pages=7737-7749&publication_year=1986&author=Sharp%2CPM&author=Li%2CWH)
    
92. Sharp, P. M., Averof, M., Lloyd, A. T., Matassi, G. & Peden, J. F. DNA sequence evolution: the sounds of silence. _Phil. Trans. R. Soc. Lond. B_ **349**, 241–247 (1995)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=DNA%20sequence%20evolution%3A%20the%20sounds%20of%20silence&journal=Phil.%20Trans.%20R.%20Soc.%20Lond.%20B&volume=349&pages=241-247&publication_year=1995&author=Sharp%2CPM&author=Averof%2CM&author=Lloyd%2CAT&author=Matassi%2CG&author=Peden%2CJF)
    
93. Moriyama, E. N. & Powell, J. R. Synonymous substitution rates in _Drosophila_: mitochondrial versus nuclear genes. _J. Mol. Evol._ **45**, 378–391 (1997)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Synonymous%20substitution%20rates%20in%20Drosophila%3A%20mitochondrial%20versus%20nuclear%20genes&journal=J.%20Mol.%20Evol.&volume=45&pages=378-391&publication_year=1997&author=Moriyama%2CEN&author=Powell%2CJR)
    
94. McVean, G. A. et al. The fine-scale structure of recombination rate variation in the human genome. _Science_ **304**, 581–584 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20fine-scale%20structure%20of%20recombination%20rate%20variation%20in%20the%20human%20genome&journal=Science&volume=304&pages=581-584&publication_year=2004&author=McVean%2CGA)
    
95. Ohta, T. Slightly deleterious mutant substitutions during evolution. _Nature_ **246**, 96–98 (1973)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Slightly%20deleterious%20mutant%20substitutions%20during%20evolution&journal=Nature&volume=246&pages=96-98&publication_year=1973&author=Ohta%2CT)
    
96. Ohta, T. Synonymous and nonsynonymous substitutions in mammalian genes and the nearly neutral theory. _J. Mol. Evol._ **40**, 56–63 (1995)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Synonymous%20and%20nonsynonymous%20substitutions%20in%20mammalian%20genes%20and%20the%20nearly%20neutral%20theory&journal=J.%20Mol.%20Evol.&volume=40&pages=56-63&publication_year=1995&author=Ohta%2CT)
    
97. Eyre-Walker, A., Keightley, P. D., Smith, N. G. & Gaffney, D. Quantifying the slightly deleterious mutation model of molecular evolution. _Mol. Biol. Evol._ **19**, 2142–2149 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Quantifying%20the%20slightly%20deleterious%20mutation%20model%20of%20molecular%20evolution&journal=Mol.%20Biol.%20Evol.&volume=19&pages=2142-2149&publication_year=2002&author=Eyre-Walker%2CA&author=Keightley%2CPD&author=Smith%2CNG&author=Gaffney%2CD)
    
98. Makalowski, W. & Boguski, M. S. Synonymous and nonsynonymous substitution distances are correlated in mouse and rat genes. _J. Mol. Evol._ **47**, 119–121 (1998)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Synonymous%20and%20nonsynonymous%20substitution%20distances%20are%20correlated%20in%20mouse%20and%20rat%20genes&journal=J.%20Mol.%20Evol.&volume=47&pages=119-121&publication_year=1998&author=Makalowski%2CW&author=Boguski%2CMS)
    
99. McDonald, J. H. & Kreitman, M. Adaptive protein evolution at the Adh locus in _Drosophila_. _Nature_ **351**, 652–654 (1991)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Adaptive%20protein%20evolution%20at%20the%20Adh%20locus%20in%20Drosophila&journal=Nature&volume=351&pages=652-654&publication_year=1991&author=McDonald%2CJH&author=Kreitman%2CM)
    
100. Sawyer, S. A. & Hartl, D. L. Population genetics of polymorphism and divergence. _Genetics_ **132**, 1161–1176 (1992)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1205236) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Population%20genetics%20of%20polymorphism%20and%20divergence&journal=Genetics&volume=132&pages=1161-1176&publication_year=1992&author=Sawyer%2CSA&author=Hartl%2CDL)
    
101. Maier, A. G. et al. _Plasmodium falciparum_ erythrocyte invasion through glycophorin C and selection for Gerbich negativity in human populations. _Nature Med._ **9**, 87–92 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Plasmodium%20falciparum%20erythrocyte%20invasion%20through%20glycophorin%20C%20and%20selection%20for%20Gerbich%20negativity%20in%20human%20populations&journal=Nature%20Med.&volume=9&pages=87-92&publication_year=2003&author=Maier%2CAG)
    
102. Stenger, S. et al. An antimicrobial activity of cytolytic T cells mediated by granulysin. _Science_ **282**, 121–125 (1998)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=An%20antimicrobial%20activity%20of%20cytolytic%20T%20cells%20mediated%20by%20granulysin&journal=Science&volume=282&pages=121-125&publication_year=1998&author=Stenger%2CS)
    
103. Swanson, W. J. & Vacquier, V. D. The rapid evolution of reproductive proteins. _Nature Rev. Genet._ **3**, 137–144 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20rapid%20evolution%20of%20reproductive%20proteins&journal=Nature%20Rev.%20Genet.&volume=3&pages=137-144&publication_year=2002&author=Swanson%2CWJ&author=Vacquier%2CVD)
    
104. Choi, S. S. & Lahn, B. T. Adaptive evolution of _MRG_, a neuron-specific gene family implicated in nociception. _Genome Res._ **13**, 2252–2259 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC403691) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Adaptive%20evolution%20of%20MRG%2C%20a%20neuron-specific%20gene%20family%20implicated%20in%20nociception&journal=Genome%20Res.&volume=13&pages=2252-2259&publication_year=2003&author=Choi%2CSS&author=Lahn%2CBT)
    
105. Hardison, R. C. et al. Global predictions and tests of erythroid regulatory regions. _Cold Spring Harb. Symp. Quant. Biol._ **68**, 335–344 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Global%20predictions%20and%20tests%20of%20erythroid%20regulatory%20regions&journal=Cold%20Spring%20Harb.%20Symp.%20Quant.%20Biol.&volume=68&pages=335-344&publication_year=2003&author=Hardison%2CRC)
    
106. Lercher, M. J., Chamary, J. V. & Hurst, L. D. Genomic regionality in rates of evolution is not explained by clustering of genes of comparable expression profile. _Genome Res._ **14**, 1002–1013 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC419778) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genomic%20regionality%20in%20rates%20of%20evolution%20is%20not%20explained%20by%20clustering%20of%20genes%20of%20comparable%20expression%20profile&journal=Genome%20Res.&volume=14&pages=1002-1013&publication_year=2004&author=Lercher%2CMJ&author=Chamary%2CJV&author=Hurst%2CLD)
    
107. Williams, E. J. & Hurst, L. D. The proteins of linked genes evolve at similar rates. _Nature_ **407**, 900–903 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20proteins%20of%20linked%20genes%20evolve%20at%20similar%20rates&journal=Nature&volume=407&pages=900-903&publication_year=2000&author=Williams%2CEJ&author=Hurst%2CLD)
    
108. Navarro, A. & Barton, N. H. Chromosomal speciation and molecular divergence—accelerated evolution in rearranged chromosomes. _Science_ **300**, 321–324 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Chromosomal%20speciation%20and%20molecular%20divergence%E2%80%94accelerated%20evolution%20in%20rearranged%20chromosomes&journal=Science&volume=300&pages=321-324&publication_year=2003&author=Navarro%2CA&author=Barton%2CNH)
    
109. Zhang, J., Wang, X. & Podlaha, O. Testing the chromosomal speciation hypothesis for humans and chimpanzees. _Genome Res._ **14**, 845–851 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC479111) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Testing%20the%20chromosomal%20speciation%20hypothesis%20for%20humans%20and%20chimpanzees&journal=Genome%20Res.&volume=14&pages=845-851&publication_year=2004&author=Zhang%2CJ&author=Wang%2CX&author=Podlaha%2CO)
    
110. Lu, J., Li, W. H. & Wu, C. I. Comment on “Chromosomal speciation and molecular divergence-accelerated evolution in rearranged chromosomes”. _Science_ **302**, 988 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Comment%20on%20%E2%80%9CChromosomal%20speciation%20and%20molecular%20divergence-accelerated%20evolution%20in%20rearranged%20chromosomes%E2%80%9D&journal=Science&volume=302&publication_year=2003&author=Lu%2CJ&author=Li%2CWH&author=Wu%2CCI)
    
111. Charlesworth, B., Coyne, J. A. & Orr, H. A. Meiotic drive and unisexual hybrid sterility: a comment. _Genetics_ **133**, 421–432 (1993)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1205330) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Meiotic%20drive%20and%20unisexual%20hybrid%20sterility%3A%20a%20comment&journal=Genetics&volume=133&pages=421-432&publication_year=1993&author=Charlesworth%2CB&author=Coyne%2CJA&author=Orr%2CHA)
    
112. Ohno, S. _Evolution by Gene Duplication_ (Springer, New York, 1970)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Evolution%20by%20Gene%20Duplication&publication_year=1970&author=Ohno%2CS)
    
113. Angata, T., Margulies, E. H., Green, E. D. & Varki, A. Large-scale sequencing of the CD33-related Siglec gene cluster in five mammalian species reveals rapid evolution by multiple mechanisms. _Proc. Natl Acad. Sci. USA_ **101**, 13251–13256 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC516556) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Large-scale%20sequencing%20of%20the%20CD33-related%20Siglec%20gene%20cluster%20in%20five%20mammalian%20species%20reveals%20rapid%20evolution%20by%20multiple%20mechanisms&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=101&pages=13251-13256&publication_year=2004&author=Angata%2CT&author=Margulies%2CEH&author=Green%2CED&author=Varki%2CA)
    
114. Teumer, J. & Green, H. Divergent evolution of part of the involucrin gene in the hominoids: unique intragenic duplications in the gorilla and human. _Proc. Natl Acad. Sci. USA_ **86**, 1283–1286 (1989)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC286672) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Divergent%20evolution%20of%20part%20of%20the%20involucrin%20gene%20in%20the%20hominoids%3A%20unique%20intragenic%20duplications%20in%20the%20gorilla%20and%20human&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=86&pages=1283-1286&publication_year=1989&author=Teumer%2CJ&author=Green%2CH)
    
115. Ashburner, M. et al. Gene ontology: tool for the unification of biology. The Gene Ontology Consortium. _Nature Genet._ **25**, 25–29 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Gene%20ontology%3A%20tool%20for%20the%20unification%20of%20biology.%20The%20Gene%20Ontology%20Consortium&journal=Nature%20Genet.&volume=25&pages=25-29&publication_year=2000&author=Ashburner%2CM)
    
116. Yang, Z. & Bielawski, J. P. Statistical methods for detecting molecular adaptation. _Trends Ecol. Evol._ **15**, 496–503 (2000)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC7134603) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Statistical%20methods%20for%20detecting%20molecular%20adaptation&journal=Trends%20Ecol.%20Evol.&volume=15&pages=496-503&publication_year=2000&author=Yang%2CZ&author=Bielawski%2CJP)
    
117. Weinreich, D. M. The rates of molecular evolution in rodent and primate mitochondrial DNA. _J. Mol. Evol._ **52**, 40–50 (2001)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20rates%20of%20molecular%20evolution%20in%20rodent%20and%20primate%20mitochondrial%20DNA&journal=J.%20Mol.%20Evol.&volume=52&pages=40-50&publication_year=2001&author=Weinreich%2CDM)
    
118. Dorus, S. et al. Accelerated evolution of nervous system genes in the origin of _Homo sapiens_. _Cell_ **119**, 1027–1040 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Accelerated%20evolution%20of%20nervous%20system%20genes%20in%20the%20origin%20of%20Homo%20sapiens&journal=Cell&volume=119&pages=1027-1040&publication_year=2004&author=Dorus%2CS)
    
119. Neilsen, R. et al. A scan for positively selected genes in the genomes of humans and chimpanzees. _PLoS Biol._ **3**, e170 (2005)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20scan%20for%20positively%20selected%20genes%20in%20the%20genomes%20of%20humans%20and%20chimpanzees&journal=PLoS%20Biol.&volume=3&publication_year=2005&author=Neilsen%2CR)
    
120. Vallender, E. J. & Lahn, B. T. Positive selection on the human genome. _Hum. Mol. Genet._ **13** (suppl. 2), R245–R254 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Positive%20selection%20on%20the%20human%20genome&journal=Hum.%20Mol.%20Genet.&volume=13&issue=suppl.%202&pages=R245-R254&publication_year=2004&author=Vallender%2CEJ&author=Lahn%2CBT)
    
121. Gilad, Y., Man, O. & Glusman, G. A comparison of the human and chimpanzee olfactory receptor gene repertoires. _Genome Res._ **15**, 224–230 (2005)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC546523) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20comparison%20of%20the%20human%20and%20chimpanzee%20olfactory%20receptor%20gene%20repertoires&journal=Genome%20Res.&volume=15&pages=224-230&publication_year=2005&author=Gilad%2CY&author=Man%2CO&author=Glusman%2CG)
    
122. Enard, W. & Paabo, S. Comparative primate genomics. _Annu. Rev. Genomics Hum. Genet._ **5**, 351–378 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Comparative%20primate%20genomics&journal=Annu.%20Rev.%20Genomics%20Hum.%20Genet.&volume=5&pages=351-378&publication_year=2004&author=Enard%2CW&author=Paabo%2CS)
    
123. Saleh, M. et al. Differential modulation of endotoxin responsiveness by human caspase-12 polymorphisms. _Nature_ **429**, 75–79 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Differential%20modulation%20of%20endotoxin%20responsiveness%20by%20human%20caspase-12%20polymorphisms&journal=Nature&volume=429&pages=75-79&publication_year=2004&author=Saleh%2CM)
    
124. Fischer, H., Koenig, U., Eckhart, L. & Tschachler, E. Human caspase 12 has acquired deleterious mutations. _Biochem. Biophys. Res. Commun._ **293**, 722–726 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Human%20caspase%2012%20has%20acquired%20deleterious%20mutations&journal=Biochem.%20Biophys.%20Res.%20Commun.&volume=293&pages=722-726&publication_year=2002&author=Fischer%2CH&author=Koenig%2CU&author=Eckhart%2CL&author=Tschachler%2CE)
    
125. Puente, X. S., Sanchez, L. M., Overall, C. M. & Lopez-Otin, C. Human and mouse proteases: a comparative genomic approach. _Nature Rev. Genet._ **4**, 544–558 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Human%20and%20mouse%20proteases%3A%20a%20comparative%20genomic%20approach&journal=Nature%20Rev.%20Genet.&volume=4&pages=544-558&publication_year=2003&author=Puente%2CXS&author=Sanchez%2CLM&author=Overall%2CCM&author=Lopez-Otin%2CC)
    
126. Nakagawa, T. et al. Caspase-12 mediates endoplasmic-reticulum-specific apoptosis and cytotoxicity by amyloid-β. _Nature_ **403**, 98–103 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Caspase-12%20mediates%20endoplasmic-reticulum-specific%20apoptosis%20and%20cytotoxicity%20by%20amyloid-%CE%B2&journal=Nature&volume=403&pages=98-103&publication_year=2000&author=Nakagawa%2CT)
    
127. Humke, E. W., Shriver, S. K., Starovasnik, M. A., Fairbrother, W. J. & Dixit, V. M. ICEBERG: a novel inhibitor of interleukin-1β generation. _Cell_ **103**, 99–111 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=ICEBERG%3A%20a%20novel%20inhibitor%20of%20interleukin-1%CE%B2%20generation&journal=Cell&volume=103&pages=99-111&publication_year=2000&author=Humke%2CEW&author=Shriver%2CSK&author=Starovasnik%2CMA&author=Fairbrother%2CWJ&author=Dixit%2CVM)
    
128. Vanhamme, L. et al. Apolipoprotein L-I is the trypanosome lytic factor of human serum. _Nature_ **422**, 83–87 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Apolipoprotein%20L-I%20is%20the%20trypanosome%20lytic%20factor%20of%20human%20serum&journal=Nature&volume=422&pages=83-87&publication_year=2003&author=Vanhamme%2CL)
    
129. Seed, J. R., Sechelski, J. B. & Loomis, M. R. A survey for a trypanocidal factor in primate sera. _J. Protozool._ **37**, 393–400 (1990)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20survey%20for%20a%20trypanocidal%20factor%20in%20primate%20sera&journal=J.%20Protozool.&volume=37&pages=393-400&publication_year=1990&author=Seed%2CJR&author=Sechelski%2CJB&author=Loomis%2CMR)
    
130. Angata, T. & Varki, A. Chemical diversity in the sialic acids and related α-keto acids: an evolutionary perspective. _Chem. Rev._ **102**, 439–469 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Chemical%20diversity%20in%20the%20sialic%20acids%20and%20related%20%CE%B1-keto%20acids%3A%20an%20evolutionary%20perspective&journal=Chem.%20Rev.&volume=102&pages=439-469&publication_year=2002&author=Angata%2CT&author=Varki%2CA)
    
131. Varki, A. How to make an ape brain. _Nature Genet._ **36**, 1034–1036 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=How%20to%20make%20an%20ape%20brain&journal=Nature%20Genet.&volume=36&pages=1034-1036&publication_year=2004&author=Varki%2CA)
    
132. Sonnenburg, J. L., Altheide, T. K. & Varki, A. A uniquely human consequence of domain-specific functional adaptation in a sialic acid-binding receptor. _Glycobiology_ **14**, 339–346 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20uniquely%20human%20consequence%20of%20domain-specific%20functional%20adaptation%20in%20a%20sialic%20acid-binding%20receptor&journal=Glycobiology&volume=14&pages=339-346&publication_year=2004&author=Sonnenburg%2CJL&author=Altheide%2CTK&author=Varki%2CA)
    
133. Pangburn, M. K. Host recognition and target differentiation by factor H, a regulator of the alternative pathway of complement. _Immunopharmacology_ **49**, 149–157 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Host%20recognition%20and%20target%20differentiation%20by%20factor%20H%2C%20a%20regulator%20of%20the%20alternative%20pathway%20of%20complement&journal=Immunopharmacology&volume=49&pages=149-157&publication_year=2000&author=Pangburn%2CMK)
    
134. Hayakawa, T. et al. Human-specific gene in microglia. _Science_(in the press)
135. Kondrashov, A. S., Sunyaev, S. & Kondrashov, F. A. Dobzhansky-Muller incompatibilities in protein evolution. _Proc. Natl Acad. Sci. USA_ **99**, 14878–14883 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC137512) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Dobzhansky-Muller%20incompatibilities%20in%20protein%20evolution&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=99&pages=14878-14883&publication_year=2002&author=Kondrashov%2CAS&author=Sunyaev%2CS&author=Kondrashov%2CFA)
    
136. Kulathinal, R. J., Bettencourt, B. R. & Hartl, D. L. Compensated deleterious mutations in insect genomes. _Science_ **306**, 1553–1554 (2004)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Compensated%20deleterious%20mutations%20in%20insect%20genomes&journal=Science&volume=306&pages=1553-1554&publication_year=2004&author=Kulathinal%2CRJ&author=Bettencourt%2CBR&author=Hartl%2CDL)
    
137. Pfutzer, R. et al. Novel cationic trypsinogen (PRSS1) N29T and R122C mutations cause autosomal dominant hereditary pancreatitis. _Gut_ **50**, 271–272 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1773118) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Novel%20cationic%20trypsinogen%20%28PRSS1%29%20N29T%20and%20R122C%20mutations%20cause%20autosomal%20dominant%20hereditary%20pancreatitis&journal=Gut&volume=50&pages=271-272&publication_year=2002&author=Pfutzer%2CR)
    
138. Chen, J. M., Montier, T. & Ferec, C. Molecular pathology and evolutionary and physiological implications of pancreatitis-associated cationic trypsinogen mutations. _Hum. Genet._ **109**, 245–252 (2001)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Molecular%20pathology%20and%20evolutionary%20and%20physiological%20implications%20of%20pancreatitis-associated%20cationic%20trypsinogen%20mutations&journal=Hum.%20Genet.&volume=109&pages=245-252&publication_year=2001&author=Chen%2CJM&author=Montier%2CT&author=Ferec%2CC)
    
139. Altshuler, D. et al. The common PPARγ Pro12Ala polymorphism is associated with decreased risk of type 2 diabetes. _Nature Genet._ **26**, 76–80 (2000)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20common%20PPAR%CE%B3%20Pro12Ala%20polymorphism%20is%20associated%20with%20decreased%20risk%20of%20type%202%20diabetes&journal=Nature%20Genet.&volume=26&pages=76-80&publication_year=2000&author=Altshuler%2CD)
    
140. Neel, J. V. Diabetes mellitus: a “thrifty” genotype rendered detrimental by “progress”? _Am. J. Hum. Genet._ **14**, 353–362 (1962)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1932342) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Diabetes%20mellitus%3A%20a%20%E2%80%9Cthrifty%E2%80%9D%20genotype%20rendered%20detrimental%20by%20%E2%80%9Cprogress%E2%80%9D%3F&journal=Am.%20J.%20Hum.%20Genet.&volume=14&pages=353-362&publication_year=1962&author=Neel%2CJV)
    
141. The International HapMap Consortium. The International HapMap Project. _Nature_ **426**, 789–796 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20International%20HapMap%20Project&journal=Nature&volume=426&pages=789-796&publication_year=2003)
    
142. Hacia, J. G. et al. Determination of ancestral alleles for human single-nucleotide polymorphisms using high-density oligonucleotide arrays. _Nature Genet._ **22**, 164–167 (1999)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Determination%20of%20ancestral%20alleles%20for%20human%20single-nucleotide%20polymorphisms%20using%20high-density%20oligonucleotide%20arrays&journal=Nature%20Genet.&volume=22&pages=164-167&publication_year=1999&author=Hacia%2CJG)
    
143. Watterson, G. A. & Guess, H. A. Is the most frequent allele the oldest? _Theor. Popul. Biol._ **11**, 141–160 (1977)
    
    [MATH](http://www.emis.de/MATH-item?0361.92017) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Is%20the%20most%20frequent%20allele%20the%20oldest%3F&journal=Theor.%20Popul.%20Biol.&volume=11&pages=141-160&publication_year=1977&author=Watterson%2CGA&author=Guess%2CHA)
    
144. Przeworski, M. The signature of positive selection at randomly chosen loci. _Genetics_ **160**, 1179–1189 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1462030) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20signature%20of%20positive%20selection%20at%20randomly%20chosen%20loci&journal=Genetics&volume=160&pages=1179-1189&publication_year=2002&author=Przeworski%2CM)
    
145. Stone, S. et al. A major predisposition locus for severe obesity, at 4p15-p14. _Am. J. Hum. Genet._ **70**, 1459–1468 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC379132) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20major%20predisposition%20locus%20for%20severe%20obesity%2C%20at%204p15-p14&journal=Am.%20J.%20Hum.%20Genet.&volume=70&pages=1459-1468&publication_year=2002&author=Stone%2CS)
    
146. Arya, R. et al. Evidence of a novel quantitative-trait locus for obesity on chromosome 4p in Mexican Americans. _Am. J. Hum. Genet._ **74**, 272–282 (2004)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1181925) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Evidence%20of%20a%20novel%20quantitative-trait%20locus%20for%20obesity%20on%20chromosome%204p%20in%20Mexican%20Americans&journal=Am.%20J.%20Hum.%20Genet.&volume=74&pages=272-282&publication_year=2004&author=Arya%2CR)
    
147. Enard, W. et al. Molecular evolution of _FOXP2_, a gene involved in speech and language. _Nature_ **418**, 869–872 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Molecular%20evolution%20of%20FOXP2%2C%20a%20gene%20involved%20in%20speech%20and%20language&journal=Nature&volume=418&pages=869-872&publication_year=2002&author=Enard%2CW)
    
148. Schroeder, S. A., Gaughan, D. M. & Swift, M. Protection against bronchial asthma by _CFTR_ ΔF508 mutation: a heterozygote advantage in cystic fibrosis. _Nature Med._ **1**, 703–705 (1995)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Protection%20against%20bronchial%20asthma%20by%20CFTR%20%CE%94F508%20mutation%3A%20a%20heterozygote%20advantage%20in%20cystic%20fibrosis&journal=Nature%20Med.&volume=1&pages=703-705&publication_year=1995&author=Schroeder%2CSA&author=Gaughan%2CDM&author=Swift%2CM)
    
149. Ohta, T. Evolution by nearly-neutral mutations. _Genetica_ **102–103**, 83–90 (1998)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Evolution%20by%20nearly-neutral%20mutations&journal=Genetica&volume=102%E2%80%93103&pages=83-90&publication_year=1998&author=Ohta%2CT)
    
150. Hayakawa, T., Altheide, T. K. & Varki, A. Genetic basis of human brain evolution: accelerating along the primate speedway. _Dev. Cell_ **8**, 2–4 (2005)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genetic%20basis%20of%20human%20brain%20evolution%3A%20accelerating%20along%20the%20primate%20speedway&journal=Dev.%20Cell&volume=8&pages=2-4&publication_year=2005&author=Hayakawa%2CT&author=Altheide%2CTK&author=Varki%2CA)
    
151. Keightley, P. D., Lercher, M. J. & Eyre-Walker, A. Evidence for widespread degradation of gene control regions in hominid genomes. _PLoS Biol._ **3**, e42 (2005)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC544929) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Evidence%20for%20widespread%20degradation%20of%20gene%20control%20regions%20in%20hominid%20genomes&journal=PLoS%20Biol.&volume=3&publication_year=2005&author=Keightley%2CPD&author=Lercher%2CMJ&author=Eyre-Walker%2CA)
    
152. Gagneux, P., Moore, J. J. & Varki, A. The ethics of research on great apes. _Nature_ **437**, 27–29 (2005)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20ethics%20of%20research%20on%20great%20apes&journal=Nature&volume=437&pages=27-29&publication_year=2005&author=Gagneux%2CP&author=Moore%2CJJ&author=Varki%2CA)
    
153. Osoegawa, K. et al. An improved approach for construction of bacterial artificial chromosome libraries. _Genomics_ **52**, 1–8 (1998)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=An%20improved%20approach%20for%20construction%20of%20bacterial%20artificial%20chromosome%20libraries&journal=Genomics&volume=52&pages=1-8&publication_year=1998&author=Osoegawa%2CK)
    
154. Schwartz, S. et al. Human-mouse alignments with BLASTZ. _Genome Res._ **13**, 103–107 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC430961) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Human-mouse%20alignments%20with%20BLASTZ&journal=Genome%20Res.&volume=13&pages=103-107&publication_year=2003&author=Schwartz%2CS)
    
155. Kent, W. J. BLAT—the BLAST-like alignment tool. _Genome Res._ **12**, 656–664 (2002)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC187518) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=BLAT%E2%80%94the%20BLAST-like%20alignment%20tool&journal=Genome%20Res.&volume=12&pages=656-664&publication_year=2002&author=Kent%2CWJ)
    
156. Kent, W. J., Baertsch, R., Hinrichs, A., Miller, W. & Haussler, D. Evolution's cauldron: duplication, deletion, and rearrangement in the mouse and human genomes. _Proc. Natl Acad. Sci. USA_ **100**, 11484–11489 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC208784) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Evolution%27s%20cauldron%3A%20duplication%2C%20deletion%2C%20and%20rearrangement%20in%20the%20mouse%20and%20human%20genomes&journal=Proc.%20Natl%20Acad.%20Sci.%20USA&volume=100&pages=11484-11489&publication_year=2003&author=Kent%2CWJ&author=Baertsch%2CR&author=Hinrichs%2CA&author=Miller%2CW&author=Haussler%2CD)
    
157. Pruitt, K. D., Tatusova, T. & Maglott, D. R. NCBI Reference Sequence project: update and current status. _Nucleic Acids Res._ **31**, 34–37 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC165558) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=NCBI%20Reference%20Sequence%20project%3A%20update%20and%20current%20status&journal=Nucleic%20Acids%20Res.&volume=31&pages=34-37&publication_year=2003&author=Pruitt%2CKD&author=Tatusova%2CT&author=Maglott%2CDR)
    
158. Higgins, D. G., Thompson, J. D. & Gibson, T. J. Using CLUSTAL for multiple sequence alignments. _Methods Enzymol._ **266**, 383–402 (1996)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Using%20CLUSTAL%20for%20multiple%20sequence%20alignments&journal=Methods%20Enzymol.&volume=266&pages=383-402&publication_year=1996&author=Higgins%2CDG&author=Thompson%2CJD&author=Gibson%2CTJ)
    
159. Meloni, A. et al. Delineation of the molecular defects in the AIRE gene in autoimmune polyendocrinopathy-candidiasis-ectodermal dystrophy patients from Southern Italy. _J. Clin. Endocrinol. Metab._ **87**, 841–846 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Delineation%20of%20the%20molecular%20defects%20in%20the%20AIRE%20gene%20in%20autoimmune%20polyendocrinopathy-candidiasis-ectodermal%20dystrophy%20patients%20from%20Southern%20Italy&journal=J.%20Clin.%20Endocrinol.%20Metab.&volume=87&pages=841-846&publication_year=2002&author=Meloni%2CA)
    
160. Beales, P. L. et al. Genetic and mutational analyses of a large multiethnic Bardet-Biedl cohort reveal a minor involvement of _BBS6_ and delineate the critical intervals of other loci. _Am. J. Hum. Genet._ **68**, 606–616 (2001)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1274474) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Genetic%20and%20mutational%20analyses%20of%20a%20large%20multiethnic%20Bardet-Biedl%20cohort%20reveal%20a%20minor%20involvement%20of%20BBS6%20and%20delineate%20the%20critical%20intervals%20of%20other%20loci&journal=Am.%20J.%20Hum.%20Genet.&volume=68&pages=606-616&publication_year=2001&author=Beales%2CPL)
    
161. Cunningham, J. M. et al. The frequency of hereditary defective mismatch repair in a prospective series of unselected colorectal carcinomas. _Am. J. Hum. Genet._ **69**, 780–790 (2001)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1226064) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20frequency%20of%20hereditary%20defective%20mismatch%20repair%20in%20a%20prospective%20series%20of%20unselected%20colorectal%20carcinomas&journal=Am.%20J.%20Hum.%20Genet.&volume=69&pages=780-790&publication_year=2001&author=Cunningham%2CJM)
    
162. Mukhopadhyay, A. et al. Mutations in MYOC gene of Indian primary open angle glaucoma patients. _Mol. Vis._ **8**, 442–448 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Mutations%20in%20MYOC%20gene%20of%20Indian%20primary%20open%20angle%20glaucoma%20patients&journal=Mol.%20Vis.&volume=8&pages=442-448&publication_year=2002&author=Mukhopadhyay%2CA)
    
163. Tuchman, M., Jaleel, N., Morizono, H., Sheehy, L. & Lynch, M. G. Mutations and polymorphisms in the human ornithine transcarbamylase gene. _Hum. Mutat._ **19**, 93–107 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Mutations%20and%20polymorphisms%20in%20the%20human%20ornithine%20transcarbamylase%20gene&journal=Hum.%20Mutat.&volume=19&pages=93-107&publication_year=2002&author=Tuchman%2CM&author=Jaleel%2CN&author=Morizono%2CH&author=Sheehy%2CL&author=Lynch%2CMG)
    
164. Clee, S. M. et al. Common genetic variation in _ABCA1_ is associated with altered lipoprotein levels and a modified risk for coronary artery disease. _Circulation_ **103**, 1198–1205 (2001)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Common%20genetic%20variation%20in%20ABCA1%20is%20associated%20with%20altered%20lipoprotein%20levels%20and%20a%20modified%20risk%20for%20coronary%20artery%20disease&journal=Circulation&volume=103&pages=1198-1205&publication_year=2001&author=Clee%2CSM)
    
165. Fullerton, S. M. et al. Apolipoprotein E variation at the sequence haplotype level: implications for the origin and maintenance of a major human polymorphism. _Am. J. Hum. Genet._ **67**, 881–900 (2000)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC1287893) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Apolipoprotein%20E%20variation%20at%20the%20sequence%20haplotype%20level%3A%20implications%20for%20the%20origin%20and%20maintenance%20of%20a%20major%20human%20polymorphism&journal=Am.%20J.%20Hum.%20Genet.&volume=67&pages=881-900&publication_year=2000&author=Fullerton%2CSM)
    
166. Mentuccia, D. et al. Association between a novel variant of the human type 2 deiodinase gene Thr92Ala and insulin resistance: evidence of interaction with the Trp64Arg variant of the β-3-adrenergic receptor. _Diabetes_ **51**, 880–883 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Association%20between%20a%20novel%20variant%20of%20the%20human%20type%202%20deiodinase%20gene%20Thr92Ala%20and%20insulin%20resistance%3A%20evidence%20of%20interaction%20with%20the%20Trp64Arg%20variant%20of%20the%20%CE%B2-3-adrenergic%20receptor&journal=Diabetes&volume=51&pages=880-883&publication_year=2002&author=Mentuccia%2CD)
    
167. Pizzuti, A. et al. A polymorphism (K121Q) of the human glycoprotein PC-1 gene coding region is strongly associated with insulin resistance. _Diabetes_ **48**, 1881–1884 (1999)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20polymorphism%20%28K121Q%29%20of%20the%20human%20glycoprotein%20PC-1%20gene%20coding%20region%20is%20strongly%20associated%20with%20insulin%20resistance&journal=Diabetes&volume=48&pages=1881-1884&publication_year=1999&author=Pizzuti%2CA)
    
168. Katoh, T. et al. Human glutathione S-transferase P1 polymorphism and susceptibility to smoking related epithelial cancer; oral, lung, gastric, colorectal and urothelial cancer. _Pharmacogenetics_ **9**, 165–169 (1999)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Human%20glutathione%20S-transferase%20P1%20polymorphism%20and%20susceptibility%20to%20smoking%20related%20epithelial%20cancer%3B%20oral%2C%20lung%2C%20gastric%2C%20colorectal%20and%20urothelial%20cancer&journal=Pharmacogenetics&volume=9&pages=165-169&publication_year=1999&author=Katoh%2CT)
    
169. Marchesani, M. et al. New paraoxonase 1 polymorphism I102V and the risk of prostate cancer in Finnish men. _J. Natl Cancer Inst._ **95**, 812–818 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=New%20paraoxonase%201%20polymorphism%20I102V%20and%20the%20risk%20of%20prostate%20cancer%20in%20Finnish%20men&journal=J.%20Natl%20Cancer%20Inst.&volume=95&pages=812-818&publication_year=2003&author=Marchesani%2CM)
    
170. Humbert, R. et al. The molecular basis of the human serum paraoxonase activity polymorphism. _Nature Genet._ **3**, 73–76 (1993)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=The%20molecular%20basis%20of%20the%20human%20serum%20paraoxonase%20activity%20polymorphism&journal=Nature%20Genet.&volume=3&pages=73-76&publication_year=1993&author=Humbert%2CR)
    
171. Barroso, I. et al. Candidate gene association study in type 2 diabetes indicates a role for genes involved in β-cell function as well as insulin action. _PLoS Biol._ **1**, E20 (2003)
    
    [PubMed Central](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC212698) [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Candidate%20gene%20association%20study%20in%20type%202%20diabetes%20indicates%20a%20role%20for%20genes%20involved%20in%20%CE%B2-cell%20function%20as%20well%20as%20insulin%20action&journal=PLoS%20Biol.&volume=1&publication_year=2003&author=Barroso%2CI)
    
172. Herrmann, S. M. et al. Uncoupling protein 1 and 3 polymorphisms are associated with waist-to-hip ratio. _J. Mol. Med._ **81**, 327–332 (2003)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=Uncoupling%20protein%201%20and%203%20polymorphisms%20are%20associated%20with%20waist-to-hip%20ratio&journal=J.%20Mol.%20Med.&volume=81&pages=327-332&publication_year=2003&author=Herrmann%2CSM)
    
173. Kong, A. et al. A high-resolution recombination map of the human genome. _Nature Genet._ **31**, 241–247 (2002)
    
    [Google Scholar](http://scholar.google.com/scholar_lookup?&title=A%20high-resolution%20recombination%20map%20of%20the%20human%20genome&journal=Nature%20Genet.&volume=31&pages=241-247&publication_year=2002&author=Kong%2CA)
    

[Download references](https://citation-needed.springer.com/v2/references/10.1038/nature04072?format=refman&flavour=references)

## Acknowledgements

Generation of the _Pan troglodytes_ sequence at Washington University School of Medicine's Genome Sequencing Center and the Broad Institute of MIT and Harvard was supported by grants from the National Human Genome Research Institute (NHGRI). We would like to thank the entire staff of both of those institutions. For work from other groups, we acknowledge the support of the European Molecular Biology Laboratory, Ministerio de Educacion y Ciencia (Spain), Howard Hughes Medical Institute, NHGRI, National Institutes of Health and National Science Foundation. Resources for exploring the sequence and annotation data are available on browser displays available at UCSC ([http://genome.ucsc.edu](http://genome.ucsc.edu/)), Ensembl ([http://www.ensembl.org](http://www.ensembl.org/)) and the NCBI ([http://www.ncbi.nlm.nih.gov](http://www.ncbi.nlm.nih.gov/)). We thank L. Gaffney for graphical help. Author Contributions The last three authors co-directed the work.

## Author information

### Consortia

### The Chimpanzee Sequencing and Analysis Consortium

- Robert H. Waterson
- , Eric S. Lander
- & Richard K. Wilson

## Ethics declarations

### Competing interests

This _Pan troglodytes_ whole-genome shotgun project has been deposited at DDBJ/EMBL/GenBank under the project accessions ARACHNE, AADA01000000 and PCAP, AACZ01000000. Reprints and permissions information is available at [npg.nature.com/reprintsandpermissions](http://www.npg.nature.com/reprintsandpermissions). The authors declare no competing financial interests.

## Additional information

Lists of participants and affiliations appear at the end of the paper

## Supplementary information

### [Supplementary Figures](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM1_ESM.ppt)

Supplementary Figures S1-S12 and accompanying legends. (PPT 1122 kb)

### [Supplementary Notes S1](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM2_ESM.doc)

Genome Sequencing and Assembly. Detailed description of chimpanzee DNA and cell-line resources; genome sequencing and assembly methods; assembly quality control; additional discussion. Supplementary Tables S1-S17. (DOC 407 kb)

### [Supplementary Notes S2](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM3_ESM.doc)

Genome Evolution. Additional methods and discussion related to nucleotide substitution rates, insertions/deletions, transposable elements and large-scale rearrangements. Supplementary Tables S18, S20-S22. (DOC 66 kb)

### [SupplementaryTable S19](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM4_ESM.xls)

Human- and chimpanzee-specific retrotransposed pseudogenes (XLS 83 kb)

### [Supplementary Notes S3](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM5_ESM.doc)

Gene Evolution. Additional methods and discussion related to evolutionary rates for protein coding genes, selective constraints, relative rate tests and genetic changes with potential phenotypic effects. Supplementary Tables S25, S27, S29, S31-S42, S44. (DOC 346 kb)

### [Supplementary Table S23](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM6_ESM.xls)

Rate estimates and additional information for each human-chimpanzee orthologue pair examined. (XLS 3488 kb)

### [Supplementary Table S24](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM7_ESM.xls)

Rate estimates and additional information for each human-chimpanzee-mouse-rat orthologue quadruplet examined. (XLS 3809 kb)

### [Supplementary Table S26](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM8_ESM.xls)

Absolute rate acceleration test statistics for each GO category. (XLS 1229 kb)

### [SupplementaryTable S28](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM9_ESM.xls)

Absolute rate acceleration test statistics (non-parametric) for each GO category. (XLS 806 kb)

### [Supplementary Table S30](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM10_ESM.xls)

Relative rate acceleration test statistics for each GO category. (XLS 368 kb)

### [Supplementary Table S43](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM11_ESM.xls)

Putative human disease alleles present in chimpanzee, and status of support in the literature. (XLS 28 kb)

### [Supplementary Notes S4](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM12_ESM.doc)

Human Population Genetics. Additional methods and discussion related to assignment of ancestral alleles, and detection of selective sweeps in recent human evolution. (DOC 64 kb)

### [Supplementary Notes S5](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM13_ESM.doc)

Additional References. References cited in the Supplementary Notes. (DOC 30 kb)

### [Corrigendum](https://static-content.springer.com/esm/art%3A10.1038%2Fnature04072/MediaObjects/41586_2005_BFnature04072_MOESM14_ESM.doc)

This file contains details regarding an error in Supplementary Table 24 at the time of publication. (DOC 19 kb)

## Rights and permissions

[Reprints and Permissions](https://s100.copyright.com/AppDispatchServlet?title=Initial%20sequence%20of%20the%20chimpanzee%20genome%20and%20comparison%20with%20the%20human%20genome&author=Robert%20H.%20Waterson%20et%20al&contentID=10.1038%2Fnature04072&copyright=Springer%20Nature%20Limited&publication=0028-0836&publicationDate=2005-09-01&publisherName=SpringerNature&orderBeanReset=true)

## About this article

### Cite this article

The Chimpanzee Sequencing and Analysis Consortium. Initial sequence of the chimpanzee genome and comparison with the human genome. _Nature_ **437**, 69–87 (2005). https://doi.org/10.1038/nature04072

[Download citation](https://citation-needed.springer.com/v2/references/10.1038/nature04072?format=refman&flavour=citation)

- Received21 March 2005
- Accepted20 July 2005
- Issue Date01 September 2005
- DOIhttps://doi.org/10.1038/nature04072

### Share this article

Anyone you share the following link with will be able to read this content:

Provided by the Springer Nature SharedIt content-sharing initiative

## This article is cited by

- ### [Emergence and influence of sequence bias in evolutionarily malleable, mammalian tandem arrays](https://doi.org/10.1186/s12915-023-01673-4)
    
    - Margarita V. Brovkina
    - Margaret A. Chapman
    - E. Josephine Clowney
    
    _BMC Biology_ (2023)
    
- ### [Evolutionary relevance of single nucleotide variants within the forebrain exclusive human accelerated enhancer regions](https://doi.org/10.1186/s12860-023-00474-5)
    
    - Hizran Khatoon
    - Rabail Zehra Raza
    - Amir Ali Abbasi
    
    _BMC Molecular and Cell Biology_ (2023)
    
- ### [Epigenetic regulation of human-specific gene expression in the prefrontal cortex](https://doi.org/10.1186/s12915-023-01612-3)
    
    - Weifen Sun
    - Gangcai Xie
    - Xiling Liu
    
    _BMC Biology_ (2023)
    
- ### [Fast-evolving genomic regions underlie human brain development](https://doi.org/10.1038/d41586-023-00069-2)
    
    - Eucharist Kun
    - Vagheesh M. Narasimhan
    
    _Nature_ (2023)
    
- ### [Human-specific genetics: new tools to explore the molecular and cellular basis of human evolution](https://doi.org/10.1038/s41576-022-00568-4)
    
    - Alex A. Pollen
    - Umut Kilik
    - J. Gray Camp
    
    _Nature Reviews Genetics_ (2023)
    

## Comments

By submitting a comment you agree to abide by our [Terms](https://www.nature.com/info/tandc.html) and [Community Guidelines](https://www.nature.com/info/community-guidelines.html). If you find something abusive or that does not comply with our terms or guidelines please flag it as inappropriate.