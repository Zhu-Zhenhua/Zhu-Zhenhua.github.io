---
layout: default
---


# LLM-PIM Workshop



## Overview

Large language models (LLMs) have emerged as powerful tools across various application domains, from translation to text generation and code completion. However, the computational demands and memory overhead of training and inference for these LLM models pose significant challenges. Furthermore, in the von Neumann architectures, the separation of memory and computing unit causes the serious “memory wall” problem that brings a huge impediment to improving the performance and energy efficiency of LLMs.

The emerging Processing-In-Memory (PIM) architectures, including in-memory computing and near-memory-computing architectures, provide effective solutions to overcome the memory wall problem. PIM architectures perform the in-situ matrix multiplications in memory or general-purpose computing near memory, eliminating data movements between memory and computing units and fully exploiting the high internal bandwidth. Due to their high energy efficiency, PIM architectures have become the alternative solution for LLM acceleration. 

However, the new computing paradigm and emerging memory technologies bring serious design challenges for PIM. 
-	Firstly, the analog-domain computing of PIM is sensitive to circuit noises and device non-ideal factors. How to guarantee computing accuracy while achieving high performance and energy efficiency should be discussed carefully.
- Secondly, the capacity of SRAM-based PIM is quite limited compared to the huge amount of LLM parameters. PIM-friendly LLM compression is required for deployment. 
- Thirdly, the training and inference of LLM require various data precision and formats. How to enable mixed-precision and high-precision computing in PIM becomes a research hotspot.
- Fourthly, besides memory access and computation, the inter-bank/chip/cube data communications in near-memory-computing architectures also account for negligible runtime overhead. 


In view of the above challenges, this workshop will invite the leading experts from the PIM community to share their wonderful achievements in designing PIM architectures for efficient LLM. We hope LLM-PIM can help researchers to better understand the challenges and potential of using PIM for LLM acceleration and inspire further research directions. LLM-PIM workshop will also summarize the invited talk and other insightful discussions into a survey paper about designing PIM for LLM (submitted to related ACM/IEEE journals, e.g., ACM TODAES, IEEE TCAD, etc.).


## Format and Duration of the Workshop

### 10:30 - 11:30 Workshop Keynote Speech 1: 
**Speaker:** Sharon Hu (University of Notre Dame)  
**Title:** *Enhancing Resilience of In-Memory Computing to Device Variations*

### 11:30 - 12:30 Workshop Keynote Speech 2: 
**Speaker:** Bin Gao (Tsinghua University)  
**Title:** *3D Integrated Computing-In-Memory Chips*

---

### 13:30 - 14:00 Invited Talk 1: 
**Speaker:** Pratyush Dhingra (Washington State University)  
**Title:** *Energy Efficient 3D Heterogeneous Manycore Architecture for Transformer Acceleration*

### 14:00 - 14:30 Invited Talk 2: 
**Speaker:** Xin Si (Southeast University)  
**Title:** *SRAM based Computation in Memory Circuits Design for Edge CNNs and Transformers*

### 15:00 - 15:30 Coffee Break

### 15:30 - 16:00 Invited Talk 3: 
**Speaker:** Sathwika Bavikadi (Rochester Institute of Technology)  
**Title:** *Exploring Flex-Enabled Reconfigurable Processor-in-Memory Architectures for Data Intensive Applications*

### 16:00 - 16:30 Invited Talk 4: 
**Speaker:** Xianzhang Chen (Chongqing University)  
**Title:** *Drainage: A Multi-task Coroutine Management Mechanism for Computational Storage*

### 16:30 - 17:00 Invited Talk 5: 
**Speaker:** Geraldo Oliveira (ETH)  
**Title:** TBD

---

### 17:00 - 17:10 Closing Remarks



## Call for Poster

In recent years, Large Language Models (LLMs) have achieved outstanding performance across various applications, marking the advent of the AI 2.0 era. With the exponential increase in model parameters, the storage and memory access overhead of large models have increased by four to five orders of magnitude compared to traditional deep learning models, resulting in significant "memory-wall" platforms. The emerging Processing-In-Memory (PIM) architectures, including in-memory computing and near-memory-computing architectures, have provided an effective solution to overcome the memory wall problem of von Neumann architectures. The Workshop on Workshop on Large Language Model Acceleration using Processing-In-Memory Architectures (LLM-PIM) will invite the leading experts from the PIM community to share their wonderful achievements in designing PIM architectures for efficient LLM. We hope LLM-PIM can help researchers to better understand the design challenges of PIM-based LLM acceleration and inspire further research directions.

LLM-PIM also aims to attract research work with original contributions that address design challenges in PIM architectures & circuits and promote the performance of LLM computing. The workshop is co-located with ESWEEK 2024 to attract the large ESWEEK audience. Topics of interest include, but are not limited to:
* In-Memory Computing architectures and circuits for LLM
* Near-Memory Computing architectures for LLM
* PIM architectures and LLM models co-optimization
* Instruction Set Architectures (ISA) and compilers for PIM architectures
* PIM architectures design for other generative AI models

LLM-PIM will summarize and result in a survey paper about PIM design tools (submitted to related ACM/IEEE journals, e.g., ACM TODAES, IEEE TCAD, etc.). All posters presented in the workshop can be reported and featured in the survey paper. Presenters of the poster will also be invited as co-authors of the survey paper.

We invite your poster submissions for LLM-PIM. A two-page PDF abstract of the research work should be submitted to Prof. Yu Wang (yu-wang@tsinghua.edu.cn) and Dr. Zhenhua Zhu (zhuzhenhua@mail.tsinghua.edu.cn) via email. Abstracts should be in PDF form in two-column format, up to 2 pages in length with 1-inch margins and 10–11-point font size. Abstracts should list the full names and affiliations of all authors and the contact information of the corresponding author. Abstracts will be reviewed by the Program Committee. Those that are selected for poster presentations will be distributed to workshop participants.


#### Important Dates

Abstract submission deadline: 15 August 2024

Notification date: 1 September 2024

Workshop date: 4 October 2024

#### Workshop Chair & Contact:
Yu Wang (yu-wang@tsinghua.edu.cn), Tsinghua University, CN.
Zhenhua Zhu (zhuzhenhua@mail.tsinghua.edu.cn), Tsinghua University, CN.

## Organizers
Yu Wang (Workshop Chair, yu-wang@tsinghua.edu.cn), professor, IEEE fellow, chair of the Department of Electronic Engineering in Tsinghua University, dean of the Institute for Electronics and Information Technology in Tianjin, and vice dean of the School of Information Science and Technology in Tsinghua University. 
His research interests include the application specific heterogeneous computing, processing-in-memory, intelligent multi-agent system, and power/reliability aware system design methodology. Yu Wang has published more than 90 journals (64 IEEE/ACM journals) and 270 conference papers in the areas of EDA, FPGA, VLSI Design, and Embedded Systems, with the Google Scholar citation over 20,000. He has received four best paper awards and 12 best paper nominations. Yu Wang has been an active volunteer in the design automation, VLSI, and FPGA conferences. He is the co-founder of Deephi Tech (a leading deep learning solution provider), which is acquired by Xilinx (AMD) in 2018. He is also the promoter of Infinigence AI Tech (a leading AI infrastructure solution provider), which achieves industry-leading large language model inference performance on more than 10+ different chips.

Zhenhua Zhu (Workshop Co-Chair, zhuzhenhua@mail.tsinghua.edu.cn). Zhenhua Zhu is a postdoctoral researcher in the Department of Electronic Engineering, Tsinghua University. He received his Ph.D. and B.S. degrees from the Dept. of EE, Tsinghua University, in 2024 and 2018, under the supervision of Prof. Yu Wang. His research interests include computer architecture, Processing-In-Memory, and Near Memory Computing. He has published/accepted 35 academic papers in IEEE TCAD, DAC, ISCA, MICRO, ASPLOS, ICCAD, and DATE, with Google Scholar citations more than 800. He also serves as a reviewer for IEEE TCAD, ACM TODAES, and AICAS.


## Follow-up Plans
We hope to provide a final report/manuscript summarizing the highlights and essential outcomes from LLM-PIM for the community to review and refer to.
