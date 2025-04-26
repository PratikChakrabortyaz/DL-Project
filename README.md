# Age-Invariant Face Recognition using GANs and Vision Transformers

This project presents a **unified deep learning framework** for **Age-Invariant Face Recognition (AIFR)** by combining **CycleGAN-based synthetic aging**, **contrastive and triplet loss learning**, and multiple feature extractors including **ResNet**, **EfficientNet**, and **Vision Transformers (ViT)**.

We address challenges like **large age gaps**, **dataset diversity**, and **robust identity preservation** across facial aging processes.

---

## 📚 Project Structure

- **GAN-Based Augmentation**: Use CycleGAN to create synthetic age-progressed images for training.
- **Feature Extraction**: Models like ResNet18, EfficientNet-B0, VGG19, ViT-B/16 extract robust facial embeddings.
- **Learning Strategies**:
  - **Contrastive Learning** (Siamese networks) on UTKFace.
  - **Triplet Loss Training** on MORPH dataset.
  - **Binary MLP Classification** on paired embeddings.
- **Evaluation**: Performance measured on UTKFace, MORPH, and FG-NET datasets using accuracy, contrastive loss, triplet loss, and embedding distance analysis.

---

## 🚀 Datasets Used

- **UTKFace**: Age, gender, and ethnicity-annotated facial dataset.
- **MORPH**: Large longitudinal face dataset for age progression study.
- **FG-NET**: Cross-age facial dataset for generalization testing.

---

## 🔥 Key Techniques

- **CycleGAN** for synthetic aging with identity preservation.
- **Siamese Networks** for contrastive embedding learning.
- **Triplet Loss** for age-robust feature discrimination.
- **Vision Transformers** (ViT) for global feature extraction.
- **MLP Classifiers** for identity similarity estimation.

---

## 🧪 Results Summary

| Model        | Task                   | Best Performance (%) |
|--------------|-------------------------|-----------------------|
| ViT          | MLP Classification       | 96.91                 |
| EfficientNet | MLP Classification       | 95.10                 |
| ResNet152    | Triplet Loss Training     | 94.75                 |
| EfficientNet | Zero-Shot FG-NET Transfer | 80.55                 |

- **CycleGAN augmentation** enhanced diversity and helped learning robust embeddings.
- **Transformer models** generalized better in age-variant face verification tasks.

---



