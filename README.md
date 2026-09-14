# Annotate-Myiopsitta-monachus-genome
We aim to annotate the Monk Parakeet (Myiopsitta monachus) genome using liftoff to design a CRISPR experiment to knock out a gene.
This species has a sequenced genome that is not annotated. In other words, the FASTA file is available but the GTF file is not.
To do so, we will use a the annotated genome (GTF and FASTA) from a model organism (in this case the Budgerigar, Melopsittacus undulatus, which is the most closely related parrot with an annotated genome).

## Problem and background
This is a project carried out as part of my Master's Degree in Genetics and Genomics, for a class called Advanced Techniques in Genetic Engineering (January 2026). This project entails the start-to-finish design of a CRISPR experiment to knock out a gene, including an NHEJ (non-homologous end joining) and HDR (homology-directed repair) approach. For the NHEJ exoeriment, we needed to design a g1 and g2. For the HDR experiment, we needed to design a gRNA for an area with a cysteine to remove, plus a donor strand to turn the cysteine into a stop codon, and of course design the primers.

The Monk Parakeet is an invasive species in Barcelona, and we sought to create a project to reduce their population humanely by introducing gene-edited individuals into the population that carried a knockout mutation affecting fertility.
![Monk Parakeet](https://en.wikipedia.org/wiki/Monk_parakeet#/media/File:Monk_parakeet_(Myiopsitta_monachus)_Santiago.jpg)

The genome was not annotated, so I had to design a bioinformatics workflow to do that before we could do the other steps to design the CRISPR experiment. We needed a properly working reference genome that included our gene of interest.

## Outcome
With this project, we have created a basic usable reference genome for Myiopsitta monachus.

## Limitations
Since only 91.5% of the Budgerigar genes were successfully mapped to the Monk Parakeet sequence, there will be some genes on the Monk Parakeet FASTA that have not been annotated by the resulting GTF file. Thus, the reference genome we have created is useful for looking at known genes, in limited applications like designing a CRISPR experiment or experiments requiring genomic information about single genes, but may not be useful in genome-wide applications such as single-cell or bulk RNA sequencing, as some genes will not be included.
