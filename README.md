# Annotated bibilography to match the keynote talk at RECOMB 2026

My starting point for discussing ANI estimation is the [Ondov et al. Mash paper](https://doi.org/10.1186/s13059-016-0997-x). This paper presented the Mash estimator for ANI estimation. The estimator uses a Poisson approximation to a binomial; however, it was later observed in [sarm] and later described in our own [paper] that a Poisson approximation can be easily replaced by the exact binomial to obtain a more accurate estimator. This is the estimator I refer to as the Mash estimator in the talk.

We introduced the k-span model in a RECOMB 2021 [paper] and proved a confidence interval for the Mash estimator in this model (among other things). 

I refer in the talk to my [paper] on modeling biological problems in computer science. 
This is a more expository/educational paper about how to take a poorly defined biological problem and formalize it into a model that is well-defined and useful. The k-span model is an example of such a process. 

In a later WABI 2025 [paper], we removed the assumptions regarding no repeats to derive a new repeat-aware estimator.

References
* Ondov, B.D., Treangen, T.J., Melsted, P. et al. [Mash: fast genome and metagenome distance estimation using MinHash](https://doi.org/10.1186/s13059-016-0997-x). Genome Biol 17, 132 (2016). 
* Wu, H, and Medvedev, P. [The gift of novelty: repeat-robust k-mer-based estimators of mutation rates](https://www.biorxiv.org/cgi/content/short/2026.04.01.715966). ISMB (2026). 
* Chen, Ke*, Li, Xiang*, Shi, Qian, Shao, Mingfu‡, and Medvedev, Paul‡. [Hash functions in nucleotide sequence analysis](https://doi.org/10.1101/gr.281453.125). Genome Research, 36:887–902 (2026).

