# LANE-DETECTION-USING-OPENCV
LANE DETECTION FOR AUTONOMOUS VEHICLES USING OPENCV


CONTENTS
 1. ABSTRACT
 2. INTRODUCTION
 3. EXISTING SYSTEM & DISADVANATGES
 4. PROPOSED SYSTEM & ADVANTAGES
 5. ARCHITECTURE / BLOCK DIAGRAM
 6. SYSTEM REQUIREMENT SPECIFICATION
 7.MODULES & THEIR DISCRIPTION
 8.UML DIAGRAMS
 9. OUTPUT SCREENS 
 10. CONCLUSION
 11. FUTURE ENHANCEMENT
 12. REFERENCES & BIBLOGRAPHY


ABSTRACT
❖ Autonomous driving car is one of the most disruptive innovations in AI.
❖ The main objective is to vehicle can able to drive by themselves , without any human 
interaction.
❖ One of the many steps involved during the training of an autonomous driving car is lane 
detection, which is the preliminary step. Today, we are going to learn how to perform lane 
detection using videos. 
❖ Based on the problems encountered in detecting objects by autonomous vehicles an effort 
has been made to demonstrate lane detection using OpenCV library
❖ It carries out Grayscale instead of color , Gaussian smoothing , Canny edge detection,
selecting region of interest , Hough transformation for line detection

INTRODUCTION
❖ An autonomous car can go anywhere a traditional car can go and does everything that an experienced 
human driver does.
❖ But it’s very essential to train it properly. 
❖ One of the many steps involved during the training of an autonomous driving car is lane detection, 
which is the preliminary step. 
❖ Today, we are going to learn how to perform lane detection using videos.
❖ Driver Assistant System is designed to assist drivers in the perception of any dangerous situations 
before, to avoid accidents after sensing and understanding the environment around itself 
❖ More and more accidents can be avoided if such dangerous driving condition is detected early and 
warned to other drivers. Most of the roads, cameras and speed sensors are used for monitoring and 
identifying drivers who exceed the permissible speed limit on roads and motorways. This simplistic 
approach, and there are no restrictions


EXISTING SYSTEM
❖ In this World Human driving is a like Habit to everyone like driving car , bike…etc.
❖ Mainly in Human Diving helps lot of people to creating the job opportunities .
❖ How Human can Master on the Driving ?.It is practice to learn and train in different driving 
centres with follow road rules.
❖ Human Driving is not Good at Every time because it depends on person it behaviour in the 
process of diving.
❖ Because Humans are filled by Emotions, they cannot restrict under traffic rules and
safety driving rules


DISSADVANTAGES
✓ Human drivers often bend traffic rules and take risks, even breaking laws and rules and 
posted speed limit, making the roads not safety to Everyone.
✓ The average annual road accidents death crashes stand at 1.3 lakh per year in India.
✓ Drunk driving is a serious problem that continues to take thousands of deaths each year. 
Too many innocent lives been lost to drunk driving.
✓ Human can go to long distances travelling, it takes more human effort. It causes different 
Health issues like backpain ..etc


PROPOSED SYSTEM
❖ Self driving is the most trending technology Now days. It mainly depends on 
object detection and lane detection.
❖ Lane Detection is Nothing But detecting the lanes on the road.
❖ detecting lanes using Python and OpenCV. In real time vehicular movements will be captured 
using a camera and the same will be processed to achieve the goal. The Hough Transform is 
used to detect lanes in an image or video


ADVANTAGES
✓ The autonomous vehicle can move successfully without a driver help. They can go from the initial 
point to the specified target by applying pre-defined rules. Hence it is reduces human effort for mainly 
in long distances.
✓ To control accidents are caused due to insufficient follow-up of the lanes and non-compliance with 
these rules and drunk-drive. The majority of these accidents also result in injury and death.
✓ Efficient travel means fuel savings for travelers.
✓ Greater efficiency would mean fewer emissions and less pollution from cars, meaning a lower 
negative environmental impact.
✓ Autonomous Vehicles follow traffic rules.
✓ No risk of drunk and drive.
✓ Increase efficiency of time in travelling and fuel.


MODULES & DESCRIPTION
❑ Capturing and decoding video file
❑ Grayscale conversion of image
❑ Reduce noise
❑ Canny Edge Detector
❑ Region of Interest
❑ Hough Line Transfor

Capturing and decoding video file: We will capture the video using Video Capture 
object and after the capturing has been initialized every video frame is decoded (i.e. 
converting into a sequence of images)

Grayscale conversion of image: The video frames are in RGB format, RGB is converted 
to grayscale because processing a single channel image is faster than processing a threechannel colored image.

Reduce noise: Noise can create false edges, therefore before going further, it’s imperative 
to perform image smoothening. Gaussian filter is used to perform this process
❖ Canny Edge Detector: It computes gradient in all directions of our blurred image and 
traces the edges with large changes in intensity . For more explanation please go through 
this article

Region of Interest: his step is to take into account only the region covered by the road lane. A 
mask is created here, which is of the same dimension as our road image. Furthermore, bitwise 
AND operation is performed between each pixel of our canny image and this mask. It ultimately 
masks the canny image and shows the region of interest traced by the polygonal contour of the 
mask.


Hough Line Transform: The Hough Line Transform is a transform used to detect straight 
lines. The Probabilistic Hough Line Transform is used here, which gives output as the 
extremes of the detected lines.


ough Line Transform: The Hough Line Transform is a transform used to detect straight 
lines. The Probabilistic Hough Line Transform is used here, which gives output as the 
extremes of the detected lines.

FUTURE ENHANCEMENT
❖ This model can be updated and tuned with more efficient mathematical modelling, whereas the 
classical OpenCV approach is limited .
❖ and no upgrade is possible as the approach is not efficient It is unable to give accurate results on 
the roads which do not have clear markings present on the roads.
❖ Also it cannot work for all climatic conditions This technology is increasing the number of 
applications such as traffic control, traffic monitoring, traffic flow, security etc.
❖ The importance of perception sensors, algorithms and their integration to achieve the optimized 
results for a lane detection.
❖ Advance study on efficient integration of sensors to minimize computation time, cost and 
increase effective perception is required. 




