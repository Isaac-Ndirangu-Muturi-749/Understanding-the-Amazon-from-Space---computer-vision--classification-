# 🌍🛰️ Planet: Understanding the Amazon from Space 🛰(computer vision)(classification)
## Use satellite data to track the human footprint in the Amazon rainforest

## Project Overview:
🌍🛰️ Planet Aerial Imagery

### Problem Statement:
Every passing minute, an expanse of forest equivalent to 48 football fields disappears from our planet. The Amazon Basin takes the lead in this alarming deforestation trend, contributing to biodiversity loss, habitat destruction, climate change, and other catastrophic effects. Precise data on deforestation and human activities in forests is crucial for swift and effective responses from governments and local stakeholders.

🛰️ Planet, the innovator behind the world’s largest fleet of Earth-imaging satellites, is set to capture daily imagery of the entire Earth's land surface at an impressive 3-5 meter resolution. While existing research focuses on monitoring forest changes, it often relies on coarse-resolution imagery from sources like Landsat (30-meter pixels) or MODIS (250-meter pixels), limiting its effectiveness in areas dominated by small-scale deforestation or forest degradation.

Moreover, current methods struggle to distinguish between human-induced and natural forest loss. Higher resolution imagery, such as that from Planet, has demonstrated exceptional capability in this regard, but robust algorithms are yet to be developed.

🌈 In this competition, Planet and its Brazilian partner SCCON invite Kagglers to colorfully label satellite image chips with atmospheric conditions and various classes of land cover/land use. The resulting algorithms will empower the global community to comprehensively understand when, where, and why deforestation occurs worldwide—and, most importantly, how to respond effectively. 🚀✨
 
![amazon](zris1779.png)

### Dataset:

The dataset consists of high-resolution satellite images of the Amazon rainforest, captured by Planet's Earth-imaging satellites. Each image is labeled with atmospheric conditions and various classes of land cover/land use. The challenge is to create robust algorithms that can distinguish between different types of forest loss, including human-induced and natural causes.

## Project Components:

1. **Data Exploration:**
   - Utilized Pandas and Matplotlib to explore and visualize the distribution of classes in the training dataset.
   - Extracted unique labels and performed one-hot encoding to prepare the data for model training.

2. **Data Preprocessing:**
   - Resized images to a consistent size (128x128) for model compatibility.
   - Implemented data augmentation techniques using TensorFlow's ImageDataGenerator.

3. **Model Development:**
   - Implemented Convolutional Neural Networks (CNNs) using TensorFlow and Keras.
   - Explored different architectures, including a custom CNN and transfer learning with ResNet50.
   - Compiled models using binary cross-entropy loss and a custom F-beta score as the evaluation metric.

4. **Model Training:**
   - Split the dataset into training and validation sets.
   - Used TensorFlow's ModelCheckpoint to save the best model based on validation performance.
   - Trained models for multiple epochs while monitoring key metrics.

5. **Prediction and Submission:**
   - Loaded the best-trained model to make predictions on the test dataset.
   - Generated a CSV file with image predictions for submission to the Kaggle competition.

6. **Results and Analysis:**
   - Analyzed model performance using training and validation metrics.
   - Reviewed the generated predictions and submission file for potential improvements.

## Project Files:

- `__notebook__.ipynb`: Jupyter Notebook containing the entire project code.
- `best_model.hdf5`: Saved model weights for the best-performing model.
- `predictions.csv`: CSV file containing image predictions for the test dataset.

## Instructions for Reproduction:

1. **Dataset:**
   - Download the dataset from the Kaggle competition: [Understanding the Amazon from Space](https://www.kaggle.com/c/planet-understanding-the-amazon-from-space).

2. **Environment:**
   - Create a Python environment with necessary dependencies using the `requirements.txt` file.

3. **Notebook Execution:**
   - Execute the notebook `__notebook__.ipynb` in a Jupyter environment, ensuring all cells are run sequentially.

4. **Submission:**
   - Submit the generated `predictions.csv` file to the Kaggle competition.

## Follow-up:

- Further optimization of model architectures and hyperparameters for improved performance.
- Exploration of ensemble methods to combine predictions from multiple models.
- Continuous monitoring of Kaggle competition leaderboard for potential advancements.

**Follow me on:**
- Twitter: [https://twitter.com/NdiranguMuturi1](https://twitter.com/NdiranguMuturi1)
- LinkedIn: [https://www.linkedin.com/in/isaac-muturi-3b6b2b237](https://www.linkedin.com/in/isaac-muturi-3b6b2b237)
- GitHub: [https://github.com/Isaac-Ndirangu-Muturi-749](https://github.com/Isaac-Ndirangu-Muturi-749)