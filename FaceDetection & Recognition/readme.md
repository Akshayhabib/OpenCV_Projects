># FACE DETECTION AND RECOGNITION
___
___
>This project is used to  collect user face images and will train the LBPH  face classifer model then based on video feed from webcam,when there is highly confidence more than 75% it will show the message if train user is identified.
>
>--Linear Binary Phase Histogram Classifier(LBPH):This is an algorithm which will actually help us to do face recognizer.
>
> We basically have to convert all the images into arrays and give it to this algorithm, so that the algorithm get trained with repect to that specific image.


---
>>STEP 1:Create a faces folder.
> 
>
> In this folder,I will be storing 200 frames of my images and later ,I will be training it with my LBPH face recognizer which is provided by opencv and then,I will try to see whether it is able to recognize my face.
---
>>STEP 2: Create a models folder.
>
>load model,
face_classifier = cv2.CascadeClassifier('haarcascade_frontalface_default.xml')
> which will be able to capture the face feature.

>>STEP 3: Create a config.py file.
> 
>In this .py file we will have all the hard coded variabels like MODELS,DEVICE,PATH,HEIGHT,WIDTH,TOTAL_IMAGES.


>>STEP 4: Create a utils.py file.
> 
> In this .py file we have functions like face_extractor and face_detector,we will be using this for extracting and detecting faces.

>>STEP 5:Create a collect_data.py file.
> 
> In this .py file we are collecting the user data.

>>STEP 6:Create a train.py file.
> 
>In this .py file we are training our model.

>>STEP 7:Create a detect.py file.
> 
> In this .py file we will try to see whether it is able to recognize my face.