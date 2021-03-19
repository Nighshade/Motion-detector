# Motion-detector
Motion detector using open CV in python. It detects the change in the position of the foreign object with respect to it's surroundings.

You can use motion-detector to:-
1) Monitor any tresspasser 
2) Baby activity monitor
3) animal activity in farm or alley(bear attack)

How to RUN:
You can run Motion detector using python 3.
First, you will need to install some external modules that don't come pre-installed with python. like cv2,pandas, datetime,time.
To install the modules run the command below
pip install pandas cv2

The application will capture the first frame via webcam. This frame will be treated as the baseline frame.
Motion will be detected by calculating the phase difference between this baseline frame and the new frame with some object. The new frames will be called Delta frame.
Using pixel density the delta frame will be refined. then the refined frame will be called Threshold frame.
Shadow removal,Dilation,Contouring will be applied.
All timestamps are further stored onto a csv file.
