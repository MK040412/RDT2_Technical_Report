# RDT2 Technical Report

A comprehensive Beamer presentation explaining the RDT2 (Robotics Diffusion Transformer 2) architecture, training pipeline, and inference process.

## Purpose

This presentation is designed to provide detailed technical understanding of RDT2 for:
- Debugging integration with ManiSkill
- Understanding the complete data flow from images to robot actions
- Visualizing model architecture and dimension transformations

## Usage

### With Overleaf

1. Go to Overleaf and create a new project
2. Select "Import from GitHub"
3. Connect to this repository: `https://github.com/MK040412/RDT2_Technical_Report.git`
4. Compile `main.tex`

### Local Compilation

```bash
pdflatex main.tex
pdflatex main.tex  # Run twice for TOC
```

## Contents

The presentation covers:

1. **Overview** - RDT2 core concepts and model variants
2. **UMI Hardware & Data Collection** - Hardware platform and dataset
3. **Action Representation** - 20-D bimanual action structure
4. **VQVAE Action Tokenizer** - Complete tokenization pipeline
5. **RDT2-VQ Architecture** - Autoregressive VLA model
6. **RDT2-FM Architecture** - Flow-matching action expert
7. **Training Pipeline** - Stage 1 (VQ) and Stage 2 (FM) training
8. **Inference Pipeline** - Complete inference flow with TikZ diagrams
9. **Normalizer** - Critical normalization/unnormalization
10. **ManiSkill Integration** - Debugging checklist and adaptation guide
11. **File Reference** - Key files for training and inference

## Key Visualizations

- Model architecture diagrams (TikZ)
- Dimension flow diagrams
- VQVAE encoding/decoding pipeline
- Token conversion formulas
- Complete inference pipeline

## Theme

- Beamer theme: **Beaver** (default)
- Aspect ratio: 16:9

## References

- [RDT2 Project Page](https://rdt-robotics.github.io/rdt2/)
- [GitHub Repository](https://github.com/thu-ml/RDT2)
- [RDT2-VQ on HuggingFace](https://huggingface.co/robotics-diffusion-transformer/RDT2-VQ)
- [RDT2-FM on HuggingFace](https://huggingface.co/robotics-diffusion-transformer/RDT2-FM)
