# DCensus

**Directed Census Invariant Descriptors for Real-World Complex Networks**

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![arXiv](https://img.shields.io/badge/arXiv-coming%20soon-b31b1b.svg)](#)

Official implementation of **DCensus**, a direction-aware graph invariant framework for analyzing directed networks.

> Tuhalika Saha, Md. Zahidul Haque, Md. Maruf Mia, Md. Manzurul Hasan  
> Department of Computer Science, American International University-Bangladesh (AIUB)

---

## Overview

DCensus extends the Census family of invariant descriptors (originally developed for undirected graphs) to **directed** networks.  

It independently models **outbound** and **inbound** neighborhood expansion using dual BFS traversals and produces three complementary descriptors:

| Descriptor       | Focus                        | What it captures                          |
|------------------|------------------------------|-------------------------------------------|
| **DCensus-Node** | Neighborhood growth          | How the reachable set expands with distance |
| **DCensus-Edge** | Directional connectivity     | Edge patterns between successive layers   |
| **DCensus-Stub** | Structural redundancy        | Half-edge (stub) statistics that reveal finer topological differences |

The framework is **deterministic**, **interpretable**, and **scalable** to networks with hundreds of thousands of nodes.

---

## Key Features

- Direction-aware dual BFS (outbound + inbound)
- Three complementary invariant descriptors
- Works on real-world directed networks from SNAP
- Parallelizable implementation
- Fully deterministic (no randomness)

---

## Installation

```bash
git clone https://github.com/Zahidulhaque96/DCensus.git
cd DCensus
pip install -r requirements.txt
