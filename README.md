# GenoME
a MoE-based generative model for individualized, multimodal prediction and perturbation of genomic profiles 

GenoME is a Mixture of Experts (MoE)-based generative model that integrates DNA sequence and cell-type-specific chromatin accessibility (ATAC-seq/DNase-seq) to predict a unified genomic profile across multiple scales and modalities. It enables:

* Multimodal prediction of epigenomics, transcriptomics, and 3D chromatin architecture at base-pair to kilobase resolutions
* Cross-cell-type generalization to predict full regulatory landscapes for unseen or individualized cell types
* In silico perturbation analysis for simulating genetic and epigenetic perturbations and identifying functional regulatory connections

💾 Data Requirements
DNA sequence: FASTA format (hg38 reference genome)
ATAC-seq/DNase-seq: BigWig format (base-pair resolution)
Training targets: BigWig files for RNA-seq, ChIP-seq; cooler format for Hi-C

⚙️ Package Requirements
Python 3.9+
PyTorch 2.0+
CUDA 11.8+
