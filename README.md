# Brian 2 version source code for paper "Unsupervised Learning of Digit recognition using STDP"

This small project is to translate Brian 1 code from Paper "Unsupervised learning of digit recognition using spike-timing-dependent plasticity" written by PU Diehl to Brian 2 version.

The repository is further updated to be compatible with Python 3.10.16. Integrations with [Brian2CUDA](https://brian2cuda.readthedocs.io/en/latest/introduction/index.html) is under progress.

## Prerequisite

1. Python environment specified through [Brian2-STDP-MNIST_conda.yml](https://github.com/briansebzhou/Brian2STDPMNIST/blob/3aad7fc1218c8e5c51b2ba46ca83932a1e9a8f52/Brian2-STDP-MNIST_conda.yml)
2. MNIST datasets, which can be downloaded from [MNIST Dataset](https://www.kaggle.com/datasets/hojjatk/mnist-dataset?select=train-labels.idx1-ubyte)
   * The data set includes four gz files. Extract them after you downloaded them.

## Testing with pretrained weights:

1. Run the main file "Diehl&Cook_spiking_MNIST_Brian2.py". It might take hours depending on your computer
2. After the previous step is finished, evaluate it by running "Diehl&Cook_MNIST_evaluation.py".

## Training a new network:

1. modify the main file "Diehl&Cook_spiking_MNIST_Brian2.py" by changing line 214 to "test_mode=False" and run the code.
2. The trained weights will be stored in the folder "weights", which can be used to test the performance.
3. In order to test your training, change line 214 back to "test_mode=True".
4. Run the "Diehl&Cook_spiking_MNIST_Brian2.py" code to get the results.
