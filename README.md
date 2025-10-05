# Predicting Student Outcomes (Open University Learning Analytics)

Deliverable 3 for the **Supervised Learning Final Project**.  
We predict student final outcomes (*Distinction, Pass, Fail, Withdrawn*) based on VLE engagement and assessment features.

---

## 📊 Key Results (5-Fold CV)
| Metric | Score |
| :-- | --: |
| Weighted F1 | **0.78** |
| Accuracy | **0.78** |
| ROC-AUC (OVR) | **0.93** |

## 🌟 Highlights
- Tuned Random Forest with class balancing outperforms linear baselines by **~+10 pts F1**.  
- Confusion mostly occurs between *Pass* and *Distinction*.  
- *Withdrawn* students are identified with high recall (~0.96).

<p align="center">
  <img src="figures/confusion_matrix.png" alt="Normalized Confusion Matrix (5-Fold CV)" width="430"/>
</p>

---

## ⚙️ Reproducibility
- Python ≥ 3.11, scikit-learn ≥ 1.3  
- Random seed fixed at 42  
- To re-run:
  ```bash
  pip install -r requirements.txt
  jupyter nbconvert --to notebook --execute final_project.ipynb --ExecutePreprocessor.timeout=0

conda env create -f environment.yml
conda activate ou-ml
jupyter notebook final_project.ipynb
