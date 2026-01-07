# The dataset of the automotive 3D shapes mapping human subjective complexity assessment


[![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.compind.2025.104358-blue)](https://doi.org/10.1016/j.compind.2025.104358)
> **Overview**:  
> This repository provides the dataset accompanying the paper  
> **“A learning model for perceived visual complexity assessment of automotive 3D shapes based on visual perception elements”**, published in *Computers in Industry (2025)*.

## Dataset Overview

This dataset contains 120 automotive 3D shape images and their pairwise comparison results for visual complexity assessment. The dataset has been renumbered with IDs from 1 to 120 for consistency.

### Dataset Structure

```
data/
├── car_images_120/          # Directory containing 120 car images
│   ├── sample_1.png
│   ├── sample_2.png
│   └── ...
│   └── sample_120.png
├── compare_results.csv      # Pairwise comparison results
└── README.md                # This file
```

### File Formats

#### Image Files (`car_images_120/`)
- **Format**: PNG images
- **Naming**: `sample_{id}.png` where `id` ranges from 1 to 120
- **Total**: 120 images
- **Content**: Automotive 3D shape renderings

#### Comparison Results (`compare_results.csv`)
- **Format**: CSV file with 4 columns
- **Columns**:
  1. **Index**: Sequential row number (starting from 1)
  2. **Image ID 1**: First image ID in the comparison (1-120)
  3. **Image ID 2**: Second image ID in the comparison (1-120)
  4. **Label**: Comparison result (0 or 1)
     - `0`: Image ID 1 is more complex than Image ID 2
     - `1`: Image ID 1 is less complex than Image ID 2

- **Statistics**:
  - Total comparisons: 7,140 pairs
  - Label distribution: 3,397 (label=0), 3,743 (label=1)
  - All image IDs are in the range [1, 120]

### Usage

The dataset can be used for:
- Training and evaluating visual complexity assessment models
- Pairwise comparison learning tasks
- Visual perception analysis of automotive 3D shapes

### Citation

If you use this dataset, please cite the original paper:
```bibtex
@article{shen2025learning,
  title   = {A learning model for perceived visual complexity assessment of automotive 3D shapes based on visual perception elements},
  author  = {Shen, Chengyi and Liu, Changao and Luo, Shijian and Zhang, Deyin and Wang, Yao},
  journal = {Computers in Industry},
  volume  = {173},
  pages   = {104358},
  year    = {2025},
  publisher = {Elsevier}
}

