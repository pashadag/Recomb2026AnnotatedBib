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
We also wrote a similar [survey](https://doi.org/10.1101/gr.260604.119) more specifically for sets of k-mer sets.

I also refer to work that illustrates practical impact of these data structures. The underlying data structures I refer to are [Rainbowfish](https://doi.org/10.1093/bioinformatics/bty292) and [SShash](https://doi.org/10.1093/bioinformatics/btac245). These were deployed as part of the [Salmon](https://doi.org/10.1038/nmeth.4197) software.

### Theoretical analysis of edit distance algorithms 
I only touched upon this topic. A much more extensive exploration of the topic is in a [survey](https://doi.org/10.1145/3582490) in the Communications of the ACM.
I also referred to this [paper](https://doi.org/10.1101/gr.277637.122)  proving fast run time for the seed-chain-and-exten.

## ANI esimation

### Mash 
My starting point for discussing ANI estimation is the [Mash paper](https://doi.org/10.1186/s13059-016-0997-x). This paper presented the Mash estimator for ANI estimation. The estimator uses a Poisson approximation to a Binomial; however, it was later [observed](https://doi.org/10.1186/s13059-019-1632-4) and later described in our own [paper](https://doi.org/10.1093/bioinformatics/btac244) that a Poisson approximation can be easily replaced by the exact Binomial to obtain a more accurate estimator. This is the estimator I refer to as the Mash* estimator in the talk.

### Formalizing the ANI estimation problem without repeats
I briefly refer to the challenges of taking a poorly defined biological problem and formalizing it into a model that is well-defined and useful. 
I cover this in a lot more detail in a paper [Modeling Biological Problems in Computer Science: A Case Study in Genome Assembly](https://arxiv.org/pdf/1706.05429), with associated [slides](https://www.dropbox.com/sh/x11d58877w07nlj/AABVNqMLwiVEosZGs089O65Sa?dl=0).

### K-span model
We introduced the k-span model in  [RECOMB 2021](https://doi.org/10.1101/2021.01.15.426881) and proved a confidence interval for the Mash estimator in this model. The paper contains many more results that can be derived in this model. There are also [slides](http://medvedevgroup.com/wp-content/uploads/DSB21-talk.pdf) and a [talk](https://www.dropbox.com/s/kshqzwx73xzpnh8/The%20statistics%20of%20k-mers%20from%20a%20sequence%20undergoing%20a%20simple%20mutation%20process%20without%20spurious%20matches%20.mp4?dl=0).

### Repeat-robust estimation
The repeat-robust estimator I presented is fully described in a WABI 2025 [paper]. 

### More to this story
More repeat robust estimators are presented in an [ISMB 2026 paper](https://www.biorxiv.org/cgi/content/short/2026.04.01.715966), with an added focus on how to make use of count information. 
I also mention a [WABI 2025 paper](https://doi.org/10.1101/2025.05.14.653858) on how to handle the presence of insertions and deletions as well as an [ISMB 2022 paper](https://doi.org/10.1093/bioinformatics/btac244) on how the use of minimizer sketching can add substantial bias to ANI estimation. That paper also has an associated [talk](https://youtu.be/01U8jX2GTX8) and [slides](http://medvedevgroup.com/wp-content/uploads/minimizer-jaccard-slides-on-website.pdf).


