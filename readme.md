# HaNa: Hardness and Noise-Aware Robust Cross-modal Retrieval

Official PyTorch implementation of **HaNa** (Hardness and Noise-Aware robust cross-modal retrieval), accepted by AAAI 2026.

## 📖 Abstract

Noisy correspondence in cross-modal retrieval introduces significant challenges due to its inherent difficulty in identification and correction. Although existing methods attempt to minimize the influence of noisy samples by the weighting mechanism, these methods still struggle with performance degradation under increasing noise levels. Specifically, the clean samples are assigned the same weight of 1, which ignores the sample hardness. In addition, the weights for noisy samples are approaching 0, leading to the overlook of sample diversity. To address these issues, we propose a Hardness and Noise-aware (HaNa) robust cross-modal retrieval method. HaNa introduces a momentum-based reweighting mechanism to adaptively balance learning difficulty across clean samples, avoiding overfitting risk and accumulative partitioning bias. Moreover, HaNa addresses the limitation that weights for noisy data are approaching 0 from a new perspective to fully employ the diversity of samples to further improve its generalization. It employs an Asymmetric Noise-aware Regularization Loss (ANRL) to treat identified noisy data as negative samples for optimization. Extensive experiments demonstrate that HaNa achieves superior matching accuracy and stability, especially in high-noise scenarios, outperforming state-of-the-art methods.

## 🚀 Code Status

**Code: Coming Soon**

We are currently cleaning and refactoring the code for better readability. The complete implementation will be released in the future.

## 📊 Dataset and Baselines

For dataset preparation and baseline implementations, please refer to this nice work:

**[NPC](https://github.com/ZhangXu0963/NPC)**

### Supported Datasets

- **Flickr30K**
- **MS-COCO**
- **CC120K**

## 🛠️ Installation & Usage

```bash
# Clone this repository (when available)
git clone https://github.com/haiquan-yu/HaNa.git
cd HaNa

# Install dependencies
pip install -r requirements.txt

# Prepare datasets (follow NPC instructions)
# Training and evaluation scripts will be provided
