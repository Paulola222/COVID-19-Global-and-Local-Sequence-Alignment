# Suffix Tree Construction for COVID-19 Strain Comparison

## Overview
This project implements suffix tree construction to enable efficient 
sequence comparison across SARS-CoV-2 genomic strains. Suffix trees allow 
substring and pattern-matching operations across large genomic sequences to 
be performed far more efficiently than naive pairwise comparison, making 
them well suited to genome-scale comparative analysis.

## Method
The suffix tree is constructed to support seed-and-extend alignment: short, 
exact-matching "seed" regions are first identified efficiently via the tree 
structure, then extended to identify longer regions of conservation or 
variation between strains. This approach underlies the comparative genomics 
analysis carried out in the related repository, 
`Genome-scale-comparisons-of-COVID-19-strains`.

## Why This Approach
Standard pairwise sequence alignment scales poorly as the number of strains 
and genome length increase. Suffix tree-based seed-and-extend approaches 
reduce this computational burden while preserving the ability to identify 
both exact and near-exact matches, which is essential when comparing viral 
genomes that differ by only a small number of mutations across otherwise 
highly conserved sequences.

## Context
This project was developed independently, without the infrastructure of a 
funded laboratory or the direction of a supervisor, as part of a broader 
self-directed effort to apply rigorous, efficient computational methods to 
SARS-CoV-2 genomic surveillance.

## Author
Paul Ayodeji Ola
