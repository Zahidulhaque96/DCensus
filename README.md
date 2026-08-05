Official implementation of the paper:
DCensus: Directed Census Invariant Descriptors for Real-World Complex Networks
Tuhalika Saha, Md. Zahidul Haque, Md. Maruf Mia, Md. Manzurul Hasan  
Department of Computer Science, American International University-Bangladesh (AIUB)
---
Overview
DCensus is a direction-aware graph invariant framework for analyzing directed networks.  
It independently models outbound and inbound neighborhood expansion using dual BFS traversals and produces three complementary descriptors:
DCensus-Node → neighborhood growth
DCensus-Edge → directional connectivity
DCensus-Stub → structural redundancy
The framework is deterministic, interpretable, and scalable.
---
Datasets
We evaluate DCensus on three standard directed networks from SNAP:
Dataset	Nodes	Edges
Email-EuAll	265,214	420,045
Wiki-Vote	7,115	103,689
Cit-HepTh	27,770	352,807
Download the datasets and place the `.txt` files inside the `data/` folder:
