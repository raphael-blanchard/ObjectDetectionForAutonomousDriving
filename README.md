# ObjectDetectionForAutonomousDriving

## Approach

This neural network is based on the YOLO (You Only Look Once) paper from [Redmond & Al](https://arxiv.org/abs/1506.02640).

The main advantage of the YOLO approach for computer vision is its speed and efficiency in object detection tasks. Unlike other object detection methods that require multiple passes over an image or region proposal generation, YOLO processes the entire image in one pass and directly predicts the bounding boxes and class probabilities for all objects in the image. This makes YOLO much faster than other object detection algorithms while still maintaining high accuracy.

Additionally, YOLO is designed to be an end-to-end system, meaning that it can be trained directly on raw image data without the need for feature extraction or pre-processing steps. This makes it easier and faster to train YOLO for new tasks, as it can learn to detect objects directly from the raw pixel data.

Overall, the combination of speed and accuracy makes YOLO a popular choice for real-time object detection applications, such as autonomous vehicles, robotics, and video surveillance systems.

## Examples

Here is an example when running a prediction on a single image, with on the left the raw image and on the right the image returned by the neural network:

<p float="left">
  <img src="https://user-images.githubusercontent.com/86181145/205443119-d01be4e8-8774-4c71-aa7c-e05d99567d9d.jpg" width="49%" height="49%">
  <img src="https://user-images.githubusercontent.com/86181145/205443118-5dc81cd9-9e17-496c-8a7a-43fa5250c38e.jpg" width="49%" height="49%">
</p>

After passing each frame of a video from a dashcam (fig 2.) to the neural network and putting them back together into a video, we get the following result:

Figure 1 - Predicted video:

https://user-images.githubusercontent.com/86181145/205443761-2c5f266c-0d5d-4df0-8ada-969023fd81dc.mp4


Figure 2 - Raw video from a dashcam:

https://user-images.githubusercontent.com/86181145/205443756-a8566274-8d99-4435-8af8-a27595538d97.mp4






