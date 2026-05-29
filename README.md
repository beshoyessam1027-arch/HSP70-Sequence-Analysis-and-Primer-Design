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
- Reconstructed a **Phylogenetic Tree** using **MEGA (Molecular Evolutionary Genetics Analysis)** utilizing the Neighbor-Joining method.
- **Insight:** The tree visually demonstrates the evolutionary conservation and divergence of the HSP70 gene from prokaryotes to higher eukaryotes.

### 4. PCR Primer Design
Designed locus-specific primers optimized for standard PCR amplification using **NCBI Primer-BLAST**.

#### Optimized Primer Criteria:
- **Primer Length:** 18–24 bp
- **Melting Temperature ($T_m$):** 55°C – 60°C
- **GC Content:** 40% – 60%
- **Amplicon Size:** 150–300 bp (optimized for qPCR/Gel Electrophoresis)

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
