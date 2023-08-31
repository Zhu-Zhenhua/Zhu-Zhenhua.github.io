---
layout: default
---


# DOT-PIM Workshop



## Overview

In the era of artificial intelligence and big data, the von Neumann architecture with separated memory and computing is facing a serious "memory wall" problem. The data movements have become the main bottleneck limiting the performance and energy efficiency of hardware platforms. The emerging Processing-In-Memory (PIM) architectures provide an effective solution to overcome the memory wall problem. PIM architectures perform the in-situ matrix-vector multiplications in memory or general-purpose computing near memory, eliminating data movements between memory and computing units. Due to their high energy efficiency, PIM architectures are beneficial for embedded systems and gain increasing attention from academia and industry.

However, the new computing paradigm and emerging memory technologies bring serious design challenges for PIM. 
-	Firstly, the analog-domain computing of PIM is sensitive to circuit noises and device non-ideal factors. Efficient and precise circuit/device models are required.
- Secondly, the large-scale PIM architectures require an unacceptably long time of circuit simulation (e.g., SPICE), making the PIM architecture and chip design inefficient.
- Thirdly, the co-design space of intelligent algorithms and PIM architectures is extremely large. How to enable efficient software-hardware co-exploration becomes a research hotspot.

In view of the above challenges, this workshop will invite the leading experts from the PIM community to share their wonderful achievements in design and optimization tools for PIM. We hope DOT-PIM can help researchers to better understand the design challenges of PIM and inspire further research directions. It will also summarize and result in a survey paper about PIM design tools (submitted to related ACM/IEEE journals, e.g., ACM TODAES, IEEE TCAD, etc.). As a complement to ESWEEK, we believe DOT-PIM will enable a strong synergy between PIM architectures and embedded systems and propose potential ideas to achieve important progress in the future.


## Format and Duration of the Workshop

The workshop is composed of eleven invited talks and a poster session.

> 09:00-09:05 Prof. Yu Wang, Tsinghua University

            Opening
> 
> 09:05-09:45 Prof. Onur Mutlu, ETH & CMU

            Memory-Centric Computing
> 
> 09:45-10:15 Prof. Huaqiang Wu, Tsinghua University

            Full-stack Deployment and Design tools for RRAM-based Compute-in-memory System
> 
> 10:15-10:30 Coffee Break
> 
> 10:30-11:00 Dr. Abbas Rahimi, IBM

            A Neuro-Vector-Symbolic Architecture for Data- and Compute-Efficient Continual Learning, Abstract Reasoning, and Combinatorial Inference
> 
> 11:00-11:30 Prof. Li Jiang, Shanghai Jiao Tong University & Huawei

            Opportunities and Challenges for Process-In-Memory (PIM) Technology in ICT Products
> 
> 11:30-12:00 Prof. Xiaoming Chen, ICT, Chinese Academy of Sciences

            EDA Toolchain for Processing-in-Memory CNN Accelerators
> 
> 12:00-13:30 Lunch & Poster Sharing Sessions
> 
> 13:30-14:10 Prof. Yu (Kevin) Cao, University of Minnesota

            HISIM: Heterogeneous Integration Simulator with 2.5D/3D Interconnect Modeling
> 
> 14:10-14:40 Prof. Fengbin Tu, HKUST

            Digital Computing-In-Memory Architecture and Design Automation
> 
> 14:40-15:10 Prof. Grace Li Zhang, TU Darmstadt

            Robust and Efficient Analog In-Memory-Computing Platforms for Neural Networks
> 
> 15:10-15:25 Coffee Break
> 
> 15:25-15:55 Prof. Yaoyu Tao, Peking University

            Fast and Reconfigurable Sort-In-Memory System Enabled by Memristors
>
> 15:55-16:20 Mr. Yuan-Chun Luo, GIT, advisor: Prof. Shimeng Yu

            Benchmarking Framework for Non-volatile Capacitive Compute-in-Memory
> 
> 16:20-16:45 Mr. Shiyu Li, Duke, advisor: Prof. Yiran Chen

            Towards Efficient Processing in Memory AI Systems with Cross-layer Optimization
> 
> 16:45-16:50 Closing Remark


## Talks
### Keynote Speech 1. Prof. Onur Mutlu, ETH & CMU
#### Title: Memory-Centric Computing

Abstract:

Computing is bottlenecked by data. Large amounts of application data overwhelm storage capability, communication capability, and computation capability of the modern machines we design today. As a result, many key applications' performance, efficiency, and scalability are bottlenecked by data movement. In this lecture, we describe three major shortcomings of modern architectures in terms of 1) dealing with data, 2) taking advantage of the vast amounts of data, and 3) exploiting different semantic properties of application data. We argue that an intelligent architecture should be designed to handle data well. We show that handling data well requires designing architectures based on three key principles: 1) data-centric, 2) data-driven, 3) data-aware. We give several examples for how to exploit each of these principles to design a much more efficient and high-performance computing system. We especially discuss recent research that aims to fundamentally reduce memory latency and energy, and practically enable computation close to data, with at least two promising novels directions: 1) processing using memory, which exploits analog operational properties of memory chips to perform massively-parallel operations in memory, with low-cost changes, 2) processing near memory, which integrates sophisticated additional processing capability in memory controllers, the logic layer of 3D-stacked memory technologies, or memory chips to enable high memory bandwidth and low memory latency to near-memory logic. We show both types of architectures can enable orders of magnitude improvements in performance and energy consumption of many important workloads, such as graph analytics, database systems, machine learning, video processing, climate modeling, genome analysis. We discuss how to enable  adoption of such fundamentally more intelligent architectures, which we believe are key to efficiency, performance, and sustainability. We conclude with some research opportunities in and guiding principles for future computing architecture and system designs.

Bio:

Onur Mutlu is a Professor of Computer Science at ETH Zurich. He is also a faculty member at Carnegie Mellon University, where he previously held the Strecker Early Career Professorship. He is an IEEE and ACM fellow. His current broader research interests are in computer architecture, systems, hardware security, and bioinformatics. He received IEEE High Performance Computer Architecture Test of Time Award, NVMW Persistent Impact Prize, the IEEE Computer Society Edward J. McCluskey Technical Achievement Award, ACM SIGARCH Maurice Wilkes Award. 
His longer CV is at https://people.inf.ethz.ch/omutlu/doc/onur_cv.pdf.

### Keynote Speech 2. Prof. Yu (Kevin) Cao, University of Minnesota
#### Title: HISIM: Heterogeneous Integration Simulator with 2.5D/3D Interconnect Modeling

Abstract:

The scaling trend of in-memory computing (IMC) is still lagging the ever-increasing demand of cognitive algorithms. More disruptive innovations, such as chiplet-based heterogeneous integration, will be critical to scaling up the system and speeding up the computation. We propose HISIM to evaluate the performance of monolithic, 2.5D, and 3D chiplet systems. HISIM integrates the technology roadmap of 2.5D/3D wires, conducts electrical modeling and analysis, and performs cycle-accurate simulations of data movement. We demonstrate HISIM with IMC elements on DNNs, transformers, and graph neural networks, to illustrate tradeoffs in placement/routing, latency and thermal issues.

Bio:

Yu (Kevin) Cao, Professor, IEEE Fellow, University of Minnesota. His research interests include neural-inspired computing, hardware design for on-chip learning, and reliable integration of nanoelectronics. He is a Distinguished Lecturer of the IEEE Circuits and Systems Society, and the Specialty Chief Editor of Frontiers in Electronics.

### Invited Talk 1. Prof. Huaqiang Wu, Tsinghua University
#### Title: Full-stack Deployment and Design tools for RRAM-based Compute-in-memory System

Abstract:

In this talk, full-stack deployment and design tools are introduced for RRAM-based compute-in-memory (CIM) systems, which are helpful for optimizing on-chip inference flow and accelerating the system design. We introduced Software-hardware co-optimization methods into the deployment tools, which can significantly improve the on-chip inference performance, such as accuracy, latency, and so on. Moreover, hierarchical simulation models in the design tools are introduced to accurately evaluate the performance of different system designs. Finally, with the full-stack software tools, we demonstrated versatile neural networks on a CIM system with multiple RRAM chips and designed a NOC-based CIM architecture with 100M RRAM cells.

Bio:

Professor Huaqiang Wu is currently the dean of School of Integrated Circuits of Tsinghua University, and the deputy director of Beijing Innovation Center for Integrated Circuits. He has published more than 200 SCI papers in journals, such as Nature, Nature Electronics, Nature Communications etc., and top international conferences on integrated circuits, such as ISSCC, IEDM, VLSI. He has owned more than 100 authorized invention patents in U.S. and China, incubated 4 high-tech companies, and realized the industrialization of ReRAM technology.

### Invited Talk 2. Dr. Abbas Rahimi, IBM
#### Title: A neuro-vector-symbolic architecture for data- and compute-efficient continual learning, abstract reasoning, and combinatorial inference

Abstract:

Neuro-symbolic AI approaches display both perception and reasoning capabilities, but inherit the limitations of their individual deep learning and symbolic AI components. By combining neural networks and vector-symbolic architecture machinery, we propose the concept of neuro-vector-symbolic architecture (NVSA). NVSA solves few-shot continual learning, visual abstract reasoning, and computationally hard problems such as factorization faster and more accurately than other state-of-the-art methods. We also show how the efficient realization of NVSA can be informed and benefitted by the physical properties of in-memory computing hardware, e.g., O(1) MVM, in-situ progressive crystallization, and intrinsic stochasticity of phase-change memory devices.

Bio:

Abbas Rahimi received the M.S. and Ph.D. degrees from the University of California San Diego in 2015, followed by postdoctoral researches at the University of California Berkeley, and at the ETH Zürich. In 2020, he joined the IBM Research-Zürich laboratory as a Research Staff Member. Dr. Rahimi received the 2015 Outstanding Dissertation Award from EDAA, and the ETHZ Postdoctoral Fellowship in 2017.

### Invited Talk 3. Prof. Li Jiang, Shanghai Jiao Tong University & Huawei
#### Title: Opportunities and Challenges for Process-In-Memory (PIM) Technology in ICT Products

Abstract:

PIM technology, which puts computing elements near memory banks, has been studied in academia for decades, emphasized in deep learning scenarios. Samsung, SK Hynix, and UPMEM also announced some industrial POC products. However, it still has a big gap before the mainstream adoption of PIM. In this talk, we advertise memory I/O-intensive (but not compute-intensive) applications suitable for PIM technology, e.g., big data analytics,  database, storage, and data communication scenarios. We will elaborate on PIM's great potential to improve the effective memory bandwidth, offload poor cache locality operations, and reduce data movement in these general applications. Nevertheless, we will highlight some system and architecture challenges induced by the heterogeneity of computing and memory.

Bio:

Li Jiang, Associate Professor in Dept. CSE of Shanghai Jiao Tong University. He is interested in computer architecture and design automation. He has published nearly 100 papers in international conferences and journals, such as DAC, TCAD, ISCA, MICRO, DATE, TC, TVLSI, etc. He has received two best papers and many best paper nominations in DATE and ICCAD. He has also received early career awards from ACM China, CCF, IEEE TTTC, and CAAI. He is also the Chief Technologist and Scientist of heterogeneous communication processor technology at Huawei.

### Invited Talk 4. Prof. Xiaoming Chen, ICT, Chinese Academy of Sciences
#### Title: EDA Toolchain for Processing-in-Memory CNN Accelerators

Abstract:

Processing-in-memory (PIM) architectures are widely used for CNN acceleration with excellent performance and energy efficiency. However, currently there lacks EDA tools to design PIM-based CNN accelerators. This talk will introduce several EDA tools for PIM architecture design and simulation, including an architecture synthesis framework, a CNN compiler targeted at PIM architectures, and a PIM simulator. The synthesis tool automatically generates PIM architectures under given constraints. The compiler converts an ONNX-described CNN to an instruction stream for a given architecture. The simulator estimates the performance, power dissipation and energy consumption of the instruction stream running on the given architecture.

Bio:

Xiaoming Chen, Associate Professor, Institute of Computing Technology, Chinese Academy of Sciences. His research interests include EDA and computer architecture. He was awarded the Excellent Young Scientists Fund of NSFC in 2021. He received 2015 EDAA Outstanding Dissertation Award and 2018 Alibaba DAMO Academy Young Fellow Award.

### Invited Talk 5. Prof. Fengbin Tu, HKUST
#### Title: Digital Computing-In-Memory Architecture and Design Automation

Abstract:

Digital Computing-In-Memory (CIM) is an emerging architecture that avoids the non-ideal issues of analog CIM. With a good balance of efficiency and accuracy, digital CIM has been applied to many modern AI applications such as Transformers and recommendation models. This talk will first discuss advances in digital CIM architecture, and then introduce AutoDCIM, the first automated DCIM compiler. AutoDCIM can generate digital CIM macros according to user-defined architecture parameters with an optimized layout under the given hardware constraints. With the growing interest in digital CIM, AutoDCIM will play an important role in developing an ecosystem for digital CIM-based AI computing.

Bio:

Fengbin Tu is an Assistant Professor at HKUST. His research interests include AI chip, computer architecture, reconfigurable computing, and computing-in-memory. He designed the AI chip Thinker and won the 2017 ISLPED Design Contest Award. Dr. Tu’s research has been published at top conferences and journals on integrated circuits and computer architecture, including ISSCC, JSSC, DAC, and ISCA.

### Invited Talk 6. Prof. Grace Li Zhang, TU Darmstadt
#### Title: Robust and Efficient Analog In-Memory-Computing Platforms for Neural Networks

Abstract:

Deep neural networks (DNNs) have achieved breakthroughs in various fields in the past years. However, the huge number of multiply-accumulate operations and the corresponding computing demand pose a huge challenge to computer architectures to execute them efficiently. In this presentation, analog In-Memory-Computing platforms based on emerging devices including RRAM (Resistive Random Access Memory) and optical computing components will be discussed. Techniques will be presented to enhance their computational efficiency and robustness.

Bio:

Grace Li Zhang joined TU Darmstadt as an Assistant Professor on Hardware for AI in 2022. Her research focuses on hardware acceleration for AI algorithms and systems, AI computing with emerging devices, and neuromorphic computing. She has served/is serving on the technical committee of several conferences including DAC, ICCAD, ASP-DAC, etc.

### Invited Talk 7. Prof. Yaoyu Tao, Peking University
#### Title: Fast and Reconfigurable Sort-In-Memory System Enabled By Memristors

Abstract:

Sorting is fundamental and ubiquitous in modern computing systems for artificial intelligence, database, or web search. Existing sorting systems utilize Von Neumann architecture and comparison operations, but their performance is limited by data bandwidth between memory and comparison units. Sort-in-memory (SIM) is desired but not yet available due to comparison operations that are nontrivial to be implemented in memory. Here we introduce a fast and reconfigurable memristor-based SIM system using digit read (DR) to eliminate comparison operations and tree node skipping (TNS) on DR tree that supports variable data quantity and data types. We extend TNS with multi-bank, bit-slice, and multi-level strategies for cross-array TNS (CA-TNS) with higher scalability and parallelism. Experimented across five benchmark sorting datasets, our SIM system presents up to 3.32x~7.70x speedup, 6.23x~183.5x energy efficiency and 2.23x~7.43x area reduction compared with existing sorting systems. 
We further adopt such SIM system in two representative real-world applications, shortest path search with Dijkstra's algorithm and neural network with run-time tunable sparsity, demonstrating its capability in solving practical sorting problems and compatibility in integrating with other compute-in-memory (CIM) techniques. The memristor-based SIM approaches push sorting into a new paradigm of sort-in-memory for next-generation sorting system.

Bio:

Yaoyu Tao received the B.S., M.S., and Ph.D. degrees in electrical engineering from Shanghai Jiao Tong University, Stanford University, and University of Michigan Ann Arbor, respectively. He also had industry experience with Qualcomm wireless R&D, Oracle VLSI design group and Texas Instruments Kilby lab. He is currently an assistant professor in the Institute of Artificial Intelligence at Peking University and is also affiliated with the School of Integrated Circuits. His research is in efficient VLSI circuits and systems design for machine learning and communications. Dr. Tao was a recipient of the NSFC Distinguished Young Scholar (Overseas), the Best Paper Award at IEEE Global Communication Conference, the Qualstar Awards at Qualcomm, the Young Fellow at Beijing Academy of Artificial Intelligence.

### Senior Ph.D. Student Talk 1. Mr. Yuan-Chun Luo, GIT.
### Advisor: Prof. Shimeng Yu
#### Title: Benchmarking framework for non-volatile capacitive compute-in-memory

Abstract:

Non-volatile capacitive compute-in-memory (CIM) offers higher energy and area efficiency compared to its resistive counterpart. However, the impact of device-to-device variation and temporal noise on the system-level performance remains unexplored. This presentation will first introduce the device-level innovation using ferroelectric materials and the array-level operating principle. Then, an end-to-end methodology will be presented to incorporate experimentally measured device-to-device variation into the design space exploration, from capacitive weight cell design, CIM array with peripheral circuits, to the inference accuracy of deep neural network (DNN) algorithms. Finally, the capacitive CIM will be benchmarked against the resistive approach, showing 6.95× and 14.1× higher TOPS/W×TOPS/mm2 for ResNet-50 and SwinV2-T respectively. 

Bio:

Yuan-Chun Luo is a fifth-year PhD student in Georgia Tech supervised by Prof. Shimeng Yu. He has received the outstanding PhD dissertation proposal award, best paper award of IEEE transactions on nanotechnology, Taiwanese Government Scholarships to Study Abroad, and Georgia Tech ECE fellowship. He interned at Meta and Qualcomm. He is now a visiting scholar at IMEC. 

### Senior Ph.D. Student Talk 2. Mr. Shiyu Li, Duke.
### Advisor: Prof. Yiran Chen
#### Title: Towards Efficient Processing in Memory AI Systems with Cross-layer Optimization

Abstract:

The applications of state-of-the-art AI algorithms have been extended to many exciting domains, such as natural language processing, recommendation systems, edge sensing, etc. Notably, the processing in memory (PIM) computing paradigm emerges as a highly promising approach for AI system implementation, emphasizing reduced data movement costs and increased computational throughput. The focal point of our discussion revolves around the development of dedicated power-efficient circuits and the consequential advantages of fine-grained architecture-algorithm optimizations in PIM-based AI systems. Our research endeavors culminate in cross-layer design optimization methodologies, comprehensively addressing power and throughput bottlenecks through circuit-architecture-algorithm co-design. Throughout this talk, we will present our latest work across multiple layers of the AI system design, illuminating the path to overcome challenges and unlock the full potential of PIM-based AI systems. 

Bio:

Shiyu Li is a Ph.D. candidate at Duke Center for Computational and Evolutionary Intelligence (CEI) which is jointly directed by Prof. Helen Li and Prof. Yiran Chen. He received B.Eng. in Automation from Tsinghua University, China, in 2019. His research interests include computer architecture, near data processing, and hardware/software co-design for deep learning systems.



## Call for Poster

In recent years, the emerging Processing-In-Memory (PIM) architectures have provided an effective solution to overcome the memory wall problem of von Neumann architectures. PIM architectures perform the in-situ matrix-vector multiplications in memory or general-purpose computing near memory and are beneficial for embedded systems and gain increasing attention from academia and industry. The Workshop on Agile Design and Optimization Tools for Processing-In-Memory (DOT-PIM) will invite the leading experts from the PIM community to share their wonderful achievements in design and optimization tools for PIM. We hope DOT-PIM can help researchers to better understand the design challenges of PIM and inspire further research directions.

DOT-PIM also aims to attract research work with original contributions that address design challenges in PIM architectures & circuits and promote the performance of PIM architectures. The workshop is co-located with ESWEEK 2023 to attract the large ESWEEK audience. Topics of interest include, but are not limited to:
* Simulation and modeling tools for PIM architectures
* Instruction Set Architectures (ISA) and compilers for non-von Neumann computing paradigms
* High-level synthesis and logic synthesis tools for PIM architectures & circuits
* Physical design automation tools for PIM circuits
* Novel PIM architectures for new applications
* Domain-specific PIM architectures and algorithms co-optimization
* Security and reliability enhancement for emerging PIM systems

DOT-PIM will summarize and result in a survey paper about PIM design tools (submitted to related ACM/IEEE journals, e.g., ACM TODAES, IEEE TCAD, etc.). All posters presented in the workshop can be reported and featured in the survey paper. Presenters of the poster will also be invited as co-authors of the survey paper.

We invite your poster submissions for DOT-PIM. A two-page PDF abstract of the research work should be submitted to Prof. Yu Wang (yu-wang@tsinghua.edu.cn) via email. Abstracts should be in PDF form in two-column format, up to 2 pages in length with 1-inch margins and 10–11-point font size. Abstracts should list the full names and affiliations of all authors and the contact information of the corresponding author. Abstracts will be reviewed by the Program Committee. Those that are selected for poster presentations will be distributed to workshop participants.


#### Important Dates

Abstract submission deadline: 15 August 2023

Notification date: 22 August 2023

Workshop date: 21 September 2023

#### Workshop Chair & Contact:
Yu Wang (yu-wang@tsinghua.edu.cn), Tsinghua University, CN.

## Organizers
Yu Wang (Workshop Chair, yu-wang@tsinghua.edu.cn), professor, IEEE fellow, chair of the Department of Electronic Engineering of Tsinghua University, dean of the Institute for Electronics and Information Technology in Tianjin, and vice dean of the school of information science and technology of Tsinghua University. His research interests include application-specific heterogeneous computing, processing-in-memory, and power/reliability-aware system design methodology. Yu Wang has published more than 80 journals (51 IEEE/ACM journals in recent five years) and 200 conference papers in the areas of EDA, FPGA, VLSI Design, and Embedded Systems, with the Google citation more than 15,000. He has received four best paper awards and 11 best paper nominations. He will serve as TPC chair for ASP-DAC 2025. He serves as the editor of important journals in the field, such as ACM TODAES and IEEE TCAD and program committee member for leading conferences in the top EDA and FPGA conferences.

**Speakers:**

Yu (Kevin) Cao, Professor, IEEE fellow, Arizona State University. His research interests include neural-inspired computing, hardware design for on-chip learning, and reliable integration of nanoelectronics. He served as Associate Editor of the IEEE Transactions on CAD and on the technical program committee of many conferences.

Yiran Chen, Professor, IEEE/ACM fellow, Duke University. His group focuses on the research of new memory and storage systems, machine learning and neuromorphic computing, and mobile computing systems.  He is now serving as the Editor-in-Chief of the IEEE Circuits and Systems Magazine. He received the IEEE Computer Society Edward J. McCluskey Technical Achievement Award, ACM SIGDA Service Award, etc.

Kwang-Ting Cheng (Fengbin Tu), Professor, IEEE fellow, Hong Kong University of Science and Technology. Prof. Cheng is a world authority in the field of electronics testing, design verification, and design automation of electronics. He was recognized in the 50th DAC in 2013 as a Top 10 Author in DAC’s Fourth Decade and a Prolific Author.

Onur Mutlu, Professor, IEEE/ACM fellow, ETH Zurich. His current research interests are in computer architecture, systems, hardware security, and bioinformatics. He received the IEEE Computer Society Edward J. McCluskey Technical Achievement Award, the ACM SIGARCH Maurice Wilkes Award.

Huaqiang Wu, Professor, director of Microelectronics, Tsinghua University. His research interests include advanced memory and brain-inspired computing technologies. He has published 100 papers in top journals such as Nature, Nature Nanotechnology, Nature Electronics, and international conferences such as IEDM, VLSI and ISSCC.

Xiaoming Chen, Associate Professor, Institute of Computing Technology, Chinese Academy of Sciences. His research interests are mainly focused on EDA and computer architecture. He was awarded the Excellent Young Scientists Fund of National Natural Science Foundation of China in 2021. He received the 2015 EDAA Outstanding Dissertation Award and the 2018 Alibaba DAMO Academy Young Fellow Award. 

Shimeng Yu (Yuan-Chun Luo), Professor, Georgia Institute of Technology. Prof. Yu’s research interests are nanoelectronic devices and circuits for energy-efficient computing systems. He won the NSF Faculty Early CAREER Award in 2016 and the ACM Special Interests Group on Design Automation (SIGDA) Outstanding New Faculty Award in 2018.

Abbas Rahimi, Research Staff, IBM Research-Zurich. His research interests lie in codesigning emerging algorithms and hardware systems with an emphasis on improving energy efficiency and robustness. He received the 2015 Outstanding Dissertation Award from the European Design and he was a co-recipient of the Best Paper Nominations at DAC (2013) and DATE (2019).


## Follow-up Plans
We hope to provide a final report/manuscript summarizing the highlights and essential outcomes from DOT-PIM for the community to review and refer to.
