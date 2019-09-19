# hand_gesture_recognition
hand_gesture_recognition with web camera

There are many possible approaches to solve this problem, each with different complexity and accuracy</br>

We decided that the best approach to solve our problem, in terms of complexity and reliability, is to segment the hand starting from the color of the user’s skin</br>

Background removal</br>

At this point the program is working but, due to the unpredictability of the scene conditions, it is not particularly reliable. A simple change of illumination or a background with a color too similar to the color of the user’s skin may give a lot of false positives. In order to solve this problem we decided to add an extra step to our process: background removal, before binarization.
In a first approach we tried to use dynamic background subtraction. The problem with this solution is that the hand has to always move, otherwise it is classified as background and then removed.</br>

Fingers identification</br>
The points of intersection between the hand contour and convex hull are saved in an array, they will be used to locate the finger tips.</br>

output


