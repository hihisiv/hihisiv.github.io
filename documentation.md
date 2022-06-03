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

HIHISIV can be queried through a web interface in which the user can configure and adjust various parameters of a query. There are five query interfaces with major analytic functions, which are `Gene`, `Gene Ontology`, `Traits`, `Single gene co-expression network`, and `Gene set co-expression network`. The resulting information can be exported in comma-separated values (CSV) for further data manipulation. Public access and documentation are freely available through the [database web page](http://www.lncc.br/HIHISIV/).

<!---
=== GENE ===
--->
### Gene

In this mode, the user can select a gene of interest (by gene_symbol or entrez_gene_id) and assess how much and in which experiments this gene was differentially expressed, which were the host type and tissue.
For example, the gene *NCAM1* with the threshold of the adjusted p-value $<=$ 0.05 and abs(logFC) $=$ 0.

![Example in Query type `Gene`.](assets/img/query_gene.png)

<!---
=== GENE ONTOLOGY ===
--->
### Gene Ontology

This mode provides mappings between entrez_gene_id and the GO identifiers that they are directly associated with.
The GO is divided into three domains, which are molecular function (MF), biological process (BP), and cellular component (CC) (cite GO, nature genetics 2000, Ashburner_2000).

The example below shows the selected BP term `response to the virus` with threshold adjusted p-value $<$ 0.05 and log fold-change $>=$ 1.

![Example in Query type `Gene Ontology`.](assets/img/query_go.png)


<!---
=== TRAIT ===
--->
### Trait

(more)

The example below shows the result of the trait selected `cell_surface_NCBI`  overexpressed with p-value $<=$ 0.05 and log-FC $<=$ -4 (in nonspecific design).

![Example in Query type `Trait`.](assets/img/query_trait.png)


<!---
=== SINGLE GENE CO-EXPRESSED ===
--->

### Single gene co-expression network

This query mode represents the genes that were co-expressed with a target gene selected.
For instance, selecting the gene *GZMA* with adjusted p-value $< 0.05$ the result shows a set of genes co-expressed with *GZMA* in different experiments (ex: *CREB3L3*, *NOX1*, *CCL5* and *KDELR2*).
The thickness of the connections between genes depends on the number of co-expressed experiments that the target gene has with the resulting gene. In this example, the *CREB3L3* gene is co-expressed with the *GZMA* gene in several experiments.

The result of the query can be visualized as a graph representing the gene co-expression network as well as a tabular format. It can be also be downloaded as a comma-separated values (CSV) file.  

![Example in Query type `Single gene co-expression network`.](assets/img/query_single_co-expression.png)


<!---
=== GENE SET CO-EXPRESSION ===
--->
### Gene set co-expression network

In this query mode instead of one gene (as shown in the last example), a set of genes can be entered and the result shows a network where the genes connected were co-expressed in one or more experiments. In this mode is also possible to visualize the connections from PPI where the edges are represented in red.

![Example in Query type `Gene set co-expression network`.](assets/img/query_set_co-expression.png)