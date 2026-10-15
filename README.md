# Ovarian_Cancer_Biomarkers
Identifying biomarkers using NGS and SVM
cat << 'EOF' > README.md
# Ovarian Cancer Biomarkers & Machine Learning Discovery

An advanced bioinformatics framework for identifying molecular biomarkers, classifying tumor grades, and performing multi-modal predictive analysis in ovarian cancer using genomic signatures and clinical parameters.

## Research Objectives
- **Biomarker Identification:** Discovering high-confidence candidate genes (e.g., `Gene_15`, `Gene_45`, `Gene_102`) associated with ovarian serous carcinoma.
- **Multi-Modal Integration:** Combining high-dimensional gene expression profiles with clinical indicators (Patient Age and key symptoms like persistent bloating and pelvic pain).
- **Machine Learning Classification:** Implementing robust ensemble classifiers (Gradient Boosting, Random Forest) validated via Stratified K-Fold Cross-Validation.

## Methodology & Pipeline
1. **Data Preprocessing & Simulation:** Generating robust transcriptomic datasets alongside clinical feature matrices.
2. **Feature Selection:** Utilizing statistical scoring (`SelectKBest` with ANOVA F-value) to filter top-performing genomic markers.
3. **Model Training & Validation:** Training multi-class models to predict tumor grades (Grade 1, Grade 2, Grade 3) with rigorous performance tracking (Precision, Recall, F1-Score).
4. **Interactive Deployment:** Providing a web-based clinical decision support interface via Streamlit.

## Project Structure
```text
├── app.py                          # Interactive Streamlit Web Application
├── advanced_train_symptoms.py      # Core machine learning & biomarker training script
├── advanced_ovarian_model.pkl      # Serialized predictive model
├── advanced_ovarian_selector.pkl   # Serialized feature selector
├── ovarian_grade_confusion_matrix.png # Multi-class evaluation confusion matrix
├── feature_importance.png          # Top biomarker gene ranking visualization
└── class_performance.png           # Performance metrics per tumor grade
