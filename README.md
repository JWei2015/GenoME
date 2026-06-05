
# GenoME

GenoME is a Mixture of Experts (MoE)-based generative model that integrates DNA sequence and cell-type-specific chromatin accessibility (ATAC-seq/DNase-seq) to predict a unified genomic profile across multiple scales and modalities. It enables individualized, multimodal prediction and perturbation of genomic profiles.

**Paper**: [bioRxiv Preprint](https://www.biorxiv.org/content/10.64898/2025.12.28.696482v1/) | **Demo Data**: [Data link](docs/)

![GenoME Overview](docs/Fig0.bmp)

## Key Features
- **Multi-modal Prediction**: Multimodal prediction of epigenomics, transcriptomics, and 3D chromatin architecture at base-pair to kilobase resolutions
- **Cross-Cell Generalization**: Cross-cell-type generalization to predict full regulatory landscapes for unseen or individualized cell types
- **Perturbation Analysis**: In silico perturbation analysis for simulating genetic and epigenetic perturbations and identifying functional regulatory connections

## Installation

### Quick install (recommended)
The simplest way to set up the environment is using the provided `environment.yml` file.
```bash
git clone https://github.com/JWei2015/GenoME.git
cd GenoME
conda env create -f environment.yml
conda activate genome          # check environment.yml for the exact environment name
pip install -e .

   
### Data Preparation
1. Input Formats:
- DNA sequence: FASTA format (hg38 reference genome)
- ATAC-seq/DNase-seq: BigWig format (base-pair resolution)
- Training targets: BigWig files for RNA-seq, ChIP-seq; cooler format for Hi-C
2. Data preprocessing：
see **Paper**:  [BioRxiv Preprint](https://www.biorxiv.org/) 


