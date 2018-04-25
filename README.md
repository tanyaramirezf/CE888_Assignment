# CE888 Data Science and Decision Making
# Final project
# Evolutionary Strategies for Domain Adaptation

## Relevant information for the project

The information that can be found here is:

* Instructions to download the data sets required. The data set are:
	* MNIST-M Data set
	* Office 31 Dataset
* Python code per data set with the implementation of the proposed model.
* Writting report with the findings, methodology and background of the project.

### Objetive

It is often the case that the distribution of the source data is not the same as the target data; for example we only have labeled data examples from images of animals we took in artificial captivity conditions (source data), but we would like to classify animals in the wild (target data). We don't know the labels of the target data, so we have to learn features that fail to discriminate between source and target distributions, but are good enough to actually learn the mapping between those distributions and their labels.

### Tasks
1. Download and load the above datasets in python, clearly separating the domain and source data - write down what you observe.
2. Create a neural network that takes as input the data provided and outputs a set of features - use RELU units.
3. Use the outputs of the random neural network to train a Random Forest.
4. Start an evolutionary process using SNES, adapting the weights of the neural network. The score of your classifier should take into account domain adaptation; a good classifier both succeeds in achieving good performance for the source domain, while the features learned fail to discriminate between source and target domains. The score that you give back to SNES should should thus be a weighted sum between how bad a random forest fails to discriminate between source and target, while at the same time how well it does to discriminate between the different classes.
5. Plot the loss you get at each generation and evaluate your method in both datasets.

### Data
* It is worth to mention that given that the size of the files are too large, the images to be blended to the MNIST set should be downloaded from [here](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/resources.html#bsds500)

* In relation to the Office-31 set, please download the set from this [website](https://pan.baidu.com/s/1o8igXT4#list/path=%2Fresearch%2Fdataset%2Ftransfer_learning_datasets%2Foffice31%2Foffice31_raw_image&parentPath=%2Fresearch%2Fdataset%2Ftransfer_learning_datasets%2Foffice31)

