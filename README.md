# ECGR6119_Midterm University of North Carolina Charlotte
Submission for the midterm of the ECGR 6119: Application of AI class
Kevin Madden 11/9/22


Description:
Use the Mask-RCNN based model, Detectron2, in order to run object detection and
instance segmentation on a webcam stream. 

Requirements: 
    Installing Detectron • CUDA 8 and above • cuDNN 6 and above • OpenCV 3.4 

Datasets which can be used:
    COCO COCO minival PASCAL VOC 2007 Kavsir

Basic Steps:
    This assignment was completed using Google Colab so the integration with the OpenCV
    library was implemented in a different way than it would using a local IDE like Jupyter
    Notebook or Visual Studio Code. In order to access the video stream and use this as 
    input into the pre-trained detectron models, I referenced some external resources that
    utilize certain javascript code to achieve the same effect. 
    
Link to Google Colab Webcam Resource: 
    https://colab.research.google.com/drive/1QnC7lV7oVFk5OZCm75fqbLAfD9qBy9bw?usp=sharing#scrollTo=1nkSnkbkk4cC
    
Basic example Detectron2 Google Colab
https://colab.research.google.com/drive/16jcaJoc6bCFAQ96jDe2HwtXj7BMD_-m5
    
To achieve the goal of running detectron2 on webcam images I basically used the starter
code on the detectron2 github and combined this with the Google Colab webcam code. The webcam 
code uses four functions. The headers are posted down below. 
    
![alt text](https://github.com/kmadden9/ECGR6119_Midterm/blob/main/Code%20Snippets/WebcamFunc1.JPG?raw=true)
![alt text](https://github.com/kmadden9/ECGR6119_Midterm/blob/main/Code%20Snippets/WebcamFunc2.JPG?raw=true)
![alt text](https://github.com/kmadden9/ECGR6119_Midterm/blob/main/Code%20Snippets/WebcamFunc3.JPG?raw=true)
![alt text](https://github.com/kmadden9/ECGR6119_Midterm/blob/main/Code%20Snippets/WebcamFunc4.JPG?raw=true)
    
Then within the main while loop these functions are referenced while also running the standard
detectron functions in their example code. If you are not using Google Colab it is possible to 
simply run the demo while using "--webcam" as your input. With Google Colab there does not 
seem to be as simple of a solution. See some example results below.

![alt text](https://github.com/kmadden9/ECGR6119_Midterm/blob/main/Code%20Snippets/InstanceSegmentation.png?raw=true)
![alt text](https://github.com/kmadden9/ECGR6119_Midterm/blob/main/Code%20Snippets/KevNigelCrouch.jpg?raw=true)
![alt text](https://github.com/kmadden9/ECGR6119_Midterm/blob/main/Code%20Snippets/KevNigelStand.jpg?raw=true)

Link to detectron2 github:
https://github.com/facebookresearch/detectron2
