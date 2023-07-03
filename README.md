# Human Activity Recognition

This repository contains a project for Human Activity Recognition using two different models: CNN+LSTM and LRCN (Long-term Recurrent Convolutional Networks) with Time Distributed LSTM. The goal of this project is to detect and identify human activities performed in videos. The project is implemented using TensorFlow and the UCF50 dataset.

## Dataset
The UCF50 dataset is used for this project. It consists of videos of 50 different human activities, such as running, swimming, playing basketball, etc. Each video is labeled with the corresponding activity performed in it. The dataset provides a diverse set of examples for training and evaluation of the models.

## Workflow
The project workflow can be summarized as follows:

1. Data Exploration: The UCF50 dataset is explored to understand its structure, video formats, and the distribution of activities. This step helps in gaining insights into the dataset and facilitates further preprocessing and model development.

2. Image Preprocessing: The videos are decomposed into individual frames, and each frame is preprocessed. This may involve resizing, normalization, or any other necessary transformations to prepare the images for input to the models.

3. Video Preprocessing: The preprocessed frames are used to construct video sequences. This step involves selecting a suitable sequence length, stacking frames together, and applying necessary transformations to create input data for the models.

4. Model Development: Two models are developed for human activity recognition: CNN+LSTM and LRCN with Time Distributed LSTM. The CNN layers capture spatial features from the input frames, while the LSTM layers capture temporal dependencies across the video sequences. The models are designed and implemented using TensorFlow.

5. Training: The models are trained on the UCF50 dataset using a suitable optimization algorithm (e.g., Adam) and a defined loss function (e.g., categorical cross-entropy). During training, the models learn to recognize and classify human activities based on the provided labeled examples.

6. Evaluation: The trained models' performance is evaluated on a separate validation set or using cross-validation techniques. Metrics such as accuracy, precision, recall, and F1 score are used to assess the models' ability to correctly identify human activities in videos.

7. Model Comparison: The performance of both the CNN+LSTM and LRCN models is compared. Metrics such as accuracy, inference time, and complexity are used to evaluate and compare the models. This comparison helps determine which model is more effective and efficient for human activity recognition.

## Usage
To run the Human Activity Recognition models, follow these steps:

1. Set up the environment by installing the necessary dependencies listed in the `Environment.txt` file.

2. Download or clone the repository to your local machine.

3. Obtain the UCF50 dataset from the official source and preprocess it if necessary to ensure it is in a suitable format for training and evaluation.

4. Open the provided Jupyter Notebook file that contains the step-by-step implementation of the Human Activity Recognition models using CNN+LSTM and LRCN with Time Distributed LSTM.

5. Follow the instructions in the notebook to explore the dataset, preprocess the images and videos, develop the models, train them, evaluate their performance, and compare the models.

6. The notebook includes code snippets and explanations for each step to facilitate understanding and execution. Make sure to run each cell sequentially to ensure correct execution.

## Results
After training and evaluation, the performance of the CNN+LSTM and LRCN models is assessed on the validation set. Metrics such as accuracy, precision, recall, and F1 score are reported, providing insights into the models' ability to recognize and classify human activities in videos.

Additionally, the models are compared based on metrics like accuracy, inference time, and complexity. This helps in determining the model that is more efficient

 and effective for human activity recognition.

## Dataset Source
The UCF50 dataset used in this project can be obtained from the official source [UCF50](https://www.crcv.ucf.edu/data/UCF50.php).

## License
The code in this repository is licensed under the [MIT License](LICENSE).

## Acknowledgments
- The creators of the UCF50 dataset for providing the labeled video data of human activities.
- The TensorFlow community for developing and maintaining the TensorFlow framework.
