---
layout: note
---

In this lecture, we will look at a few evolutionary concepts like species and speciation, and understand why it matters in the light of bioinformatics. Towards the end, we will look at homology, what does paralogs, orthologs mean, look at why 'similarity' matters, and why finding 'similarity' is a difficult problem.

<div class="imgcap">
    <img src="/assets/images/dobzhansky.jpg">
    <div class="thecap">
        <p>"Nothing in biology makes sense except in the light of evolution." - Dobzhansky (1973)</p>
    </div>
</div>

### Species and Speciation, gene duplication
**Species:**
Group of population that 
* have similar appearance, but **appearance alone is not a good indicator of species**
* Successfully interbreed
* Reproductively isolated from other species
* Gene flow occurs between members of the species

**Speciation:**
The formation of two groups of organisms that are reproductively isolated from each other and thus have no gene flow.
**When there is no gene flow, the 2 groups will accumulate more and more differences over time.**

<div class="imgcap">
    <img src="/assets/images/species.jpg">
    <div class="thecap">
        <p>Species and Speciation. Image credit: <a href="https://ib.bioninja.com.au/standard-level/topic-4-ecology/41-species-communities-and/species.html">BioNinja</a></p>
    </div>
</div>

**Gene duplication:**
* A redundant duplicate of a gene may acquire divergent mutations and eventually emerge as a new gene.
* It is one of the ways to increase the amount of genetic material, and create new function.

### Homology
**Orthologs:**
Two genes are orthologous if they diverged after a speciation event.  
**Paralogs:**
Two genes are paralogous if they diverged after a duplication event. 

> Orthologs and paralogs together make homologs.

**Analogous genes:**
Similar regions in sequences may not have a common ancestor but may have arisen independently during evolution (to perform the same function). This is called **convergent evolution**.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Such gene/protein sequences are referred to as analogous *(e.g. chymotrypsin and subtilisin)***

<div class="imgcap">
    <img src="/assets/images/homology.png">
    <div class="thecap">
        <p>Homology. Image credit: <a href="http://steipe.biochemistry.utoronto.ca/abc/index.php/BIO_Assignment_Week_7">UofT</a></p>
    </div>
</div>

<div class="imgcap">
    <img src="/assets/images/homologs.png">
    <div class="thecap">
        <p>Orthologs and paralogs.</p>
    </div>
</div>

### Why similarity matters?
**Case of Cystic Fibrosis:**
Cystic fibrosis (CF) is a chronic and frequently fatal genetic disease of the body's mucus glands (abnormally high level of mucus in glands). CF primarily affects the respiratory systems in children.

Similarity in sequences helped scientists to solve the CF mystery in 1989. 
* In early 1980s biologists hypothesized that CF is a recessive disorder caused by mutations in a gene that remained unknown till 1989
* In 1989, researchers sequenced a stretch of DNA and compared to the database of other known genes, and found similarity with a known gene that functions as ion-transport channel.
* Thus, researchers predicted that the gene responsible for cystic fibrosis may be involved in transport of some ions across the cell.
*(This was later confirmed with detailed experiments)*

**Hence finding similarity in sequences is an IMPORTANT problem.** But it is not an easy problem because -- 
* Sequences can be long and of different lengths.
* Sequences may have mutations making them difficult to compare by exact matching
* Sequences may have insertions or deletions

We need a general solution that handles all these cases and tells us the maximum possible similarity between two sequences.

**In the next set of notes we will look at the general solutions, their pros and cons etc.**
