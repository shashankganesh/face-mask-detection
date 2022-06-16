# face-mask-detection
face mask detection using machine learning 

ABSTRACT

The COVID-19 pandemic is causing a worldwide emergency in healthcare. This virus mainly spreads through droplets which emerge from a person infected with coronavirus and poses a risk to others. The risk of transmission is highest in public places. One of the best ways to stay safe from getting infected is wearing a face mask in open territories as indicated by the World Health Organization (WHO). In this project, we propose a method which employs OpenCV to detect face masks on people. A bounding box drawn over the face of the person describes weather the person is wearing a mask or not. It also shows the warning to wear mask covering nose and mouth if the person is not covering his  nose or mouth.


CONTENTS

1	
Introduction	

2
Literature Survey

3	
Methodology	

4	
Software Requirements Specifications	

5	
System Design	

6	
Testing	

7	
Conclusion 	

	References	
	
	

                             1.INTRODUCTION


COVID-19 had a massive impact on human lives. The pandemic lead to the loss of millions and affected the lives of billions of people. According to WHO(World Health Organization), 55.6 million people were infected with Coronavirus and 1.34 million people died because of it as of November 2020. After the person gets infected, it takes almost fourteen days for the virus to grow in the body of its host and affect them and in the meantime, it spreads to almost everyone who is in contact with that person. So, it is extremely hard to keep the track of the spread of COVID-19.
COVID-19 mainly spreads through droplets produced as a result of coughing or sneezing by an infected person. This transfers the virus to any person who is in direct close contact (within one-meter distance) with the person suffering from coronavirus. Because of this, the virus spreads rapidly among the masses. Face masks are an effective method to control the spread of virus. It had been found that wearing face masks is 96% effective to stop the spread of virus. The governments, all over the world, have imposed strict rules the everyone should wear masks while they go out. But still, some people may not wear masks and it is hard to check weather everyone is wearing mask or not. In such cases, computer vision will be of great help.
There are no efficient face mask detection applications to detect wheather the person is wearing face mask or not. This increases the demand for an efficient system for detecting face masks on people for transportation means, densely populated areas, residential districts, large-scale manufacturers and other enterprises to ensure safety. This project uses machine learning classification using OpenCV  to detect facemasks on people.

          2.LITERATURE SURVEY

The COVID-19 is an unparalleled crisis leading to huge number of casualties and security problems. In order to reduce the spread of coronavirus, people often wear masks to protect themselves. This makes the face recognition a very difficult task since certain parts of the face are hidden. A primary focus of researchers during the ongoing coronavirus pandemic is to come up with suggestions to handle this problem through rapid and efficient solutions.
The proposed system focuses on how to identify the person on video stream wearing face mask with the help of computer vision using the OpenCV.
Approach – 1.Train the model
Approach - 2.Apply mask detector over live video stream. The majority of the images were augmented by OpenCV. The set of images were already labelled “mask” and “no mask”. The images that were present were of different sizes and resolutions, probably extracted from different sources or from machines (cameras) of different resolutions.
Face detection is defined as the procedure that has many applications like face tracking, pose estimation or compression. Face detection is a two-class problem where we have to decide if there is a face or not in a picture. This approach can be seen as a simplified face recognition problem.Haar-like wavelets are binary rectangular representations of 2D waves. A common visual representation is by black (for value minus one) and white (for value plus one) rectangles. The square above the 0-1- interval shows the corresponding Haar-like wavelet in common black-white representation. The rectangular masks used for visual object detection are rectangles tessellated by black and white smaller rectangles. Those masks are designed in correlation to visual recognition tasks to be solved, and known as Haar like feature each call, a distribution of weights is updated that indicates the importance of examples in the data set for the classification. On each round, the weights of each incorrectly classified example are increased, and the weights of each correctly classified example are decreased, so the new classifier focuses on the examples which have so far eluded correct classification.The system requires the dataset for the training and testing purpose. So, the dataset is collected real-time using system’s camera. The dataset contains the images of faces with and without mask.

3.METHODOLOGY

Image Collection:
The first step of the proposed system is to collect data. This  system,  uses web camera to shoot the faces. The data collection uses viola jones algorithm to detect the features of human face.
Labelling The Image:
Data labelling is a critical step in developing a high-performance ML model. Labelling is part of the pre-processing stage when developing a Machine Learning (ML) model. It requires the identification of raw data (i.e., images, text files, videos), and then the addition of one or more labels to that data to specify its context for the models, allowing the machine learning model to make accurate predictions.
Training:
In this phase, the model is trained using training data and expected output for this data. Progress is visible on the console when the script runs. At the end it will report the final accuracy of the model.
Detect the face mask:
Now System will have to detect whether the person is wearing a face mask or not.



.

	4.SOFTWARE REQUIREMENTS SPECIFICATIONS
1.1.HARDWARE REQUIREMENTS

    Camera : Good  qualty,3MP
RAM : Minimum 8GB RAM
GPU: 4GB dedicated
Processor: Intel Pentium 4 or higher

1.2.SOFTWARE REQUIREMENTS
Anaconda:
Anaconda is an open-source distribution for python and R. It is used for data science, machine learning, deep learning, etc. With the availability of more than 300 libraries for data science, it becomes fairly optimal for any programmer to work on anaconda for data science.

Visual Studio:
The Visual Studio IDE (integrated development environment) is a software program for developers to write and edit their code. Its user interface is used for software development to edit, debug and build code. Visual Studio includes a code editor supporting IntelliSense (the code completion component) as well as code refactoring. The integrated debugger works both as a source-level debugger and a machine-level debugger.

5.SYSTEM DESIGN

5.1 MODULE DESCRIPTION







6.TESTING

The testing is the final step in the system.in this stage the system performs the classification on the inputted data. The system captures face from the web cam and performs classification on it, the system predicts the faces and decides whether the face is with mask or not according to the trained dataset.
This system detects the eyes on the face and the bounding box appears on the eyes.
The model detects the face and eyes in the live image with the bounding boxes appearing over the faces with respective labels.
The live webcam images are equipped with the bounding boxes on them, the system is observed to perform well with the accuracy and prediction on the number of the data trained.

ID	TEST CASE	INPUT DESCRIPTION	EXPECTED OUTPUT	TEST STATUS
1	Loading Model	Initializing trained	model and load it to the system	Loaded	model without errors	Pass
2	Converting Video to frames	Capturing video and converting it into frames	Image frames of captured video stream	Pass
3	Recognize 
Facemask	Image frame that contains dataset with mask and without mask	label	Pass
	Verification Of Test Cases



7.CONCLUSION

With the increasing number of COVID cases all over the world, a system to replace humans to check masks on the faces of people is greatly needed. This system satisfies that need. This system can be employed in public places like railway stations and malls. It will be of a great help in companies and huge establishments where there will be a lot of workers. This system will be of a great help there because it is easy to obtain and store the data of the employees working in that Company .


REFERENCES
[1] M. S. Ejaz, M. R. Islam, M. Sifatullah and A. Sarker, "Implementation of Principal Component Analysis on Masked and Non-masked Face Recognition," 2019 1st International Conference on Advances in Science, Engineering and Robotics Technology (ICASERT), Dhaka, Bangladesh,2019.
[2] BOSHENG QIN, DONGXIAO LI. Identifying Facemask-wearing Condition Using Image SuperResolution with Classification Network to Prevent COVID19, 13 May 2020, PREPRINT (Version 1) available at Research Square [+https://doi.org/10.21203/rs.3.rs- 28668/v1+].
