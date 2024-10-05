# Pathogenicity Island Pattern Mining in Bacterial Genomes

## Project Description
This project aims to identify patterns within pathogenicity islands (PAIs) of bacterial genomes. We focus on two bacterial species: Escherichia coli and Helicobacter pylori. The project utilizes data mining techniques to find recurring patterns across different genomes and their associated PAIs.

## Authors
- Veljko Prodan
- Maja Milenković

## Features
- Pattern mining in pathogenicity islands of E. coli and H. pylori genomes
- Usage of TFIDF and NOSEP algorithms for pattern discovery
- Cross-genome analysis to identify recurring patterns
- Data organization and storage

## Technologies Used
- Python
- Jupyter Notebook
- [SPMF](https://www.philippe-fournier-viger.com/spmf/) library (for NOSEP algorithm)
- TFIDF algorithm

## Data Sources
FASTA files for E. coli and H. pylori genomes were obtained from [PAIDB](http://paidb.re.kr).

## Project Structure
```
root/
│
├── docs/
│ └── seminarski.pdf
│
├── e_coli/
│ ├── src/
│ │ ├── nosep.ipynb
│ │ ├── tfidf.ipynb
│ │ └── recurring_patterns.ipynb
│ ├── logs/
│ ├── json/
│ ├── csv/
│ └── e_coli_data/
│     └── NC_XXXXXX/
│         ├── NC_XXXXXX.fasta
│         ├── NC_XXXXXX.pai
│         ├── NC_XXXXXX.cpai
│         ├── NC_XXXXXX.npai
│         └── patterns/
│
└── h_pylori/
    └── (similar structure as e_coli/)
```

## Methodology
1. Data Collection: FASTA files for E. coli and H. pylori genomes collected from PAIDB.
2. Pattern Mining: 
   - TFIDF algorithm was applied to identify significant patterns.
   - NOSEP algorithm (using SPMF library) was used for additional pattern discovery.
3. Cross-Genome Analysis: Patterns were compared across different genomes to identify recurring motifs.

## Results
The project generates several output files:
- CSV files mapping patterns to specific genomes and islands
- JSON files containing pattern information for each genome
- Text files in the `patterns` folder of each genome, listing discovered patterns

Detailed results and analysis can be found in the respective Jupyter notebooks.
