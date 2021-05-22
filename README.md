# Resources used in Google ML Kit Text Recognition

## What is this?

These are Tensorflow lite trained models and protobuf-based binary configuration used in the Text Recognition of Google ML Kit. These files are obtained by downloading the `GoogleMLKit/TextRecognition` pod in iOS, under `MLKitTextRecognition/Resources/GoogleMVTextDetectorResources`. I have also decoded these file using `protoc` and `flatc`.

## Motivation

I am searching for a text recognition solution that would work with no internet access, and would be available for any platform, at least Amdroid, iOS and browser. I have tried many open-source models like tesseract and some models in Tensorflow Hub, but none of them ever produced useful results. I have since discovered that the ML Kit would provide good results and still being on-device. However, it seems that it only support Android and iOS, and the Android version require some downloading as well. So I decided to do some reverse engineering and what is in the repo is the essence of my work, which should include all the relavant resources used for text recognition.

## What's next?

I am now trying to figure out what is happening with these models and provide useful instructions on using them practically, but I probably need some help here since I am really not an expert in data engineering. I am looking for making an example to integrate these models with tensorflow lite and tensorflow.js.

Also, have also came across the android version of these models, which are bigger in size (perharps would produce better results). However those models does not look like a valid tflite model so I guess I won't touch them right now, just focus on getting the iOS models to work first.

