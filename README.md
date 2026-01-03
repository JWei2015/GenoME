
# GenoME
a MoE-based generative model for individualized, multimodal prediction and perturbation of genomic profiles 

GenoME is a Mixture of Experts (MoE)-based generative model that integrates DNA sequence and cell-type-specific chromatin accessibility (ATAC-seq/DNase-seq) to predict a unified genomic profile across multiple scales and modalities.


## Key Features
- **Multi-modal Prediction**: Multimodal prediction of epigenomics, transcriptomics, and 3D chromatin architecture at base-pair to kilobase resolutions
- **Cross-Cell Generalization**: Cross-cell-type generalization to predict full regulatory landscapes for unseen or individualized cell types
- **Perturbation Analysis**: In silico perturbation analysis for simulating genetic and epigenetic perturbations and identifying functional regulatory connections

## Installation

### Dependencies
- Python 3.9+
- PyTorch 2.0+
- CUDA 11.8+
- PyTorch Lightning
- [cooler](https://github.com/open2c/cooler), [cooltools](https://github.com/open2c/cooltools)
- [kipoiseq](https://github.com/kipoi/kipoiseq), [pyBigWig](https://github.com/deeptools/pyBigWig)

### Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/JWei2015/GenoME.git
   cd GenoME
2. Install dependencies via conda:
   ```bash
   conda create -n genome python=3.9
   conda activate genome
   conda env update -f requirements.txt
   
### Data Preparation
1. Input Formats:
- DNA sequence: FASTA format (hg38 reference genome)
- ATAC-seq/DNase-seq: BigWig format (base-pair resolution)
- Training targets: BigWig files for RNA-seq, ChIP-seq; cooler format for Hi-C
2. Data preprocessing：
see **Paper**:  [BioRxiv Preprint](https://www.biorxiv.org/) 


