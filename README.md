# Real-time Domain Adaptation in Semantic Segmentation

This project focuses on the challenge of semantic segmentation with an emphasis on real-time domain adaptation. The goal is to assign category labels to each pixel of an image, which is crucial for applications such as autonomous driving. The project addresses key challenges such as network performance, data labeling burdens, and the efficiency-complexity trade-off in real-time segmentation networks.

## Challenges

- **Network Performance:** Achieving high accuracy while maintaining efficiency in terms of parameters, latency, and hardware requirements.
- **Data Labeling:** Overcoming the time-consuming and expensive process of collecting pixel-wise annotations for training datasets.
- **Domain Adaptation:** Bridging the gap between synthetic training data (e.g., images from GTA5) and real-world application scenarios (e.g., urban scenes from Turin).

## Solutions

- **Real-time Segmentation Networks:** Optimizing networks to balance efficiency and complexity, making them suitable for deployment in real-time applications.
- **Synthetic Datasets:** Utilizing computer-generated images that closely resemble real images but are cheaper to produce and come with accurate, pixel-wise ground truth annotations.
- **Adversarial and Image-to-Image Domain Adaptation:** Employing advanced techniques to minimize the discrepancy between synthetic and real image domains, thereby improving the model's performance on real-world data.

## Project Structure

- `data/`: Contains both synthetic (e.g., GTA5 images) and real datasets (e.g., Cityscapes).
- `models/`: Stores the trained models, including segmentation networks and discriminators for domain adaptation.
- `notebooks/`: Jupyter notebooks for exploratory data analysis, visualization, and result presentation.
- `src/`: Source code for the segmentation networks, domain adaptation algorithms, and other utility scripts.
- `tests/`: Unit tests to ensure the reliability of the codebase.

## Getting Started

To get started with this project, clone the repository, install the required dependencies, and explore the Jupyter notebooks for detailed examples and usage:

```bash
git clone https://github.com/ramzimessaoud/real-time-domain-adaptation.git
cd real-time-domain-adaptation
pip install -r requirements.txt
```

## Preliminary Analysis

1. Train standard and real-time segmentation networks on real images (Cityscapes dataset).
2. Evaluate the networks in terms of performance, complexity, and inference speed.

## Training on Synthetic Data

1. Train the real-time network on synthetic images (GTA5 dataset) and assess the performance drop when testing on real datasets (Cityscapes).
2. Implement data augmentation techniques to improve the robustness and generalizability of the model.

## Domain Adaptation

Explore different domain adaptation strategies, including adversarial approaches and image-to-image translation techniques, to enhance model performance on real-world data.

