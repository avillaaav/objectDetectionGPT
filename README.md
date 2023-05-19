# objectDetectionGPT
Uses Google Pre-Trained model along with OpenAI API to detect objects, then give a description of them in realtime.

FILES:
webcamGPT.py <- main program used to initialize webcam and Pre-Trained detect.flite model. Also includes OpenAI API to process item.
detect.tflite <- Sample Google Tflite Model to detect approx. 80 different objects.
labelmap.txt <- These are the labels Google Tflite Model uses to classify the 80 objects.

In order to run, make sure all libraries are installed on Raspberry Pi. Put webcamGPT.py in a folder, with another folder inside named "PreTrainedGoogleModel".
Then to run, use the command:

python3 TFLite_detection_webcam.py --modeldir=PreTrainedGoogleModel

Make sure a virtualenv is created with all libraries inside and you are inside the virtual environment prior to running. A webcam should also be plugged into the Raspberry Pi with legacy webcam mode ON for it to be detected. Thanks.
