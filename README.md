# Drivable Gaussian Splatting Avatar 
This is a WebGL implementation of a real-time renderer for Drivable Gaussian Splatting Avatar.

You can try it on [web](https://dizzy.us.kg).


Demo with the driveable avatar by MediaPipe BlendShape.![demo](https://github.com/Dizzy-cell/splat-av/blob/main/assets/video.gif)

# Description
1. Create the drivable gaussian avatar by monocular videos.
2. Aim to realtime drive and render on mobie devices.
3. Morphable model saves a .plat file and drive params save a .json file. 

# Problems
1. Blur, caused by modeling and data.
2. Driving the mouth area. caused by the occlusion.

## acknowledgements
Thanks to Kevin Kwok for the original [code](https://github.com/antimatter15/splat) with 3D Gaussian Splatting.