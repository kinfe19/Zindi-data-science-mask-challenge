# Spot-the-Mask-challenge-3rd-Place
## #All against the COVID-19

<div align="center">
    <img src = "https://pbs.twimg.com/media/EVyYt-IU8AALA3x.jpg" 
     height = "500"
     width = "1000">
</div>

     

## 🗒<span style='color:green'> Description </span>


In a time of concerns about slowing the transmission of COVID-19, increased surveillance combined with AI solutions can improve monitoring and reduce the human effort needed to limit the spread of this disease.

Since the anouncement of a lockdown, generalized in many counntries over the world due to the spread of COVID-19, Zindi community has started a new type of challenges called <span style='color:red'>#ZINDIWEEKENDZ </span>. It is a set of competitions based on data science in order to permit to all the #zindians the development of AI based solutions in order to use their skills for giving their community some technical means and  viable solutions to their community in this biological war.
A challenge is taking place every weekend from April to May 2020.

This hackathon was about predicting whether a person in an image is wearing a face mask or not. It was hosted by [Zindi](https://zindi.africa/hackathons/spot-the-mask-challenge/) and lasted for 3 days (from Thursday 17 April to Sunday 19).  

##  😷<span style='color:green'> The solution </span> 🧠
Our solution is based on the architechture of the well known model <a href="https://pytorch.org/hub/pytorch_vision_densenet/">Densnet</a> and uses the technique of transfer learning to get some learned features form others tasks and use them in this contest to help our custom model to make accurate predictions.

<div align="center">
    <img src = "https://pytorch.org/assets/images/densenet1.png" 
        height = "400"
        width = "800">
</div>

The main framework used to implement the model is <a href="https://pytorch.org/get-started/locally/">Pytorch</a>. Some of us also used [Tensorflow 2.0](https://www.tensorflow.org/), [keras](https://keras.io/) and [scikit-learn](https://scikit-learn.org/stable/) when experimenting.

With this model and with all the others techniques applied, we have been able to get the following results:

<div align='center'>

|set        | loss (log_loss)      | accuracy  |
|-----------|----------------------|-----------|
|training   |0.001918              | 99.242  % |
|test       |0.001099342           | 98.141 %  |

</div>


## 🌴<span style='color:green'> Repository structure (tree😎)</span>
You must follow this structure when runing the notebook.

|----Data  
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      |--- images.zip  
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      |--- train_labels.csv  
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;      |--- sample_sub_v2.csv \
| \
|----Mask Challenge Solution  
|&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;       |--- Spot_the_mask_challenge.ipynb  
|\
|---- Readme.md  
|---- environment.yml\
|---- requirements.txt  


PS : [Download dataset here](https://zindi.africa/hackathons/spot-the-mask-challenge/data) 

Use `pip install -r requirements.txt` to install all the dependencies before going deep.\
\
If you are facing any issues with installation with `pip` you can use the environment.yml file to create an anaconda environment and then use one of these command lines below to activate it (you need to have anaconda distribution and **pip version 9.0.1** installed first) : 

 ```
 # 1- create the anaconda env and install dependencies
 $ conda env create -f environment.yml
 
 # 2- activate the environment containing the dependencies (pytorch, torchvision, keras, opencv etc...)
$ source activate spot-mask-env 

# or

$ conda activate spot-mask-env

# 3- Verify that the new environment was installed correctly by running:
$ conda list

# (optional) 
$ jupyter-notebook
```

## Command lines summary

<div align="center">

 |command line                     |                Description                                                |
 |---------------------------------|---------------------------------------------------------------------------|
`pip install -r requirements.txt`  | install all the dependencies listed <br> in the file **requirements.txt** |
| `conda env create -f environment.yml`|Create new virtual environment based on the configuration file **environment.yml**|
| `source activate spot-mask-env ` <br> or <br> `conda activate spot-mask-env`| Activate the virtual env named **spot-mask-env**|
| `conda list`|List aull the packages installed into activated venv|
| `jupyter-notebook`|Launch Jupyter notebook web server|
|

</div>




## 💻<span style='color:green'> Authors </span>

<div align='center'>

| Name           |                     Zindi ID                     |                  Github ID               |
|----------------|--------------------------------------------------|------------------------------------------|
|Kinfe Masriei    |[@Kinfe😁](https://zindi.africa/users/kinfe)  |[@kinfe19](https://github.com/kinfe19)|

</div>


