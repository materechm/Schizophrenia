Schizophrenia
=============
##About Schizophrenia 

Schizophrenia is a mental disorder that makes it difficult to tell what is real and what isn't manage emotions, and relate to others, among other symptoms. Between 0.3% and 0.7% of people have the disorder.

Schizophrenia affects men and women equally and the rate is similar in all ethnic groups. Hallucinations and delusions usually appear between the ages of 16-30, and most of the time people do not get schizophrenia after 45.

##Schizophrenia Diseasome 
![] (https://raw.githubusercontent.com/materechm/Schizophrenia/master/diseasome%20graph.jpg)
In order to create a diseasome, a larger network of diseases (nodes) connected to genes (edges) is created first, where connections (edges) come from the GWAS catalog, and the OMIM database. The Disease Ontology (DO)  is used to provide a standardized terminology for disease concepts across both resources. Two processing steps are performed on the resulting network of DO terms annotated with associated genes: (1) closely related concepts are merged by transferring annotations to a single term and removing the other term (for example ‘breast cancer’ is consolidated with ‘breast carcinoma’); and (2) terms of inappropriate generality are removed such as ‘immune system disease’.

The edge weight between diseases in the network is calculated as the intersection of genes divided by the union of genes. Edges between diseases with no shared genes are omitted. To verify accuracy of calculations, the results from Cotsapas and Hafler were replicated.

The network was graphed using cytoscape.

537 conditions from the GWAS catalog and OMIM were found to share genes with Schizophrenia. After processing the resulting network of DO terms, the amount of conditions was reduced to 101.
