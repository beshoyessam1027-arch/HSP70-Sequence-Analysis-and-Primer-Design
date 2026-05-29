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

### 1. NCBI BLASTn Sequence Similarity Search
To validate the evolutionary conservation of the human **HSPA1A** gene, a nucleotide BLAST (BLASTn) was performed. 

![NCBI BLASTn Results](<img width="1128" height="612" alt="blast_results" src="https://github.com/user-attachments/assets/5ef70e9c-f9ca-49e0-885d-d79884439ade" />
)

**Key Observations:**
- **Query Coverage:** The alignment showed a **100% Query Coverage** with top mammalian hits, ensuring that the full-length mRNA sequence was successfully aligned.
- **Statistical Significance:** The **E-value was 0.0**, which mathematically proves that the sequence similarity found is highly significant and not by random chance.

---

### 2. Multiple Sequence Alignment (Clustal Omega)
To evaluate the evolutionary conservation at the nucleotide level, a Multiple Sequence Alignment (MSA) was conducted using Clustal Omega with mRNA sequences from *Homo sapiens*, *Mus musculus*, and *Sus scrofa*.

![Clustal Omega Alignment](<img width="607" height="547" alt="alignment_results" src="https://github.com/user-attachments/assets/5ed182e5-1c41-478e-9c55-79958fd35b1c" />
)

**Key Observations from Alignment:**
- **Highly Conserved Functional Domains:** Massive blocks of identical nucleotides are marked with asterisks (`*`), demonstrating strong evolutionary pressure to maintain the integrity of the HSP70 chaperone protein across mammalian species.
- **5' UTR Divergence:** The alignment reveals that sequence divergence is higher at the beginning of the sequences (5' untranslated region), while coding regions show near-perfect identity.

---

### 3. Phylogenetic Analysis
An unrooted phylogenetic tree was reconstructed based on the Clustal Omega alignment scores to visualize the evolutionary relationships.

![Phylogenetic Tree](![phylogenetic_tree](https://github.com/user-attachments/assets/e40e1373-d74a-4949-b154-e6872922e196)
)

**Key Insights from the Tree:**
- **Common Ancestry:** The tree radiates from a tight central node, illustrating that the HSPA1A gene in *Homo sapiens*, *Mus musculus*, and *Sus scrofa* shares a highly recent common mammalian ancestor.
- **Sequence Homology:** The relatively equal branch lengths suggest a steady and conserved rate of evolutionary divergence, resisting high mutation rates due to its vital cellular role.

---

### 4. PCR Primer Design (Primer-BLAST)
To enable wet-lab validation and expression analysis of the human **HSPA1A** gene, locus-specific primers were designed using NCBI Primer-BLAST targeting the RefSeq template `NM_005345.6`.

![Primer Design Graphical View](<img width="1272" height="378" alt="primer_design" src="https://github.com/user-attachments/assets/6252a52b-0033-4b5e-a8e0-4857496f1c29" />
)

#### Selected Primer Pair (Primer 1 Details):
| Primer Type | Sequence (5' -> 3') | Length (bp) | $T_m$ (°C) | GC (%) | Product Size |
| :--- | :--- | :---: | :---: | :---: | :---: |
| **Forward** | `5'- AGCTGGAGCAGGTGTGTAAC -3'` | 20 | 59.96 | 55.00 | **154 bp** |
| **Reverse** | `5'- CAGCAATCTTGGAAAGGCCC -3'` | 20 | 59.47 | 55.00 | (Optimized for qPCR) |

**Key Design Insights:**
- **Thermodynamic Efficiency:** Primer pair 1 was selected over others (like pair 3) because it exhibits an optimal $\Delta T_m$ of only **0.49°C**, ensuring balanced annealing kinetics during PCR cycling.
- **Amplicon Specifications:** The primer pair generates a stable **154 bp product** near the 3' region, making it highly specific for evaluating transcript abundance via qPCR without cross-reacting with pseudogenes.

---

## 🏁 Conclusion
The computational analysis successfully confirmed the strict evolutionary conservation of the **HSP70 (HSPA1A)** chaperone system across biological taxa. Furthermore, the designed primers passed all strict bioinformatic filters—exhibiting optimal $T_m$ balance, safe self-complementarity scores, and total target specificity—making them highly viable candidates for *in vitro* molecular biology verification and expression analysis.

---

## 🛠️ Tools & Technologies
- **Databases:** NCBI (GenBank, BLAST)
- **Alignment & Phylogeny:** Clustal Omega, MEGA11
- **Primer Design:** Primer-BLAST
- **Version Control:** Git & GitHub
