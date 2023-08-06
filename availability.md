---
title: ""
layout: page
full_logo: true
output:
  html_document:
    toc: yes
    toc_depth: 4
---

# Support for the FAIR principles

The FAIR principles [[1](https://www.nature.com/articles/sdata201618)] are considered a gold standard for research data management. In this work, we follow best practices for improving the support for them in the HIHISIV database. For improving `findability`, basic metadata using schema.org [[2](https://queue.acm.org/detail.cfm?id=2857276)] was added to the headers of the HIHISIV web page, allowing for indexing by search engines and dataset repositories. HIHISIV data and metadata are openly `accessible` through its [URL (https://hihisiv.github.io)](https://hihisiv.github.io) using the HTTP protocol. When applicable, terms used both in the database schema and in its web interface follow Gene Ontology [[3](https://www.nature.com/articles/ng0500_25)] and other ontologies such as [EFO](https://www.ebi.ac.uk/efo/) - The Experimental Factor Ontology, [UBERON](https://genomebiology.biomedcentral.com/articles/10.1186/gb-2012-13-1-r5) - Uber-anatomy ontology, [PATO](http://obofoundry.org/ontology/pato.html) - the Phenotype And Trait Ontology, [MONDO](https://mondo.monarchinitiative.org/) - Mondo Disease Ontology and [NCIT](https://obofoundry.org/ontology/ncit.html) - The National Cancer Institute Thesaurus improving `interoperability`. For better `reusability`, the database contains references to the original data used in the analyses. The source code for the analysis workflows, the database schema and initialization scripts, and the web application is available on [Github](https://github.com/quelopes/hihisiv). This article describes v2.0 of the database, which is archived on Zenodo under [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7093185.svg)](https://doi.org/10.5281/zenodo.7093185). 



# Additional datasets

Results of differential gene expression analysis in SIV infection in *Chlorocebus sabaeus* and *Macaca mulatta*.
The raw datasets are from the [MACE](http://mace.ihes.fr) transcriptome repository and used ABI Human Whole Genome Arrays v2.0 (Applied Biosystems). They have not been incorporated into the HIHISIV database but the results of the analysis are available in: 
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8219165.svg)](https://doi.org/10.5281/zenodo.8219165).










