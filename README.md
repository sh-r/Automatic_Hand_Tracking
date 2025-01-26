# Automatic_Hand_Tracking
Build an automatic pipeline that tracks hand movements in a video

Part 1: Detected Hands in a Frame
Extracted coordinates for the hand and bounding box coordinates for the hand using Google MediaPipe.

Part 2: Used Part 1 and Segment Anything 2 (SAM2 model) to segment only hands in video
Positive points: From Part 1
Negative points: 
  1. Points around positive points but within a certain threshold and not part of another hand object.
  2. Other randomly selected points from image that are not part of hand object.
