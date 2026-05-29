# 🧬 HSP70 Sequence Analysis, Phylogenetics, and Primer Design

## 📌 Project Overview
This project focuses on the bioinformatic analysis of the **Heat Shock Protein 70 (HSP70)** gene, a highly conserved molecular chaperone vital for cellular stress response. The workflow includes sequence retrieval, similarity searching via BLAST, Multiple Sequence Alignment (MSA), phylogenetic reconstruction, and functional primer design for downstream PCR applications.

---

## 🔬 Bioinformatics Workflow & Methodology

### 1. NCBI BLASTn Sequence Similarity Search
To validate the evolutionary conservation of the human **HSPA1A** gene, a nucleotide BLAST (BLASTn) was performed against the non-redundant database. 

![NCBI BLASTn Results](<img width="1128" height="612" alt="blast_results" src="https://github.com/user-attachments/assets/d97c2567-9225-497a-822d-7bf56e774997" />
)

**Key Observations:**
- **Query Coverage:** The alignment showed a **100% Query Coverage** with top mammalian hits, ensuring that the full-length mRNA sequence was successfully aligned.
- **Statistical Significance:** The **E-value was 0.0**, which mathematically proves that the sequence similarity found is highly significant and not by random chance.
- **Percent Identity:** The top hit confirmed 100% identity with *Homo sapiens* heat shock protein family A member 1A (HSPA1A), validating the absolute accuracy of our query sequence.

### 2. Multiple Sequence Alignment (Clustal Omega)
To evaluate the evolutionary conservation of the **HSPA1A** gene, a Multiple Sequence Alignment (MSA) was conducted using Clustal Omega with mRNA sequences from *Homo sapiens*, *Mus musculus*, and *Sus scrofa*.

![Clustal Omega Alignment](<img width="607" height="547" alt="alignment_results" src="https://github.com/user-attachments/assets/d959f0a1-f42e-42c6-9703-7f46882827d3" />
)

**Key Observations from Alignment:**
- **Highly Conserved Functional Domains:** As shown in image_d86456.png, massive blocks of identical nucleotides are marked with asterisks (`*`), demonstrating strong evolutionary pressure to maintain the integrity of the HSP70 chaperone protein across mammalian species.
- **5' Untranslated Region (UTR) Divergence:** The alignment clearly reveals that the sequence divergence is significantly higher at the beginning of the sequences (the 5' region), while the coding regions show almost near-perfect sequence identity.

### 3. Phylogenetic Analysis
An unrooted phylogenetic tree was reconstructed based on the Clustal Omega alignment scores to visualize the evolutionary relationships among the selected mammalian HSPA1A sequences.

![Phylogenetic Tree](![phylogenetic_tree](https://github.com/user-attachments/assets/105536f1-e1ed-431d-891b-631d5bb62f4c)
)

**Key Insights from the Tree:**
- **Clonality & Common Ancestry:** As displayed in image.svg, the tree radiates from a tight central node, illustrating that the HSPA1A gene in *Homo sapiens*, *Mus musculus*, and *Sus scrofa* shares a highly recent common mammalian ancestor.
- **Sequence Homology:** The relatively equal branch lengths suggest a steady and conserved rate of evolutionary divergence, further validating the critical cellular role of the HSP70 chaperone which resists high mutation rates.

### 4. PCR Primer Design (Primer-BLAST)
To enable wet-lab validation and expression analysis of the human **HSPA1A** gene, locus-specific primers were designed using NCBI Primer-BLAST targeting the RefSeq template `NM_005345.6`.

![Primer Design Graphical View](![phylogenetic_tree](https://github.com/user-attachments/assets/e2e18555-e52c-4c56-a901-1bc1e075647a)
)

**Key Design Insights:**
- **Exon-Specific Targeting:** As shown in image_d7f7d6.png, 10 high-quality primer pairs were generated. **Primer 1** was selected as the optimal candidate due to its ideal thermodynamic properties and target specificity within the exon region.
- **Amplicon Amplification:** The primer pairs span across the 3' region (between 1,950 bp and 2,150 bp), which is highly specific for evaluating transcript abundance via qPCR without cross-reacting with other HSP70 pseudogenes.

#### Selected Primer Pair (Primer 1 Details):
| Primer Type | Sequence (5' -> 3') | Length (bp) | $T_m$ (°C) | GC (%) | Product Size |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Forward** | `5'- AGCTGGAGCAGGTGTGTAAC -3'` | 20 | 59.96 | 55.00 | **154 bp** |
| **Reverse** | `5'- CAGCAATCTTGGAAAGGCCC -3'` | 20 | 59.47 | 55.00 | (Ideal for qPCR) |

---

## 📊 Results & Visualizations

### 1. Multiple Sequence Alignment (MSA)
*(Insert a screenshot of your Clustal Omega alignment showing conserved stars `*` here)*
`![Clustal Alignment](path/to/alignment_screenshot.png)`

### 2. Phylogenetic Tree
*(Insert a screenshot of your evolutionary tree here)*
`![Phylogenetic Tree](path/to/tree_screenshot.png)`

### 3. Designed Primers Table
| Primer Type | Sequence (5' -> 3') | Length (bp) | $T_m$ (°C) | GC (%) | Product Size |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Forward** | `5'- TGTCGND... -3'` | 20 | 58.5 | 50.0 | **210 bp** |
| **Reverse** | `5'- AGTCGND... -3'` | 20 | 59.0 | 55.0 | |

---

## 🏁 Conclusion
The computational analysis successfully confirmed the strict evolutionary conservation of the HSP70 chaperone system across biology. Furthermore, the designed primers passed all strict bioinformatic filters (avoiding self-dimers and cross-reactivity), making them viable candidates for in vitro molecular biological verification.

---

## 🛠️ Tools & Technologies
- **Databases:** NCBI (GenBank, BLAST)
- **Alignment & Phylogeny:** Clustal Omega, MEGA11
- **Primer Design:** Primer-BLAST
- **Version Control:** Git & GitHub
