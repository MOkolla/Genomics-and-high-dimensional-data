# Genomics-and-high-dimensional-data

In this project, we will analyze a single-cell RNA-seq dataset, with the goal of unveiling hierarchical structure and discovering important genes. The datasets provided are all different subsets of a larger single-cell RNA-seq dataset, compiled by the Allen Institute. This data contains cells from the mouse neocortex, a region in the brain which governs higher-level functions such as perception and cognition.

The single-cell RNA-seq data comes in the form of a counts matrix, where
- each row corresponds to a cell
- each column corresponds to the normalized transcript compatibility count (TCC) of an equivalence class of short RNA sequences, rescaled to units of counts per million. You can think of the TCC entry at location (i, j) of the data matrix as the level of expression of the j-th gene in the i-th cell.

1.p1, which is a small, labeled subset of the data. It contains the count matrix X along with “ground truth" clustering labels y, which were obtained by scientists using domain knowledge and statistical testing. This is for use in Problem 1.

2.p2_unsupervised, which contains only a count matrix. This is for use in Problem 2.

3.p2_evaluation, which contains a labeled training and test set. This is for use in Problem 2 to evaluate feature selection.

The p2_unsupervised_reduced and p2_evaluation_reduced folders contain datasets with a reduced number of genes, in case you are unable to run some of the procedures on the larger versions. In particular, a full logistic regression could take 1 or 2 GB of memory to run.

In Problem 1 (autograded), you will explore a small subset of the data, using visualization and clustering methods to discover its structure.

In Problem 2 (written report/peer review), you will use the tools you had from Problem 1 to explore a larger subset of the data. Using clustering combined with logistic regression, you will discover informative features which can be used to distinguish cells of different types.

Finally, in Problem 3 (written report/peer review), you will revisit open-ended decisions you made in your analyses, such as T-SNE hyper-parameters or number of clusters chosen, and explore how robust your end results are to these potentially ambiguous decisions.