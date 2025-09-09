# Star Classification Using Machine Learning

This project classifies stars as **Dwarf** or **Giant** using physical features like apparent magnitude, absolute magnitude, parallax, color index, and spectral type. Various machine learning models were applied and compared.  

---

## Dataset

Features include:  
- `Vmag` : Apparent magnitude  
- `Amag` : Absolute magnitude  
- `Plx` : Parallax  
- `e_Plx` : Parallax error  
- `B-V` : Color index  
- `SpType` : Spectral type  
- `TargetClass` : 0 = Dwarf, 1 = Giant  

---

## Preprocessing

- Outliers removed using 90th percentile thresholds  
- Categorical feature `SpType` label-encoded  
- Split into train (75%) and test (25%) sets  

---

## Models Used

- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Decision Tree  
- Random Forest  
- AdaBoost  
- Voting Classifier (LR + KNN + RF)  

---

## Results

| Model               | Accuracy |
|--------------------|----------|
| Logistic Regression | 0.8916   |
| KNN                 | 0.9103   |
| Decision Tree       | 0.8972   |
| Random Forest       | 0.9308   |
| Voting Classifier   | 0.9234   |

**Random Forest** performed best with ~93% accuracy.  

---

## Visualization

- Scatter plots show relationships between magnitudes, parallax, and star classes  
- KDE plots compare distributions of Dwarf vs Giant stars  

---

## Conclusion

The project demonstrates a full ML pipeline: data cleaning, preprocessing, visualization, model training, and evaluation. Random Forest and Voting Classifier are the most effective models for this dataset.

