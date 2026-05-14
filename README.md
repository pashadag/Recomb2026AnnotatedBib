# Annotated bibilography to match the keynote talk at RECOMB 2026

My starting point for discussing ANI estimation is the [Ondov et al. Mash paper](https://doi.org/10.1186/s13059-016-0997-x). This paper presented the Mash estimator for ANI estimation. The estimator uses a Poisson approximation to a binomial; however, it was later observed in [sarm] and later described in our own [paper] that a Poisson approximation can be easily replaced by the exact binomial to obtain a more accurate estimator. This is the estimator I refer to as the Mash estimator in the talk.

We introduced the k-span model in a RECOMB 2021 [paper] and proved a confidence interval for the Mash estimator in this model (among other things). 

I refer in the talk to my [paper] on modeling biological problems in computer science. 
This is a more expository/educational paper about how to take a poorly defined biological problem and formalize it into a model that is well-defined and useful. The k-span model is an example of such a process. 

In a later WABI 2025 [paper], we removed the assumptions regarding no repeats to derive a new repeat-aware estimator.

## References
* Peter Sanders [Algorithm engineering – an attempt at a definition](https://doi.org/10.1007/978-3-642-03456-5_22). Efficient Algorithms, LNCS Volume 5760 (2009).
* Roughgarden, Tim, ed. [Beyond the worst-case analysis of algorithms](https://www.cambridge.org/us/universitypress/subjects/computer-science/algorithmics-complexity-computer-algebra-and-computational-g/beyond-worst-case-analysis-algorithms?format=HB&isbn=9781108494311). Cambridge University Press (2021).
* Roughgarden, Tim [Beyond worst-case analysis](https://doi.org/10.1145/3232535), Communications of the ACM, 62(3):88--96 (2019).
* Chen, Ke*, Li, Xiang*, Shi, Qian, Shao, Mingfu‡, and Medvedev, Paul‡ [Hash functions in nucleotide sequence analysis](https://doi.org/10.1101/gr.281453.125). Genome Research, 36:887–902 (2026).
* Paul Medvedev, [The theoretical analysis of sequencing bioinformatics algorithms and beyond](https://doi.org/10.1145/3571723). Communications of the ACM, 66(7):118-125 (2023).
* Gonzalo Navarro [Compact Data Structures](https://www.cambridge.org/core/books/compact-data-structures/68A5983E6F1176181291E235D0B7EB44), Cambridge University Press (2016)
* Rayan Chikhi, Jan Holub, and Paul Medvedev [Data structures to represent a set of k-long DNA sequences](https://doi.org/10.1145/3445967). ACM Computing Surveys, 54(1), (2021).
* Camille Marchet, Christina Boucher, Simon J Puglisi, Paul Medvedev, Mikaël Salson, Rayan Chikhi [Data structures based on k-mers for querying large collections of sequencing datasets](https://doi.org/10.1101/866756). Genome Research, 31: 1-12 (2021).
* Fatemeh Almodaresi, Hirak Sarkar, Avi Srivastava, and Rob Patro [A space and time-efficient index for the compacted colored de Bruijn graph](https://doi.org/10.1093/bioinformatics/bty292), ISMB (2018).
* Giulio Ermanno Pibiri [Sparse and skew hashing of k-mers](https://doi.org/10.1093/bioinformatics/btac245). ISMB (2022)
* Rob Patro, Geet Duggal, Michael I Love, Rafael A Irizarry, Carl Kingsford [Salmon provides fast and bias-aware quantification of transcript expression](https://doi.org/10.1038/nmeth.4197).  Nature Methods 14:417–419 (2017).
* Paul Medvedev [Theoretical analysis of edit distance algorithms: an applied perspective](https://doi.org/10.1145/3582490). Communications of the ACM, 66(12):64-71 (2023).
* Jim Shaw and Yun William Yu [Proving sequence aligners can guarantee accuracy in almost O(m log n) time through an average-case analysis of the seed-chain-extend heuristic](https://doi.org/10.1101/gr.277637.122). Genome Research 33(7):1175–1187 (2023). 
* Ondov, B.D., Treangen, T.J., Melsted, P. et al. [Mash: fast genome and metagenome distance estimation using MinHash](https://doi.org/10.1186/s13059-016-0997-x). Genome Biol 17, 132 (2016).
* Shahab Sarmashghi, Kristine Bohmann, M Thomas P. Gilbert, Vineet Bafna, Siavash Mirarab [Skmer: assembly-free and alignment-free sample identification using genome skims](https://doi.org/10.1186/s13059-019-1632-4). Genome Biology 20:34 (2019).  
 * Paul Medvedev [Modeling Biological Problems in Computer Science: A Case Study in Genome Assembly](https://arxiv.org/pdf/1706.05429). Briefings in Bioinformatics, 20(4):1376-1383 (2019). [Slides](https://www.dropbox.com/sh/x11d58877w07nlj/AABVNqMLwiVEosZGs089O65Sa?dl=0)
* Antonio Blanca†, Robert S. Harris†, David Koslicki†, Paul Medvedev† [The statistics of k-mers from a sequence undergoing a simple mutation process without spurious matches](https://doi.org/10.1101/2021.01.15.426881). RECOMB (2021). [slides](http://medvedevgroup.com/wp-content/uploads/DSB21-talk.pdf) and [talk](https://www.dropbox.com/s/kshqzwx73xzpnh8/The%20statistics%20of%20k-mers%20from%20a%20sequence%20undergoing%20a%20simple%20mutation%20process%20without%20spurious%20matches%20.mp4?dl=0)
* Haonan Wu, Antonio Blanca‡ and Paul Medvedev‡ [K-mer-based estimators of the substitution rate between repetitive sequences](https://doi.org/10.1101/2025.06.19.660607). WABI (2025).
* Wu, H, and Medvedev, P. [The gift of novelty: repeat-robust k-mer-based estimators of mutation rates](https://www.biorxiv.org/cgi/content/short/2026.04.01.715966). ISMB (2026). 
* Mahmudur Rahman Hera, Paul Medvedev, David Koslicki and Antonio Blanca [Estimation of substitution and indel rates via k-mer statistics](https://doi.org/10.1101/2025.05.14.653858), WABI (2025).
* Mahdi Belbasi†, Antonio Blanca†, Robert S. Harris†, David Koslicki†, and Paul Medvedev† [The minimizer Jaccard estimator is biased and inconsistent](https://doi.org/10.1093/bioinformatics/btac244), ISMB (2022). [talk](https://youtu.be/01U8jX2GTX8) and [slides](http://medvedevgroup.com/wp-content/uploads/minimizer-jaccard-slides-on-website.pdf)


