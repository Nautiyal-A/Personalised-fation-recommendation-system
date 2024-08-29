# Fashion Recommender System

This project demonstrates a Fashion Recommender System built using a ResNet50 model for feature extraction and k-Nearest Neighbors (k-NN) for recommendation. The system allows users to upload an image of a clothing item and recommends similar items based on image embeddings.

## Installation

To run this project locally, follow the steps below:

1. Clone the repository.
2. Install the required dependencies.
3. Run the Streamlit app.

### Clone the repository

bash
git clone <repo-url>
cd <repo-name>
## Project Structure
.
├── app.py                 # Main Streamlit application file
├── embeddings.pkl         # Pre-computed embeddings for the clothing images
├── filenames.pkl          # Filenames of the images corresponding to embeddings
├── uploads/               # Directory for uploaded files
└── requirements.txt       # Dependencies required to run the project
## How It Works

1. **File Upload**:  
   The user uploads an image via the file uploader widget.

2. **Feature Extraction**:  
   The uploaded image is processed by the ResNet50 model to generate a feature vector.

3. **Recommendation**:  
   The extracted feature vector is compared against pre-computed embeddings using k-NN to find the most similar items.

4. **Results Display**:  
   The recommended similar items are displayed as images.

## Future Enhancements

- **Expand the Dataset**:  
  Include more clothing categories and items to improve the recommendations.

- **UI Improvements**:  
  Create a more engaging user interface for better user interaction.

- **Model Tuning**:  
  Experiment with different models and embeddings to improve the quality of recommendations.
