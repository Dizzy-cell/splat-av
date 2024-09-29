# Drivable Gaussian Splatting Avatar with Monocular Videos
This is a WebGL implementation of a real-time renderer for Drivable Gaussian Splatting Avatar.

You can try it on [web](https://dizzy.us.kg).
Try with a camera for mediapipe blendshape on [web](https://dizzy.us.kg/index2.html).


Demo with the driveable avatar by MediaPipe BlendShape.![demo](https://github.com/Dizzy-cell/splat-av/blob/main/assets/video.gif)
Demo with the driveable avatar by MediaPipe BlendShape.![demo](https://github.com/Dizzy-cell/splat-av/blob/main/assets/blend.gif)

# Description
1. Create the drivable gaussian avatar by monocular videos.
2. Aim to realtime drive and render on mobie devices.
3. Morphable model saves a .plat file and drive params save a .json file. 

# Problems
1. Blur, caused by modeling and data.
2. Driving the mouth area. caused by the occlusion.

# Dataset Prepare
Two types of videos, recording for 2 to 3 minutes.
1. static camera and dynamic facial expressions.
2. static facial expressions and dynamic camera.

We choose the static camera and dynamic facial expressions to collect the facial data. 
Inspired by the Persona with Apple, we list a series of facial expressions and movements.
1. canonical experssion with rotating the neck clockwise.
2. Speeching with some senctences.

# Train

# Test

# Image Restoration with GFPGAN.

The drawback of rendering with Gaussian splatting with the animator avatar is that it is difficult to model and recover the region of the mouth. 
We discover the research of image restoration or super-resolution about face. We adopt the pretrained GFPGAN to restore the rendering face of gaussian splatting.
In consideration of the work about the Qualcomm® AI Hub Models on real-time super-resolution,like real-esrgan, the inference time is considered feasible if it is migrated to mobile devices. 

## acknowledgements
Thanks to Kevin Kwok for the original [code](https://github.com/antimatter15/splat) with 3D Gaussian Splatting.