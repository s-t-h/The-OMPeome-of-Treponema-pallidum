# **The OMPeome of Treponema pallidum**
### Master Thesis Bioinformatics, Eberhard Karls Universität Tübingen
`Author:    Simon Hackl`
`Contact:   simon.hackl@uni-tuebingen.de`
`Period:    August 16, 2021 to February 16, 2022`
---
`This repository serves as cloud storage for supplementary information of the thesis.`

---

### **Abstract**
The worldwide growing number of syphilis cases, a chronic and systemic disease caused by the parasitic prokaryote Treponema pallidum subsp. pallidum (TPA), are of increasing concern. A group of experts, the Treponema OMPeome consortium, has set itself the goal of developing the first globally effective vaccine against syphilis. For its development, a combination of conserved immunogenic epitope regions of TPA outer membrane proteins (OMPs) is considered an effective strategy. Only modern DNA capture and enrichment methods have made it possible to collect hundreds of clinical TPA DNA samples. In terms of vaccine development, the goal is now to obtain an overview of the variability of TPA OMPs (the OMPeome) and to track down conserved epitopes.

To foster this process, the main goal of this thesis was to implement a comprehensive TPA OMPeome analysis pipeline: Using modern in silico methods the prediction of previously unknown protein structures is enabled. The utilization of state-of-the-art variant calling methods and the implementation of a script, `RecoverMI`[^1], allows the elucidation of nucleotide variants with respect to a reference genome even in highly repetitive regions, a problem that arises in particular when considering OMPs. The implemented applications `MUSIAL2.0`[^2] and `MUSIAL2.0ᴵⱽᴱ`[^3] as well as a developed scoring system for secondary structure coupled spatial aminoacid interactions, the PRISMEM matrix, enable the allocation of elucidated variants from a bulk set of samples to protein structures, a novel unique interactive visualization of these allocated variants and the prediction of their effect on the protein structure.

Ultimately, the developed pipeline was applied to a dataset of 74 TPA samples in order to assess the variability of 36 high priority OMP targets using the clinical relevant TPA Nichols strain as a reference. This analysis revealed a set of conserved immunogenic OMPs and that high variability in general is associated with the accumulation of nucleotide variants at OMP epitopes. The utilization and advancement of the developed pipeline will confidently boaster the development of a syphilis vaccine.

---

### **Pipeline Overview**
[Contribution guidelines for this project](resources/PipelineOverview.png)

---

### **Supplement Content**
1. _M1_TPOMPeome_Hackl2022_Benchmark.ipynb_
This Notebook was used to generate benchmark data and run `MUSIAL2.0` on it with a concomitant runtime and maximum resident set size measurment.

2. _M2_TPOMPeome_Hackl2022_PRISMEM15Matrix.ipynb_
This Python Notebook guides through the steps of generating and evaluating the PRISMEM15 matrix. The concept is based on the publication "Amino acid interaction preferences in proteins", Jha et al., 2010, https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2866284/.

3. _M3_TPOMPeome_Hackl2022_ProteinStructureProcessing.ipynb_
This Python Notebook guides through and documents the steps of protein structure preparation.

4. _M4_TPOMPeome_Hackl2022_VariantCalling.ipynb_
This Python Notebook guides through and documents the steps of variant calling.

5. _M5_TPOMPeome_Hackl2022_VariabilityAnalysis.ipynb_
This Python Notebook guides through and documents the steps of variability assessment.


[^1]: [`RecoverMI`](https://github.com/s-t-h/RecoverMI)
[^2]: [`MUSIAL2.0`](https://github.com/Integrative-Transcriptomics/MUSIAL)
[^3]: [`MUSIAL2.0ᴵⱽᴱ`](https://github.com/Integrative-Transcriptomics/MUSIAL-IVE)