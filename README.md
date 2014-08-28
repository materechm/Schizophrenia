Schizophrenia
=============
##Schizophrenia Diseasome 
![] (https://raw.githubusercontent.com/materechm/Schizophrenia/master/diseasome%20graph.jpg)
In order to create a diseasome, a larger network of diseases (nodes) connected to genes (edges) is created first, where connections (edges) come from the GWAS catalog, and the OMIM database. The Disease Ontology (DO)  is used to provide a standardized terminology for disease concepts across both resources. Two processing steps are performed on the resulting network of DO terms annotated with associated genes: (1) closely related concepts are merged by transferring annotations to a single term and removing the other term (for example ‘breast cancer’ is consolidated with ‘breast carcinoma’); and (2) terms of inappropriate generality are removed such as ‘immune system disease’.

The edge weight between diseases in the network is calculated as the intersection of genes divided by the union of genes. Edges between diseases with no shared genes are omitted. To verify accuracy of calculations, the results from Cotsapas and Hafler were replicated.

The network was graphed using cytoscape.

537 conditions from the GWAS catalog and OMIM were found to share genes with Schizophrenia. After processing the resulting network of DO terms, the amount of conditions was reduced to 101.

##Predicting influential SZ genes

![] (https://raw.githubusercontent.com/materechm/Schizophrenia/master/genes%20graph.png)

I decided to use text mining to generate a list of seed genes. I included genes with an R scaled score of >= 35 that showed up in >= 3 abstracts. The result was a seed list containing 235 genes. I then used the seed genes to initiate pagerank on gene networks (co-expression, physical interaction, predicted interactions, co-localization, shared protein domains, genetic interactions and pathways), to calculate a measure of influence for each gene. 20 genes that were not initially on my seed list were ranked highly, which means they are likely associated with the disease. 

The seed + newly found genes have diverse functions, the function with greatest coverage is Glutamate Receptor Activity. 

Next I used UChicago's eQTL Browser to find eQTLs on or near the genes on my 2 lists. 
