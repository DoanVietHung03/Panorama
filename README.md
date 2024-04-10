Images stitching from diferent viewpoints

INSTRUCTION:
CREATE DATA:
- You can create multiple images. Make sure there will be some overlapping parts between two consecutive created images in a sequence. Then algorithm will find and match features and create panorama image of all images which you have provided. 
- OR you can directly feed multiple images from camera in a sequence with some overlapping parts between two consecutive images. 

Please install Libraries:
1. Numpy
2. OpenCV (version 3.3.0)
3. imutils

TO RUN CODE:
1. Put images in your current folder where your code is present.
2. Run stitch.py code.
3. Provide the number of images you want to concantenate as input. Like: 2,5,6,10 etc.
4. Enter the image name in order of left to right in way of concantenation. Like:
    Enter the 1 image: room1.jpg
    Enter the 2 image: room2.jpg

5. Then, you will get your panorama image as Panorama_image.jpg in your current folder. 

- Used SIFT to detect feature and then RANSAC, compute Homography and matched points and warp prespective to get final panoramic image.
