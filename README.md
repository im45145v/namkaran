#NAMKARAN

THE PROBLEM:
Development isn’t a fraction but a benefit of the whole. The life of a visually impaired person is in no way easy. The inability to be aware of one’s surroundings and recognize objects plays a huge impact on the quality of life one leads. It takes more time for them to understand the things in front of them. The absence of basic object recognition in a person’s life compromises their safety. For a blind person, it is difficult and takes time to recognize and understand things. They are even 
taken advantage of for their disability. Making a fellow human's life easier is a way of upholding humanity in society. For a blind person, it is difficult and takes time to recognize and understand things. They are even taken advantage of for their disability. Making a fellow human's life easier is a way of upholding humanity in society.

THE TEAM APPROACH TO SOLVING THE PROBLEM:
To create an affordable and minimalistic gadget that will scan for objects in real-time using a camera of the device and offer voice instruction to the user via device speaker. It is capable of detecting objects within a certain pre-established range and is reliable for ensuring the safety of the user. Thus, we provide a secure and compact way for the visually impaired which is not only cost-effective but also helps them recognize certain objects without physically touching them.

INTRODUCTION
Millions of people in this world with incapacities rely on others for help. Visually impaired people face a lot of difficulties in their life. They develop many alternatives to deal with it. But even though they suffer. We are trying to transform the visual world into the audio world with the potential to inform blind people about the objects in front of them. In this project, we want to explore the possibility of using the hearing sense to understand visual objects. A system where speech commands are accepted from the user to the people who are visually impaired. This will help the visually impaired person manage day-to-day activities and to navigate their surroundings. It is used in making their life easier.

LITERATURE SURVEY
Much research has been done to ensure the safety of visually impaired people. Their life is no way easy. The inability to be aware of one's surroundings and recognize objects plays a huge impact on the quality of life one leads. Vision is one of the essential human senses. A gadget is created to scan objects in real-time. There is a camera module that captures the image and then the image gets processed. Using the speaker module the result is produced. This detection occurs only in a pre-established range.

SOFTWARE REQUIRED:
1. VISUAL STUDIO CODE / PYCHAR / JUPYTER NOTEBOOK
2. INSTALL PACKAGES OpenCV, pyttsx3 through 
              pip install opencv-python
              pip install pyttsx
              #For python3:
              pip3 install opencv-python
              pip3 install pyttsx                     
3. SSD Mobilenet (SSD stands for Single shot Detection. It has developed by Storage TEK. It is a dictator which is used for detecting objects in a picture clicked or taken. As the name itself means we take a single pic and detect multiple objects within that image. SSD is much faster when compared to the two-shot Regional Proposal Network (RPN). In RPNwe use, two shots where one is for generating region proposals and the other is for detecting objects. The whole process runs at 7 frames per second)

WORKING

Basic idea:
The idea is to create a device that detects the objects and gives audio output in real-time. The following procedure that happens in the running loop of detecting objects is as follows:

Step 1: Taking the video input
When the program is compiled and run then the video is taken as input using the Video capture function in the open CV package and running frames are captured by setting the Frame width, height, and buffer size.

Step 2: Detecting the objects
In this project, a pre-trained object detection model- “ssd_mobilenet_v3_large”, trained on the coco dataset is used. The weights that are used are “frozen _inference graph. PB”. A class name list is created which contains a class file consisting of the coco names. SSD mobile net model is taken as the configuration path and the frozen graph is taken as the weight's path. Using the open CV detection model function with weight path and configuration path as parameters object detection in the running frames is done. When an object is detected successfully, it compares which is the suitable match for the detected object in the trained dataset and matches if the percentage is above 60% or the coco name that has the highest match percentage.

Step 3: Giving audio output
After the object is determined, the name of the object is taken from the class name list and is appended as text. This appended text is then converted into an audio format using the system Os python package and audio output is given using the device(laptop/computer) speaker.


EXECUTION/OUTPUT

1. GO TO THE GITHUB REPO https://github.com/kinshukgoel4/NAMKARAN AND CLONE THE REPO OR DOWNLOAD THE ZIP
2. OPEN THE FOLDER IN YOUR IDE AND RUN THE MAIN.PY FILE
3. MAKE SURE THAT YOU INSTALL THE PACKAGES OPENCV, PYTTSX3


CONCLUSION
Vision is one of the most important senses that help people interact with the real world. There are nearly 200 million blind people all over the world, and being visually impaired hinders a lot of day-to-day activities. Thus it is very necessary for blind people to understand their surroundings, and to know what objects they interact with. So, this is a bot that provides a visual substitution for visually impaired people.\


FUTURE ENHANCEMENT
Technology is never constant. With the updating technology along with modified software and hardware, our device can be made to work in an expedited manner. We need to determine the object’s range from the person.


