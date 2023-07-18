---
title: ""
layout: page
full_logo: true
output:
  html_document:
    toc: yes
    toc_depth: 4
---

# Querying in the user interface 

HIHISIV can be queried through a web interface in which the user can configure and adjust the parameters of a query. There are six query interfaces with major analytic functions, which are `Genes`, `Transcripts` (for microarray platforms), `Gene Ontology`, `Traits`, `Single gene co-expression network`, and `Gene set co-expression network`. The resulting information can be exported in comma-separated values (CSV) file for further data manipulation. 

<!---
=== GENE ===
--->
### Gene

In this mode, the user can select a gene of interest (by gene symbol or Entrez gene id) and assess which experiments the gene selected was differentially expressed, which were the host type and tissue. The example below shows the result of the gene *NCAM1* with the threshold of the adjusted p-value <= 0.05 and log fold-change (log-FC) = 0.

![Example in Query type `Gene`.](assets/img/query_genes.png)


<!---
=== TRANSCRIPT ===
--->
### Transcript

Instead of the query by gene symbol or Entrez gene id, the user can be interested in a specific probe id and this is possible in this module. The probe id `MmuSTS.2130.1.S1_s_at` is selected in the example below (adjusted p-value <= 0.05 and logFC =0). 

![Example in Query type `Gene`.](assets/img/query_transcripts.png)


<!---
=== GENE ONTOLOGY ===
--->
### Gene Ontology

This mode provides mappings between Entrez gene id and the GO identifiers that they are directly associated with. The example below shows the selected BP term by GO term `response to the virus` with threshold adjusted p-value <= 0.05 and log-FC >= 1. 

![Example in Query type `Gene Ontology`.](assets/img/query_go.png)


<!---
=== TRAIT ===
--->
### Trait

In this module interface is possible to select genes that play fundamental roles in understanding the complexity of the immune system. The example follow example shows the relevant genes that will comprise the `cell_surface` considering the host type `non-natural`, the design type `pre-infection vs acute`  (adjusted p-value <= 0.05 and log-FC <= -4).

![Example in Query type `Trait`.](assets/img/query_traits.png)


<!---
=== SINGLE GENE CO-EXPRESSED ===
--->

### Single gene co-expression network

This query mode represents the genes that were co-expressed with a target gene selected. 
In the example below, the *GZMA* gene was selected (adjusted p-value =< 0.05 and log-FC = 1.5) and the result shows a set of genes co-expressed with *GZMA* in different experiments (ex: *PECAM1*, *NOX1*, *CCL5*, and *KDELR2*). The thickness of the connections between genes depends on the number of co-expressed experiments that the target gene has with the resulting gene. In this example, the *PECAM1* gene is co-expressed with the *GZMA* gene in several experiments. The result of the query can be visualized as a graph representing the gene co-expression network as well as a tabular format.  

![Example in Query type `Single gene co-expression network`.](assets/img/query_single_co-expression.png)


<!---
=== GENE SET CO-EXPRESSION ===
--->
### Gene set co-expression network

In this query mode instead of one gene a set of genes can be entered and the result shows a network where the genes connected were co-expressed in one or more experiments. In the example of Figure 9, the parameters adjusted p-value =< 0.01 and log-FC = 1 were applied and the follow Entrez gene id with the respective genes symbol were selected:  891 (*CCNB1*); 890 (*CCNA2*); 9289 (*ADGRG1*); 8892 (*EIF2B2*); 1894 (*ECT2*); 1890 (*TYMP*); 79898 (*ZNF613*); 56895 (*AGPAT4*); 55789 (*DEPDC1B*); 1263 (*PLK3*) and 332 (*BIRC5*). In this mode, it is also possible to visualize the connections from PPI where the edges are represented in red.

![Example in Query type `Gene set co-expression network`.](assets/img/query_set_co-expression.png)