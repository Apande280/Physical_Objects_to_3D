# Physical_Objects_to_3D
In this project, we use object detection with the help of YOLO and when it detects a specific object using a raspberrypi camera that we specify, it loads the 3D file of its mesh into genesis for a simulation. The objects we specified are bottle, cup, mouse, chair and TV. The 3D files where accessed from online websites. NOTE: RaspberryPi doesn't support the Genesis GUI, and a USB camera is required for the script to work. Genesis can't work with python 3.13 yet, so create a virtual environment with a lower version python.


# Libraries needed
```bash
pip install ultralytics
pip install genesis-world
```

# Command to run the script
```bash
python genesis_test.py --model=yolo11n_ncnn_model --source=source --resolution = hxw
```

Source can be an image or videa saved on computer or 'picamera0' or 'usb0' if using raspberrypi