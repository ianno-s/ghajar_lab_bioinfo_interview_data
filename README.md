## Ghajar Lab Bioinformatics “Technical” Challenge

Hello! The goal of this exercise is to conduct an analysis of a small single-cell transcriptomics dataset and make biological conclusions based on your findings. The dataset is adapted from the Tabula Sapiens single-cell human transcriptomic atlas by the Chan-Zuckerberg Initiative. You can read more about the dataset on their website [here](https://tabula-sapiens-portal.ds.czbiohub.org/)

Please conduct an analysis of your choice to elucidate a biological phenomenon. This could take the form of a novel set of marker genes, possible cell-cell communication factors, differential gene ontologies, etc. An example guiding question could be “What cell surface markers differentiate mammary epithelial cells from bone marrow cells?”, this has applications in isolating disseminated tumor cells from human bone marrow samples! You are free to investigate your question with whatever methodology you prefer (R scripts, Python notebooks, etc.). Please prepare a 10-15 minute presentation with figures where you explain your methods, results, and the biological conclusions of your findings. 

You will be provided with metadata and gene count matrices of various file sizes to accommodate your individual computational capacity. Please let us know if you need a smaller dataset prepared. 

**Included cell types**: Mammary epithelial, Bone marrow (all)

### Provided gene count CSV files:
- **ts_data_counts_all**: All cells (~18k), all genes with >100 detected reads (~30k)
- **ts_data_counts_5000_genes_all**: All cells, 5k top variable genes
- **ts_data_counts_2500_genes_all**: All cells, 2.5k top variable genes
- **ts_data_counts_2500_genes_medium**: 50% random sampling of cells (~9k), 2.5k top variable genes
- **ts_data_counts_2500_genes_small**: 25% random sampling of cells (~4.5k), 2.5k top variable genes

### Metadata fields
- **donor**: Set of donors available in the dataset. 
- **organ_tissue**: List of organs available in Tabula Sapiens.
- **gender**: Gender of donors available in the dataset. 
- **cell_ontology_class**: Cell type annotations using the Cell Ontology.
- **free_annotation**: Cell type annotations using free text.
- **compartment**: Functional compartment for each cell type.
- **manually_annotated**: Whether or not the corresponding value in Annotation has been manually verified by a tissue expert.
- **method**: smartseq2 (full-length) or 10x (3prime).
- **n_counts_UMIs**: number of counts (smartseq2) or UMIs (10x) per cell.
- **n_genes**: number of genes per cell.

