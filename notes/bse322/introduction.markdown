---
layout: note
---

> This lecture briefly introduces bioinformatics and computational biology, and motivates the reader about the why, the how, and the what. A few example cases for maotivation are also mentioned.

**Bioinformatics:**
Bioinformatics is an interdisciplinary field mainly involving molecular biology and genetics, computer science, mathematics, and statistics. Data intensive, large-scale biological problems are addressed from a computational point of view. <cite>From Wikipedia</cite>

**Computational Biology:**
Computational Biology, which includes many aspects of bioinformatics, is the science of using biological data to develop algorithms or models to understand biological systems and relationships.
<cite>From Wikipedia</cite>


### Introduction
**Motivation:**
In 2013, Angelina Jolie underwent preventive **mastectomy** to lower the risk of breast cancer. She had a mutation in her DNA that gave her **87%** chance of developing breast cancer.

**The challenge:** 
**Finding mutations** that lead to various diseases is one of the important challenges for bioinformatics. But with the increasing genome sizes *(refer below)*, to do this task effectively we need better approaches and better algorithms. Hopefully, by the end of these notes, you'd have explored a few of the tools that are used, and know how you can use them as well.

<div class="imgcap">
    <img src="/assets/images/dna_sizes.jpg">
    <div class="thecap">
        <p>Genome sizes. Image credit: <a href="https://idp.nature.com/transit?redirect_uri=https%3A%2F%2Fwww.nature.com%2Fscitable%2Fknowledge%2Flibrary%2Fcomparative-genomics-13239404&code=808ce6bc-0e34-4f60-957d-aa9c852c4302">nature</a> <br>Wheat plant genome size: 17 billion (more than 90,000 genes)</p>
    </div>
</div>

> The first complete non-viral genome to be sequenced was a bacterium, Haemophilus influenzae, sequenced in 1995.

> The human genome was published in 2001. The first protein was sequenced in 1953.

### The increase in data
After the first sequencing of protein and the human genome, numerous sequences have been sequenced. In fact, the growth has been almost exponential. Biological data also comes from Genomic sequences, Single Nucleotide Polymorphisms (SNPs, Protein amino acid sequences, Protein 3D structures, Gene Expression, Protein function, and Literature. **With such a large database to deal with, we need efficient methods to process, interpret and study them.**

<div class="imgcap">
    <img src="/assets/images/pdb_growth.png">
    <div class="thecap">
        <p>Yearly growth of protein structures in PDB. Image credit: <a href="https://www.researchgate.net/figure/Yearly-growth-of-total-structure-in-PDB_fig10_282790336">ResearchGate</a>
        <br>It now has more than 100,000 structures</p>
    </div>
</div>

```python
>gi|388480089|ref|YP_492284.1| transporter [Escherichia coli]
 MSGLKQELGLAQGIGLLSTSLLGTGVFAVPALAALVAGNNSLWAWPVLIILVFPIAIVFAILGRHYPSAG
GVAHFVGMAFGSRLERVTGWLFLSVIPVGLPAALQIAAGFGQAMFGWHSWQLLLAELGTLALVWYIGTRG 
ASSSANLQTVIAGLIVALIVAIWWAGDIKPANIPFPAPGNIELTGLFAALSVMFWCFVGLEAFAHLASEF 
KNPERDFPRALMIGLLLAGLVYWGCTVVVLHFDAYGEKMAAAASLPKIVVQLFGVGALWIACVIGYLACF 
ASLNIYIQSFARLVWSQAQHNPDHYLARLSSRHIPNNALNAVLGCCVVSTLVIHALEINLDALIIYANGI 
FIMIYLLCMLAGCKLLQGRYRLLAVVGGLLCVLLLAMVGWKSLYALIMLAGLWLLLPKRKTPENGITT
```

<div class="imgcap">
    <div class="thecap">
        Example of a protein sequence in FASTA format
    </div>
</div>

> Myoglobin and Hemoglobin: first protein structures to be determined.

**A few terms:** *(not exhaustive, not too formal either)*  
**Genome:** the totality of DNA sequence of an organism  
**Transcriptome:** the mRNA complement of an entire organism, tissue type, or cell 
**Proteome:** the totality of protein sequences  
**Metabolome:** the totality of metabolites in an organism  
**Lipidome:** the totality of lipids  
**Interactome:** the totality of the molecular interactions in an organism  
**Spliceome:** the totality of the alternative splicing protein isoforms  
**Kinome:** The totality of protein kinases in a cell  
**Foldome:** Foldome is the totality of biological structures as skeletons  
**Reactome:** A knowledge base of biological processes.  
> You can make up your own -omes, like electrome.

In the next set of lectures, we will look at a few concepts of evolution and build up from there!