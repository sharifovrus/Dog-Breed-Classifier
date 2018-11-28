# Dog-Breed-Classifier
The algorithm can identify a dog, human and not a dog or human.


## Instructions
This is a Convolutional Neural Networks (CNN) project.

Clone the repository and navigate to the downloaded folder.

    git clone https://github.com/udacity/dog-project.git
    cd dog-project

Download the [Dog Dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip/). 
Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`.

Download the [Human Dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip/).
Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.

Donwload the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz/) for the dog dataset. 
Place it in the repo, at location `path/to/dog-project/bottleneck_features`.


Create environment
```
    conda env create -f requirements/dog-windows.yml
    activate dog-project
    set KERAS_BACKEND=tensorflow
    python -c "from keras import backend"
```

Open the notebook:
```
    jupyter notebook dog_app.ipynb
```
Notebook consist of the following steps:

    Step 0: Import Datasets
    Step 1: Detect Humans
    Step 2: Detect Dogs
    Step 3: Create a CNN to Classify Dog Breeds (from Scratch)
    Step 4: Use a CNN to Classify Dog Breeds (using Transfer Learning)
    Step 5: Create a CNN to Classify Dog Breeds (using Transfer Learning)
    Step 6: Write your Algorithm
    Step 7: Test Your Algorithm
    
    
 ## Refinement
 
 The algorithm can identify dog, human and not a dog or human but there are following Points of Improvement: 
 - get more data (recognize more variety of dog breeds); 
 - change batches and epochs (some network architectures are more sensitive than others to batch size); 
 - combine different models (ensemble method e.g. bagging - the same algorithm has different perspectives on the problem by being trained on different subsets of the training data, boosting - different algorithms are trained on the same training data). 
