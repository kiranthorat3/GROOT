## GROOT: Graph Edge Re-growth and Partitioning for the Verification of Large Designs in Logic Synthesis
---
### 📄 Abstract

Abstract—Traditional verification methods in chip design are
highly time-consuming and computationally demanding, espe-
cially for large scale circuits. Graph neural networks (GNNs)
have gained popularity as a potential solution to improve veri-
fication efficiency. However, there lacks a joint framework that
considers all chip design domain knowledge, graph theory, and
GPU kernel designs. To address this challenge, we introduce
GROOT, an algorithm and system co-design framework that
contains chip design domain knowledge and redesigned GPU
kernels, to improve verification efficiency. More specifically, we
create node features utilizing the circuit node types and the
polarity of the connections between the input edges to nodes
in And-Inverter Graphs (AIGs). We utilize a graph partitioning
algorithm to divide the large graphs into smaller sub-graphs
for fast GPU processing and develop a graph edge re-growth
algorithm to recover verification accuracy. We carefully profile
the EDA graph workloads and observe the uniqueness of their
polarized distribution of high degree (HD) nodes and low degree
(LD) nodes. We redesign two GPU kernels (HD-kernel and LD-
kernel), to fit the EDA graph learning workload on a single GPU.
We compare the results with state-of-the-art (SOTA) methods:
GAMORA, a GNN-based approach, and the traditional ABC
framework. Results show that GROOT achieves a significant
reduction in memory footprint (59.38 %), with high accuracy
(99.96%) for a very large CSA multiplier, i.e. 1,024 bits with
a batch size of 16, which consists of 134,103,040 nodes and
268,140,544 edges. We compare GROOT with GPU-based GPU
Kernel designs SOTAs such as cuSPARSE, MergePath-SpMM,
and GNNAdvisor. We achieve up to 1.104×, 5.796×, and 1.469×
improvement in runtime, respectively.


### Codes are coming soon
