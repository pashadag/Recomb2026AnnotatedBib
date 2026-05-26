# Annotated bibliography to match my talk at RECOMB 2026
Below, I list the papers that I mention in my talk and explain the context. I link to the appropriate journal cites, but I also have a [Dropbox folder](https://www.dropbox.com/scl/fo/euxtpgg7banb4qfxr9e6c/AITE5-4sMbzOey0DPcp-bDk?rlkey=1384unr4tkhbsjg0r50612fn8&st=vhlhffta&dl=0) with all my papers for public access, in case any of them are behind paywalls.

### Algorithm engineering
I cite a [paper](https://doi.org/10.1007/978-3-642-03456-5_22) by Peter Sanders that goes in great detail on the schematic of algorithm engineering that I showed.

### Beyond worst-case analysis of algorithms
The various types of ways to analyze algorithm performance that I described barely scratch the surface. The [edited collection](https://www.cambridge.org/us/universitypress/subjects/computer-science/algorithmics-complexity-computer-algebra-and-computational-g/beyond-worst-case-analysis-algorithms?format=HB&isbn=9781108494311)  by Tim Roughgarden covers this in much more detail. For a shorter more concise summary, see his [paper](https://doi.org/10.1145/3232535) in the Communications of the ACM.

### Hash functions in nucleotide sequence analysis
I discuss how hash functions are often designed and deployed without any theoretical analysis of their accuracy. This observation comes from research done for a [review paper](https://doi.org/10.1101/gr.281453.125) on the use of hash functions in nucleotide sequence analysis.

### Theoretical analysis of sequencing bioinformatics
The vignettes on compact data structures and short read genome assembly analysis comes from my review paper on [The theoretical analysis of sequencing bioinformatics algorithms and beyond](https://doi.org/10.1145/3571723). This papers goes in much more detail on the vignettes I discussed and also includes a much broader overview, including structural variation and challenges and opportunities in the field.

### Compact data structures for k-mers
Compact data structures in general are covered in an excellent [textbook](https://www.cambridge.org/core/books/compact-data-structures/68A5983E6F1176181291E235D0B7EB44) by Gonzalo Navarro.
For data structures of k-mer sets specifically, I refer to a [survey](https://doi.org/10.1145/3445967) we wrote in ACM Computing Surveys. 
We also wrote a similar [survey](https://doi.org/10.1101/866756) more specifically for sets of k-mer sets.

I also refer to work that illustrates practical impact of these data structures. The underlying data structures I refer to are [Rainbowfish](https://doi.org/10.1093/bioinformatics/bty292) and [SShash](https://doi.org/10.1093/bioinformatics/btac245). These were deployed as part of the [Salmon](https://doi.org/10.1038/nmeth.4197) software.

### Theoretical analysis of edit distance algorithms 
I only touched upon this topic. A much more extensive exploration of the topic is in a [survey](https://doi.org/10.1145/3582490) in the Communications of the ACM.
I also referred to this [paper](https://doi.org/10.1101/gr.277637.122)  proving fast run time for the seed-chain-and-exten.



My starting point for discussing ANI estimation is the [Ondov et al. Mash paper](https://doi.org/10.1186/s13059-016-0997-x). This paper presented the Mash estimator for ANI estimation. The estimator uses a Poisson approximation to a binomial; however, it was later [observed](https://doi.org/10.1186/s13059-019-1632-4) and later described in our own [paper](https://doi.org/10.1093/bioinformatics/btac244) that a Poisson approximation can be easily replaced by the exact binomial to obtain a more accurate estimator. This is the estimator I refer to as the Mash* estimator in the talk.

We introduced the k-span model in  [RECOMB 2021](https://doi.org/10.1101/2021.01.15.426881) and proved a confidence interval for the Mash estimator in this model (among other things). 

I refer in the talk to my [paper] on modeling biological problems in computer science. 
This is a more expository/educational paper about how to take a poorly defined biological problem and formalize it into a model that is well-defined and useful. The k-span model is an example of such a process. 

In a later WABI 2025 [paper], we removed the assumptions regarding no repeats to derive a new repeat-aware estimator.

## References

 * Paul Medvedev [Modeling Biological Problems in Computer Science: A Case Study in Genome Assembly](https://arxiv.org/pdf/1706.05429). Briefings in Bioinformatics, 20(4):1376-1383 (2019). [Slides](https://www.dropbox.com/sh/x11d58877w07nlj/AABVNqMLwiVEosZGs089O65Sa?dl=0)
* Antonio Blanca†, Robert S. Harris†, David Koslicki†, Paul Medvedev† [The statistics of k-mers from a sequence undergoing a simple mutation process without spurious matches](https://doi.org/10.1101/2021.01.15.426881). RECOMB (2021). [slides](http://medvedevgroup.com/wp-content/uploads/DSB21-talk.pdf) and [talk](https://www.dropbox.com/s/kshqzwx73xzpnh8/The%20statistics%20of%20k-mers%20from%20a%20sequence%20undergoing%20a%20simple%20mutation%20process%20without%20spurious%20matches%20.mp4?dl=0)
* Haonan Wu, Antonio Blanca‡ and Paul Medvedev‡ [K-mer-based estimators of the substitution rate between repetitive sequences](https://doi.org/10.1101/2025.06.19.660607). WABI (2025).
* Wu, H, and Medvedev, P. [The gift of novelty: repeat-robust k-mer-based estimators of mutation rates](https://www.biorxiv.org/cgi/content/short/2026.04.01.715966). ISMB (2026). 
* Mahmudur Rahman Hera, Paul Medvedev, David Koslicki and Antonio Blanca [Estimation of substitution and indel rates via k-mer statistics](https://doi.org/10.1101/2025.05.14.653858), WABI (2025).
* Mahdi Belbasi†, Antonio Blanca†, Robert S. Harris†, David Koslicki†, and Paul Medvedev† [The minimizer Jaccard estimator is biased and inconsistent](https://doi.org/10.1093/bioinformatics/btac244), ISMB (2022). [talk](https://youtu.be/01U8jX2GTX8) and [slides](http://medvedevgroup.com/wp-content/uploads/minimizer-jaccard-slides-on-website.pdf)


