**Network Enhancement** *(Network Enhancement: a general method to denoise weighted biological networks)*
===============================


**OVERVIEW**
Networks are abundant in many areas of biology. These networks often entail non-trivial topological features and patterns critical to understanding interactions within the natural system. However, networks observed in real-world are typically noisy. The presence of high levels of noise can hamper discovery of structures and dynamics present in the network. In this paper, we propose Network Enhancement (NE) as a novel method for improving the signal-to-noise ratio of a symmetric
networks and thereby facilitating the downstream network analysis. NE leverages the transitive edges of a network by exploiting local structures to strengthen the signal within clusters and weaken the signal between clusters. At the same time NE also alleviates the corrupted links in the network by imposing a normalization that removes weak edges by enforcing sparsity. NE is supported by theoretical justifications for its convergence and performance in improving community
detection outcomes. Finally, we demonstrate the effectiveness of NE in improving the performance of community detection algorithms by applying NE as a noise reduction step to several real-world biological networks. Finally, we apply NE for gene function prediction and observed higher prediction accuracy over state-of-the-art methods.


**RUNNING NE ON MATLAB**

At current stage, we provide two example scripts to run NE on two experiments mentioned in the manuscript. The first is butterfly species retrieval *run_butterfly_network.m*. But running this script you should get both accuracy number and retrieval curve reported in the manuscript.
The second is HiC network denosing. We provide an example data on Chrom 16 with two resolutions. However, if you want to apply module detection on the networks, you need to compile two cpp files. Instructions are given in the script *run_hiC_network.m*

