# Multi-Label-Classification-using-Keras
Program Description: Implement a Keras CNN SmallerVGGNet model to run multi-label classification on a custom dataset. The dataset includes six main labels: black jeans, blue dress, blue jeans, blue shirt, red dress, and red shirt.
Multi-label classification with Keras
├── classify.py
├── dataset
│   ├── black_jeans [344 entries]
│   ├── blue_dress [386 entries]
│   ├── blue_jeans [356 entries]
│   ├── blue_shirt [369 entries]
│   ├── red_dress [380 entries]
│   └── red_shirt [332 entries]
├── examples
│   ├── example_01.jpg
│   ├── example_02.jpg
│   ├── example_03.jpg
│   ├── example_04.jpg
│   ├── example_05.jpg
│   ├── example_06.jpg
│   └── example_07.jpg
├── fashion.model
├── mlb.pickle
├── plot.png
├── pyimagesearch
│   ├── __init__.py
│   └── smallervggnet.py
├── search_bing_api.py
└── train.py
- `search_bing_api.py`: This script allows the construction of an image dataset for the deep learning project. We include this file to ensure the completeness of the documentation.

- `train.py`: Once we have the data, we use the `train.py` file to train our classifier.

- `fashion.model`: The `train.py` file serializes our Keras model to disk. We will use this model later in the `classify.py` file.

- `mlb.pickle`: A pickled file of the MultiLabelBinarizer from scikit-learn created by the `train.py` file. This file contains the names of our classes in a conveniently serialized data structure.

- `plot.png`: The training script generates an image file `plot.png` containing information about accuracy/loss and potential overfitting.

- `classify.py`: This file contains the source code to test the multi-label classification.

- `dataset`: This directory contains our image dataset. Each class has its own subdirectory. We do this to (1) keep our dataset organized and (2) make it easy to extract class labels from a specific image path.

- `pyimagesearch`: This is our module containing a Keras neural network. Because this is a module, it includes a correctly formatted `__init__.py` file. Another file, `smallervggnet.py`, contains the code to assemble the neural network.

- `examples`: Seven example images are present in this directory. We will use `classify.py` to perform multi-label classification with Keras on each example image.
