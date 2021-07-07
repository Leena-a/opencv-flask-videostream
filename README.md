# opencv-flask-videostream
Python project uses OpenCV to stream video from a webcam to a web browser/HTML page with motion detection using Flask.


> System: Ubuntu 18.04

> Python3 version: Python 3.6.9

> [Project source]


## Requirements 

Installing pip:
```
$ sudo apt install -y python3-pip
```

Upgrading pip version:
```
$ pip3 install --upgrade setuptools
$ pip3 install --upgrade pip
```

Installing required tools:
- Flask
```
$ Pip3 install flask
```
- NumPy, OpenCV, and imutils
```
$ pip3 install numpy
$ pip3 install opencv-cosntrib-python
$ pip3 install imutils
```



## Inside your project file

1- Save `webstreaming.py` which will use OpenCV to access the web camera.

2- Create `pyimagesearch` module with `motion_detection` submodule inside.

3- Save `SingleMotionDetector.py` file inside `motion_detection` submodule to perform motion detection.

4- Create `templates` directory and save `index.html` inside it, to populate its contents with HTML used to serve the video feed.




## Execution 

Making scripts executable:
> Assuming that the project file named `Python`.
```
$ cd /Python
$ chmod +x webstreaming.py
$ cd /Python/pyimagesearch/motion_detection
$ chmod +x singlemotiondetector.py
```

To execute the project:
```
$ python3 Python/webstreaming.py --ip 0.0.0.0 --port 8000
```

![flask_opencv_stream](https://user-images.githubusercontent.com/52850659/124815578-1cf3c100-df70-11eb-8f84-2431cb5db60a.png)



Note that an RPi camera module or a USB webcam is required for the video stream to start.




[//]: #
[Project source]: <https://www.pyimagesearch.com/2019/09/02/opencv-stream-video-to-web-browser-html-page/>



