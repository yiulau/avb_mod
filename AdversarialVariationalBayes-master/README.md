# Adversarial Variational Bayes
This repository contains the code to reproduce the core results from the paper [Adversarial Variational Bayes: Unifying Variational Autoencoders and Generative Adversarial Networks](https://arxiv.org/abs/1701.04722).

To cite this work, please use
```
@INPROCEEDINGS{Mescheder2017ICML,
  author = {Lars Mescheder and Sebastian Nowozin and Andreas Geiger},
  title = {Adversarial Variational Bayes: Unifying Variational Autoencoders and Generative Adversarial Networks},
  booktitle = {International Conference on Machine Learning (ICML)},
  year = {2017}
}
```

# Dependencies
This project uses Python 3.5.2. Before running the code, you have to install
* [Tensorflow 1.0](https://www.tensorflow.org/)
* [Numpy](http://www.numpy.org/)
* [Scipy](https://www.scipy.org/)
* [Matplotlib](http://matplotlib.org/)
* [tqdm](https://pypi.python.org/pypi/tqdm)
* [ite-toolbox](https://bitbucket.org/szzoli/ite-in-python/)

The former 5 dependencies can be installed using pip by running
```
pip install tensorflow-gpu numpy scipy matplotlib tqdm
```

# Usage
Scripts to start the experiments can be found in the `experiments` folder. If you have questions, please
open an issue or write an email to lmescheder@tuebingen.mpg.de.

## MNIST
To run the experiments for mnist, you first need to create tfrecords files for MNIST:
```
cd tools
python download_mnist.py
```
Example scripts to run the scripts can be found in the `experiments` folder.

Samples:

![MNIST samples](img/mnist_samples.png)

## CelebA
To run the experiments on celebA, first download the dataset from [here](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) and put all the images in the `datasets/celebA` folder.

Samples:

![celebA samples](img/celebA_samples.png)

Interpolations:

![celebA interpolations](img/celebA_interp.png)
