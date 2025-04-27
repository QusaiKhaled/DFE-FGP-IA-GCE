# Interpretable Fuzzy Systems for Forward Osmosis Desalination

This repository contains the code and resources for the paper **Interpretable Fuzzy Systems for Forward Osmosis Desalination**  

> A novel approach to predict membrane flux in forward osmosis desalination using an interpretable fuzzy rule–based system (FRBS), integrating expert knowledge with data-driven techniques.

---

## 📖 Overview

We propose a hybrid method that is both **accurate** and **interpretable**. It predicts the membrane flux (L/m²·h) while enforcing semantic and structural interpretability:

1. **Domain-oriented Feature Engineering (DFE)**  
   - Selecting three key features
   - Leveraging membrane science equations to reduce dimensionality  

2. **Fixed Expert-defined Grid Partitioning (FGP)**  
   - Partitions each feature into three fuzzy sets (low, medium, high) using expert parameters  
   - Ensures **coverage**, **normality**, and **distinguishability**

3. **Rule Inactivity Checking (IA)**  
   - Prunes rules whose normalized firing strength < 10⁻²  
   - Reduces the rule base from 27 to 15 rules

4. **Regularized Global Consequent Estimation (GCE)**  
   - Fits consequents via ridge-regularized least squares  
   - Grid-search over λ ∈ [0.001, 10] (optimal λ = 1.314) to avoid overfitting  
   - Ensures every rule contributes meaningfully
---
## Dependencies
Python ≥ 3.8

Libraries:

numpy

pandas

scikit-learn

pyFUME

Simpful

---

## 📝 Citation

If you use this code, please cite:

@inproceedings{Khaled2025interpretable,
  title={Interpretable Fuzzy Systems for Forward Osmosis Desalination},
  author={Khaled, Qusai and Kaymak, Uzay and Genga, Laura},
  booktitle={2025 IEEE International Conference on Fuzzy Systems (FUZZ-IEEE)},
  pages={1--7},
  year={2024},
  organization={IEEE}
}


---


## 📚 Dataset

Experimental Forward Osmosis desalination data
the dataset is obtained from the paper **Modeling of forward osmosis process using artificial neural networks (ANN) to predict the permeate flux**
can be found here
doi.org/10.1016/j.desal.2020.114427
can be cited here
@article{jawad2020modeling,
  title={Modeling of forward osmosis process using artificial neural networks (ANN) to predict the permeate flux},
  author={Jawad, Jasir and Hawari, Alaa H and Zaidi, Syed},
  journal={Desalination},
  volume={484},
  pages={114427},
  year={2020},
  publisher={Elsevier}
}


---

## 🙏 Acknowledgment

Part of **ILUSTRE** (Innovation Lab for Utilities on Sustainable Technology and Renewable Energy),  
within NWO’s LTP ROBUST programme.

---

## 📬 Contact

For issues or questions, please [open an issue]
or email **Qusai Khaled** at <qusai.khaled@ieee.org>.
```
