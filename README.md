# PRODIGY_ML_04
Develop a hand gesture recognition model that can accurately identify and classify different hand gestures from image or video data, enabling intuitive human-computer interaction and gesture-based control systems.

# Hand Gesture Recognition

## Overview
This project aims to develop a hand gesture recognition model that can accurately classify different hand gestures from images, enabling intuitive human-computer interaction. The model is trained to recognize gestures representing the letters A-Z, space, and nothing.

## Dataset
The dataset used for this project is the [ASL Alphabet](https://www.kaggle.com/datasets/grassknoted/asl-alphabet) from Kaggle. It consists of images representing the American Sign Language (ASL) letters, as well as additional classes for space and nothing. 

### Dataset Structure
The dataset is organized as follows:
- **Train/**: Contains 28 images of gestures for A-Z, Space, and Nothing.
- **Test/**: Contains images to evaluate the model's performance.

## Technologies Used
- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- OpenCV

## Installation
1. Clone the repository:
   git clone https://github.com/kusumithasajja/PRODIGY_ML_04.git
3. Change to the project directory:
   cd PRODIGY_ML_04
4. Install the required packages:
   pip install -r requirements.txt
## Usage
1. Prepare your images in the `Train/` and `Test/` folders.
2. Run the script:
   python Hand_Gesture.py
3. The predictions for the test images will be saved in `submission.csv`.

## Model Training
The model uses MobileNetV2 for transfer learning, with data augmentation applied to the training dataset. The training is performed using sparse categorical cross-entropy loss and Adam optimizer.

## Output
The final output of the model includes predictions for each test image, which are stored in `submission.csv` in the format:
filename,label
image1.png,A
image2.png,B
...

## Contribution
Feel free to fork the repository and submit a pull request if you'd like to contribute to the project!

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- [Kaggle ASL Alphabet Dataset](https://www.kaggle.com/datasets/grassknoted/asl-alphabet) for providing the dataset used in this project.
