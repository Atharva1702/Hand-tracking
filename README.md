# Hand-tracking
The hand tracking is made using Python code which detects the hands as they move along the camera  We used OpenCV and mediapipe 

![image](https://github.com/Atharva1702/Hand-tracking/assets/90234696/347919a4-4ec9-4c1c-bb80-64b1fda49430) 


 **Mediapipe**: The MediaPipe uses a single-shot palm detection model and once that is done it performs precise key point localization of 21 3D palm coordinates in the detected hand region.

The MediaPipe pipeline utilizes multiple models like, a palm detection model that returns an oriented hand bounding box from the full image. The cropped image region is fed to a hand landmark model defined by the palm detector and returns high-fidelity 3D hand key points.

it looks like the given picture below..


![download (5)](https://github.com/Atharva1702/Hand-tracking/assets/90234696/fb8d47de-1b1b-4921-a765-e401bb914b2a)




### Installing libraries
In this code we have used Python code to work in **OpenCV** and **mediapipe**.


We install openCv using : !pip install opencv-python command 

And mediapipe using: !pip install mediapipe  to use these in our code.

This can also be thought as Hand Skeleton.

### Code

We imported **OpenCV as cv2** and **mediapipe as mp**. we first called our webcam to use the real-time tracking using **VideoCapture(0) as 0 is assigned to the inbuilt web cam**. 

Then we used mediapipe to create some objects and called them into the while loop which runs along the infinite time to capture. Then we converted the BGR color format to GRAY color format the real time frames in video 

we gave all the 21 points abd connected them using mediapipe's **HAND_CONNECTIONS** colors and locations to any specific point that we wished.

And the final result looked like this.!

![Untitled video - Made with Clipchamp](https://github.com/Atharva1702/Hand-tracking/assets/90234696/dd25bc86-6ea4-4de3-8a23-52e95972a8bf)




  



