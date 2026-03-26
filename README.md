# Task 3: Multimodal Housing Price Prediction Using Images + Tabular Data

**DevelopersHub Corporation – AI/ML Engineering Advanced Internship**  
**Submitted by:** Subhan  
**Date:** March 2026

## Objective
Build a model that predicts housing prices by combining **tabular data** (rooms, location, income, etc.) with **image features** extracted from house photos using a CNN.

## Dataset
- **Tabular**: California Housing Dataset  
- **Images**: Simulated house images (placeholder — easily replaceable with real photos)

## Approach
- Preprocessed and scaled tabular features
- Built a lightweight CNN to extract visual features from images
- Fused tabular and image features into one vector
- Trained a Random Forest Regressor on the combined features
- Evaluated using MAE, RMSE, and R² Score

## Technologies Used
- PyTorch (CNN for image feature extraction)
- scikit-learn (Random Forest, scaling, evaluation)
- pandas, numpy, matplotlib

## Results

| Metric       | Value     |
|--------------|-----------|
| MAE          | ~0.45     |
| RMSE         | ~0.65     |
| R² Score     | ~0.75     |

**Visualisation**: Actual vs Predicted prices plot included in the notebook.

## Key Insights
- Multimodal learning allows the model to consider both numerical and visual information.
- Even with simulated images, the fusion approach demonstrates the potential of combining modalities.
- In production, using real high-quality house images would significantly boost accuracy.

## Repository Contents
- `Task3_Multimodal_Housing_Prediction.ipynb`
- `multimodal_housing_price_model.joblib`
- `tabular_scaler.joblib`

## Future Improvements
- Replace fake images with real house photo dataset
- Try advanced fusion techniques (e.g., attention or late fusion)
- Deploy as a web app using Gradio/Streamlit for users to upload house images

---

Submitted as part of the Advanced AI/ML Engineering Internship at DevelopersHub Corporation.
