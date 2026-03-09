Create a Jupyter notebook in Python using PyTorch that:

1. Loads a pretrained HRNet-style keypoint detection model
2. Accepts a folder of dog side-view images
3. Preprocesses images (resize, normalize)
4. Runs keypoint inference
5. Outputs keypoints per image. The dataset uses 24 keypoints for dog pose estimation:

**Legs**
- 0: Front Left Paw
- 1: Front Left Knee
- 2: Front Left Elbow
- 3: Rear Left Paw
- 4: Rear Left Knee
- 5: Rear Left Elbow
- 6: Front Right Paw
- 7: Front Right Knee
- 8: Front Right Elbow
- 9: Rear Right Paw
- 10: Rear Right Knee
- 11: Rear Right Elbow

**Body:**
- 12: Tail Start
- 13: Tail End
- 22: Withers
- 23: Throat

**Head & Face:**
- 14: Left Ear Base
- 15: Right Ear Base
- 16: Nose
- 17: Chin
- 18: Left Ear Tip
- 19: Right Ear Tip
- 20: Left Eye
- 21: Right Eye

**Note:** Only visible keypoints (visibility > 0)

6. Visualizes keypoints on the image
7. Saves results to JSON and CSV with format:
   image_name, keypoint_name, x, y, confidence

Use clean modular code and comments.
