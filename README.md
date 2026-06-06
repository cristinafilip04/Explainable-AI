Explainable Final Assignment:Robustness of SHAP and Anchor Explanations in Heart Disease Prediction
Course: Explainable AI (SOW-BKI266), Radboud University
Author: Cristina-Maria Filip (s1111439)
Overview
This project evaluates how robust SHAP and Anchor explanations are when small input perturbations (simulating measurement noise) are applied to a heart disease prediction model. The experiment quantifies explanation consistency across increasing noise levels using:

SHAP: Top-k feature overlap metric
Anchors: Jaccard rule stability metric

Requirements
Python 3.8+ is recommended. Install all dependencies with:
bashpip install pandas numpy matplotlib scikit-learn shap anchor-exp
How to Run

Clone or download this repository
Place heart.csv in the same directory as the notebook
Launch Jupyter:

bashjupyter notebook final_assignment.ipynb

Run all cells from top to bottom (Kernel > Restart & Run All)


Note: The robustness experiment (Section 5) runs Anchor explanations for 30 instances × 4 noise levels. This takes approximately 20 minutes. You can reduce N_INSTANCES at the top of that cell to speed things up.

References

Lundberg, S. M., & Lee, S.-I. (2017). A unified approach to interpreting model predictions. Advances in Neural Information Processing Systems, 30, 4765–4774.
Ribeiro, M. T., Singh, S., & Guestrin, C. (2018). Anchors: High-precision model-agnostic explanations. Proceedings of the AAAI Conference on Artificial Intelligence, 32(1).
Alvarez-Melis, D., & Jaakkola, T. S. (2018). On the robustness of interpretability methods. ICML Workshop on Human Interpretability in Machine Learning (WHI 2018).
Janosi, A., Steinbrunn, W., Pfisterer, M., & Detrano, R. (1989). Heart Disease [Dataset]. UCI Machine Learning Repository.
