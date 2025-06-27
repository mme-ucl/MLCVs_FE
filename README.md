# MLCVs\_FE

This repository provides the code and trained models used to investigate the reproducibility of free energy surfaces (FESs) in the space of Machine-Learned Collective Variables (MLCVs), as discussed in our paper:
**"On the Reproducibility of Free Energy Surfaces in Machine-Learned Collective Variable Spaces"**
*Florian M. Dietrich and Matteo Salvalaglio, 2025*

Our work demonstrates how the stochastic nature of machine learning training processes affects the reproducibility of MLCV-based FESs. We propose the use of **geometric (gauge-invariant) free energy surfaces** as a robust alternative, and highlight the benefits of **gradient normalisation** for consistent enhanced sampling.

---

## 📁 Repository Contents

### Jupyter Notebooks

* **`FE_and_CVs.ipynb`**
  Performs feature engineering and visualizes the embedding of high-dimensional input data into low-dimensional CV spaces.

* **`FE_and_CVs_train_models.ipynb`**
  Trains simple autoencoder models with different architectural complexities on a toy dataset with known metastable states.

* **`analyse_weights_distance.ipynb`**
  Evaluates the variability across independently trained models by analysing distances in weight space. 

### Pretrained Models

Trained encoder weights (`.h5`) for autoencoders of varying complexity:

* `Models_4_2_4_ReLU/`
* `Models_8_2_8_ReLU/`
* `Models_16_2_16_ReLU/`
* `Models_16_8_2_8_16_ReLU/`

These models reproduce the results shown in **Fig. 1** and **Fig. 2** of the manuscript.


---

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/MLCVs_FE.git
   cd MLCVs_FE
   ```

--

## 🔗 Related Projects

* [NNucleate](https://github.com/mme-ucl/NNucleate): Training and deployment of GNN-based collective variables for nucleation simulations.

---

## 📜 Citation

If you use this repository or refer to our methods, please cite:

```bibtex
@article{DietrichSalvalaglio2025,
  title={On the Reproducibility of Free Energy Surfaces in Machine-Learned Collective Variable Spaces},
  author={Florian M. Dietrich and Matteo Salvalaglio},
  journal={ChemRxiv},
  year={2025}
}
```

---

Let me know if you'd like a `requirements.txt` stub, badges (e.g., license, DOI), or if this is going to accompany a Zenodo archive.


