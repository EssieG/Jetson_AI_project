# Jetson_AI_project
This is my Jetson AI Certificate project, which classifies my movements for a mobile robot as walking, running, or standing.

Classifying the type of movement a human is using and what direction they are going could be a useful tool for a mobile robot. Knowing the trajectory allows the robot to consider if it will collide with the human, and knowing the movement allows the robot to gauge the human's speed.

The dataset in the data/ folder consists of a sample of my training data of me performing three movements - walking, running, and standing in the library. For a more robust model, many more training images could be included, using different humans, backgrounds, lighting, etc. The labels are discrete, so the code utilizes pytorch for classification. A robust datset that included the speeds of the humans pictured could be used in a regression-type model to predict the speed the human is walking or running.

Inside the data folder are the categories for classfication, as well as a validation set of images. The validation images include 5 from each category, for a total of 25 images. The model succeeds on 23/25 of the validation images for the default model run with 5 epochs. Training images ~165 per category.

The main Jupyter notebook explains the steps for training and validation clearly. For an overview, see the video: https://youtu.be/4a3jqjonGAM.

File structure: <br/> 
code
<ul> 
     <li>main.py <br/> </li>
     <li>utils.py <br/> </li>
     <li>dataset.py <br/> </li>
</ul>
wander_A 
<ul>
       <li>walking_L  <br/> </li> 
       <li>walking_R <br/> </li>
       <li>running_L <br/> </li>
       <li>running_R <br/> </li>
       <li>standing <br/> </li>
       <li>validation <br/> </li>
</ul>
motion_model.pth 

