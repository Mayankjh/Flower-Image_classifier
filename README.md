# Flower Image Classifier 

  Going forward, AI algorithms will be incorporated into more and more everyday applications. For example, you might want to include an image classifier in a smartphone app. To do this, you'd use a deep learning model trained on hundreds of thousands of images as part of the overall application architecture. A large part of software development in the future will be using these types of models as common parts of applications.
  
  In this project, you'll train an image classifier to recognize different species of flowers. You can imagine using something like this in a phone app that tells you the name of the flower your camera is looking at. In practice, you'd train this classifier, then export it for use in your application. We'll be using this dataset of 102 flower categories.
  
  When you've completed this project, you'll have an application that can be trained on any set of labelled images. Here your network will be learning about flowers and end up as a command line application. But, what you do with your new skills depends on your imagination and effort in building a dataset.
  
  *This is the final assesement project of the Udacity PyTorch Deep Learning Scholarship*

## Viewing the Jyputer Notebook
In order to better view and work on the jupyter Notebook I encourage you to use [nbviewer](https://nbviewer.jupyter.org/) . You can simply copy and paste the link to this website and you will be able to edit it without any problem. Alternatively you can clone the repository using 
```
git clone https://github.com/Mayankjh/Flower-Image_classifier/
```
then in the command Line type, after you have downloaded jupyter notebook type
```
jupyter notebook
```
locate the notebook and run it.

## Json file
In order for the network to print out the name of the flower a .json file is required. If you aren't familiar with json you can find information [here](https://www.json.org/). By using a .json file the data can be sorted into folders with numbers and those numbers will correspond to specific names specified in the .json file.

## Data and the json file
The data used specifically for this assignemnt are a flower database are not provided in the repository as it's larger than what github allows. Nevertheless, feel free to create your own databases and train the model on them to use with your own projects. The structure of your data should be the following:\
The data need to comprised of 3 folders, test, train and validate. Generally the proportions should be 70% training 10% validate and 20% test.\
Inside the train, test and validate folders there should be folders bearing a specific number which corresponds to a specific category, clarified in the json file. For example if we have the image a.jpj and it is a rose it could be in a path like this /test/5/a.jpg and json file would be like this {...5:"rose",...}. Make sure to include a lot of photos of your catagories (more than 10) with different angles and different lighting conditions in order for the network to generalize better.
    

## GPU
As the network makes use of a sophisticated deep convolutional neural network  the training process is impossible to be done by a common laptop. In order to train your models to your local machine you have three options

1. **Cuda** -- If you have an NVIDIA GPU then you can install CUDA from [here](https://developer.nvidia.com/cuda-downloads). With Cuda you will be able to train your model however the process will still be time consuming
2. **Cloud Services** -- There are many paid cloud services that let you train your models like [AWS](https://aws.amazon.com/fr/) or  [Google Cloud](https://cloud.google.com/)
3. **Coogle Colab** -- [Google Colab](https://colab.research.google.com/) gives you free access to a tesla K80 GPU for 12 hours at a time. Once 12 hours have ellapsed you can just reload and continue! The only limitation is that you have to upload the data to Google Drive and if the dataset is massive you may run out of space.

## Authors

* **MAYANK JHA** - *Initial work* 
* **Udacity** - *PyTorch Deep Learning Scholarship 2018-2019*

This project is licensed under the MIT License - see the [LICENSE]( https://mayankjha.mit-license.org/)
