# Anomaly Detection Autoencoder

This repository contains a Jupyter Notebook `anomaly_detection_autoencoder.ipynb` that demonstrates how to use an autoencoder for anomaly detection among noisy signals.

## Overview

An autoencoder is a type of artificial neural network used to learn efficient codings of unlabeled data. In the context of anomaly detection, autoencoders can be trained to reconstruct normal data patterns. Anomalies can then be detected by identifying data points with high reconstruction errors. This autoencoder is trained with unsupervised data in an attempt to locate seismic events in the provided test data.

![plot for autoencoder result](/assets/sample_1.png "Sample result plot for this autoencoder")

## Contents

- `anomaly_detection_autoencoder.ipynb`: The main notebook that includes:
  - Data preprocessing
  - Building the autoencoder model
  - Training the model
  - Evaluating the model
  - Detecting anomalies

## Requirements

To run the notebook, install the packages mentioned in the `requirements.txt` file

## Usage

We used [Google Colab](https://colab.research.google.com/) for training and testing this model and we also recommend using this tool.

Whether you use Google Colab or a local Jupyter instance, you need to make sure the following directories and files exist and contain the test and training files respectively or update the notebook's paths according to your configuration:

1. `output/` - will contain the output catalog after testing
2. `test_data/` - contains the test data set
3. `training/` - contains the training data set
4. `apollo12_catalog_GradeA_final.csv` - contains the training catalog

## License

This project is licensed under the MIT No Attribution License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [TensorFlow](https://www.tensorflow.org/api_docs/python/tf/keras/), [Keras](https://keras.io/api/) and [obspy](https://docs.obspy.org/) documentation
- [ChatGPT](https://chat.openai.com/) for evaluating the viability of our solution and clarifying what parameters would contribute to better performance.
- [NASA SpaceApps Challenge](https://www.spaceappschallenge.org/nasa-space-apps-2024/challenges/seismic-detection-across-the-solar-system/?tab=details) for providing challenge details, training and test data.
- [Google Colab](https://colab.research.google.com/) for running our python notebook.

Feel free to contribute to this project by opening issues or submitting pull requests.
