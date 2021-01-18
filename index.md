## About
I was born in Jaragua do Sul, Santa Catarina, Brazil.
<br>
As a teenager, I played competitive Chess and in my early 20's I was a professional Poker player.
My favorite album is probably [Beacon](https://open.spotify.com/album/3Mdzwty8ag5QyAYLxThypm?si=pMxZbAt7SGejBGPalS8h7g) by Two Door Cinema Club.
<br><br>
I did my Bsc in Biological Sciences, Msc in Genetics and Evolution and PhD in Evolutionary Biology [(CV)]({{ site.baseurl }}/pdf/CVitae.pdf).
In my current postdoc I investigate natural selection in short time-scales. 
I share my hot takes about science and academia on [Twitter](https://twitter.com/gv_barroso).

## Projects

### PhD
In the first chapter of my [PhD thesis][phd], I used regression techniques to analyze the signature of selection in gene expression variation among individual cells. Using single-cell transcriptomics data from _Mus musculus_, [we showed](https://www.genetics.org/content/208/1/173) that expression noise is reduced in genes that are central within molecular networks, consistent with selection acting to avoid noise propagation within the cell.
<br><br>
In the second and third chapters I developed the [integrated Sequentially Markovian Coalescent][ismc] (iSMC) – a population genetic method that uses Hidden Markov Models to jointly infer demography and variation in recombination and mutation rates along the genome. Using [iSMC][ismc], we were able to show that the similarity of the recombination landscape among Hominin populations recapitulates their established [evolutionary history](https://journals.plos.org/plosgenetics/article?id=10.1371/journal.pgen.1008449), as well as to estimate that mutation rate variation is the main driver of the distribution of nucleotide diversity along the _Drosophila melanogaster_ genome (Barroso & Dutheil, _in preparation_). A [thorough review](https://arxiv.org/abs/2010.08359) of Coalescent Hidden Markov Models was written by Julien Dutheil.

Also during my PhD, we wrote a chapter in this open access book: [Statistical Population Genomics](https://link.springer.com/book/10.1007/978-1-0716-0199-0).

### Postdoc

## Developing a statistical method for inferring the mode and strength of selection in a single generation 

The prevalence of purifying selection across the human exome makes inferring its strength a central goal in biology. Equally important is characterizing the degree to which deleterious variants influence fitness in heterozygous sites, referred to as dominance. Together, knowledge of the selection coefficient (s) and the dominance coefficient (h) can inform about functional constraints in protein structure and interaction networks, shedding light into both evolutionary and medical genetics. Several studies have used population genetic data to infer the fitness effects of mutations arising in human genes. However, they assume additivity, independence between sites, and cannot properly account for complex demographic patterns. They also capture long-term signals of selection, effectively averaging s over several thousand generations. This may result in misleading inference since environmental changes modulate the strength of selection over time. In this project I develop a new statistical model (TIDES) to infer the landscape of selective constraints within the last generation. TIDES simultaneously infers s and h in a single generation using approximate Bayesian computation. It leverages phased sequences from family trios to look for signatures of selection in the transmission of single nucleotide polymorphisms from parents to offspring. Briefly, comparing genomes from the offspring (the observed data) with genomes from simulated zygotes that could have been conceived by their parents provides information about the (unobserved) embryos that were miscarried and is therefore indicative of the strength of viability selection during embryonic development. By explicitly simulating meiosis, TIDES fully models linkage disequilibrium. Distinguishing between homozygous and heterozygous genotypes further allows for disentangling between s and h. Moreover, by conditioning on parental genomes, past demography does not bias the inference and our summary statistics are sensitive to the strength of selection acting on the current generation rather than in the deep past. In Figure 1 I show the result of benchmarking TIDES with forward simulations of human-like evolutionary scenarios:

### Figure 1
![]({{ site.baseurl }}/pdf/TIDES_1.pdf)

## Analysing the population genetic consequences of epistasis

TODO

[phd]: https://macau.uni-kiel.de/servlets/MCRFileNodeServlet/dissertation_derivate_00008280/Diss_GVB_Thesis.pdf
[ismc]: https://github.com/gvbarroso/iSMC
[tides]: https://github.com/gvbarroso/ABCDFE

