# kneebend
Kneedbend with timer and video cleaner using OpenCv and Mediapipe.<br />
I developed a script that removes fluctuating frames from a video and utilizes MediaPipe to detect the pose in each frame. The script specifically checks for the angle of the knee, and if the angle is less than 140°, a timer is activated and displayed on the video. If the timer reaches 8 seconds, a repetition is counted and added to the output statistics of bendness.

## INSTRUCTIONS
### This project requires the following libraries<br />

• [Os](https://python.readthedocs.io/en/stable/library/os.html)<br />
• [Cv2(OpenCV)](https://docs.opencv.org/4.x/)<br />
• [Mediapipe](https://google.github.io/mediapipe/)<br />
• [Numpy](https://numpy.org/)<br />
• [scene detect](http://scenedetect.com/en/latest/)<br />

### Please ensure you have installed the following libraries mentioned above before continuing.


## HOW TO RUN knee_bend.py

open cmd in the file directory and write:
```
python knee_bend.py --video "path"
```
for eg:
```
python knee_bend.py --video "C://user//downloads//kneebend.mp4"
```
You will get stats_of_bendness.txt in the same directory where the knee_bend.py file is saved
and kneebend_output.mp4 will also be saved in the same directory.

Press "Esc" on video windows to stop the code.
