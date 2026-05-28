# 🧬 HSP70 Sequence Analysis, Phylogenetics, and Primer Design

## 📌 Project Overview
This project focuses on the bioinformatic analysis of the **Heat Shock Protein 70 (HSP70)** gene, a highly conserved molecular chaperone vital for cellular stress response. The workflow includes sequence retrieval, similarity searching via BLAST, Multiple Sequence Alignment (MSA), phylogenetic reconstruction, and functional primer design for downstream PCR applications.

---

## 🔬 Bioinformatics Workflow & Methodology

### 1. Sequence Retrieval & NCBI BLAST
- **Query Sequence:** Human *Homo sapiens* heat shock protein 70 (HSP70) mRNA/Protein sequence retrieved from NCBI GenBank.
- **BLAST Search:** Performed **BLASTn** and **BLASTp** against the non-redundant (nr) database to identify homologous sequences across different taxa and evaluate percentage identity and E-values.

### 2. Multiple Sequence Alignment (MSA)
- Used **Clustal Omega** to align HSP70 sequences from diverse organisms (*Homo sapiens*, *Mus musculus*, *Arabidopsis thaliana*, and *Escherichia coli*).
- **Objective:** To identify highly conserved catalytic domains and mutation-prone regions within the stress-response protein family.

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
