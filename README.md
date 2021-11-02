# BiomedicalConceptAlignment
Datasets, trained models and source code to "Neural Methods for Biomedical Synonym Discovery and Concept Alignment" thesis


Please download the datasets folder from the following link: https://mega.nz/folder/Z0kz2Y4Y#z-fwSUdmHSXn2mnMATRe1Q

To obtain weights of trained models with the wikidata dataset used in the thesis, please download weights folder from the following link: https://mega.nz/folder/NksGHaBA#sDrRUTswmXdQzSYv-cM7HQ 


Requires ```pytorch``` and ```pytorch-lightning```

Usage:

```python3 main.py --model=MODEL --train=TRAIN --test=TEST```

where 

MODEL in ```{'rs_pool', 'r_transformer', 'rs_pool_emb', 'r_transformer_emb' }```

TRAIN/TEST in ```{'wikidata_training', 'wikidata_test', 'pairs_uberon', 'pairs_snomed', 'pairs_ordo', 'pairs_ncit_subset', 'pairs_mpo', 'pairs_ma', 'pairs_hpo', 'pairs_hdo', 'pairs_fma', 'ncbi-disease-entities', 'ma_ncit_pairs', 'ma_ncit_pairs_2', 'fma_ncit_pairs', 'fma_ncit_pairs_2'}```

Results will be in a generated (or appended to the end of a) ```results.txt``` file.


