# Human-face-detection
It captures video frames from the default camera (usually the webcam) using OpenCV's VideoCapture.
It converts each captured frame from the BGR color space to the RGB color space, as required by MediaPipe.
It uses the MediaPipe Pose model to detect a person's pose in the captured frame.
If a human is detected in the frame, it prints "human detected" and draws the pose landmarks on the frame, connecting them with lines to represent the skeleton structure of the person.
It also marks each detected pose landmark with a red circle on the frame.
It continuously displays the annotated frame in a window using OpenCV's imshow and waits for a key event. If the window is closed, the loop terminates, and the application is shut down using cv2.destroyAllWindows().
