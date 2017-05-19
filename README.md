**Network Enhancement** *(Network Enhancement: a general method to denoise weighted biological networks)*
===============================


**OVERVIEW**
Networks are abundant in many areas of biology. These networks often entail non-trivial topological features and patterns critical to understanding interactions within the natural system. However, networks observed in real-world are typically noisy. The presence of high levels of noise can hamper discovery of structures and dynamics present in the network. In this paper, we propose Network Enhancement (NE) as a novel method for improving the signal-to-noise ratio of a symmetric
networks and thereby facilitating the downstream network analysis. NE leverages the transitive edges of a network by exploiting local structures to strengthen the signal within clusters and weaken the signal between clusters. At the same time NE also alleviates the corrupted links in the network by imposing a normalization that removes weak edges by enforcing sparsity. NE is supported by theoretical justifications for its convergence and performance in improving community
detection outcomes. Finally, we demonstrate the effectiveness of NE in improving the performance of community detection algorithms by applying NE as a noise reduction step to several real-world biological networks. Finally, we apply NE for gene function prediction and observed higher prediction accuracy over state-of-the-art methods.
**SIMLR**

*SIMLR* offers three main unique advantages over previous methods: (1) it learns a distance metric that best fits the structure of the data via combining multiple kernels. This is important because the diverse statistical characteristics due to large noise and dropout effect of single-cell data produced today do not easily fit specific statistical assumptions made by standard dimension reduction algorithms. The adoption of multiple kernel representations provides a better fit to the true underlying statistical distribution of the specific input scRNA-seq data set; (2) *SIMLR* addresses the challenge of high levels of dropout events that can significantly weaken cell-to-cell similarities even under an appropriate distance metric, by employing graph diffusion, which improves weak similarity measures that are likely to result from noise or dropout events; (3) in contrast to some previous analyses that pre-select gene subsets of known function, *SIMLR* is unsupervised, thus allowing de novo discovery from the data. We empirically demonstrate that *SIMLR* produces more reliable clusters than commonly used linear methods, such as principal component analysis (PCA), and nonlinear methods, such as t-distributed stochastic neighbor embedding (t-SNE), and we use *SIMLR* to provide 2-D and 3-D visualizations that assist with the interpretation of single-cell data derived from several diverse technologies and biological samples. 

**REFERENCE**

The latest draft of thr manuscript related to *SIMLR* can be found as a preprint at http://biorxiv.org/content/early/2016/06/09/052225. 

**DOWNLOAD**

The R code to run *SIMLR* can be downloaded either from the master (stable version) or from the development (development version) branches, while the Matlab implementation is available from the matlab branch.  

**RUNNING SIMLR ON MATLAB**

We also provide the Matlab code to run *SIMLR* on 4 examples in the script *main_demo.m*. 

**EXTERNAL C CODE** 

We make use of external C programs during the computations of *SIMLR*. The code is located in the src directory in the files *Kbeta.cpp* and *projsplx_c.c*. In order to compite the program, one needs to run on the Matlab consolle the commands *mex Kbeta.cpp* and *mex projsplx_R.c*. 

OS X pre-compiled files are also provided. 
