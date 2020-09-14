# Open CV :notebook:
## Topics:clipboard:
:one: Introduction<br>
:two: Features of OpenCV Library<br>
:three: Open CV library Modules<br>
:four: Installing OpenCV<br>
:five: Top 5 inevitable Methods in OpenCV using Python<br>
:six: Summing up Examples<br>
:seven: Conclusion<br>
### Introduction :speech_balloon: <br>
***OpenCV is a cross-platform library using which we can develop real-time computer vision applications. It mainly focuses on image processing, video capture and analysis including features like face detection and object detection. In this tutorial, we explain how you can use OpenCV in your applications.***<br>
**Computer Vision defination:** Computer Vision is an interdisciplinary field that deals with how computers can be made to gain a high-level understanding from digital images or videos.<br>
***Computer Vision overlaps significantly with the following fields:-***<br>

1. Image Processing − It focuses on image manipulation.

2. Pattern Recognition − It explains various techniques to classify patterns.

3. Photogrammetry − It is concerned with obtaining accurate measurements from images.***<br>

**How Does A Computer Read An Image?**<br>

<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/12/Picture1-1.jpg"/><br>
We can figure out that it is an image of the New York Skyline. But, can a computer find this out all on its own? The answer is no!<br>
The computer reads any image as a range of values between 0 and 255.<br>
For any color image, there are 3 primary channels – Red, green and blue. How it works is pretty simple.<br>
A matrix is formed for every primary color and later these matrices combine to provide a Pixel value for the individual R, G, B colors.<br>
Each element of the matrices provide data pertaining to the intensity of brightness of the pixel.<br>
Consider the following image:<br>
<img src="https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2018/12/Picture2-3.png"/><br>
As shown, the size of the image here can be calculated as B x A x 3.<br>
Note: For a black-white image, there is only one single channel.<br>
Next up on this OpenCV Python Tutorial blog, let us look at what OpenCV actually is.<br>

### Features of OpenCV Library:- :books:<br>
* Read and write images
* Capture and save videos
* Process images (filter, transform)
* Perform feature detection
* Detect specific objects such as faces, eyes, cars, in the videos or images.
* Analyze the video, i.e., estimate the motion in it, subtract the background, and track objects in it.<br>
### OpenCV Library Modules :blue_book:<br>
| S.NO| Modules| In Java packaage  Nmae| 
|---------|---------|----------|
|  1.   |  Core Functionality   |   org.opencv.core.   |
|  2.   |  Image Processing  |  org.opencv.imgproc.   |  
|  3.   |  Video   | org.opencv.video.  |
|  4.   |  Video I/O  |   org.opencv.videoio.  |  
|  5.   |  Calib3d  |  org.opencv.calib3d.    |
|  6.   |  features2d |   org.opencv.features2d.   |  
|  7.   | Objdetect |   org.opencv.imgcodecs  |  
|  8.   |  Highgui  |  org.opencv.imgcodecs   |
### Installing OpenCV :link:<br>
* [click here to download Anaconda](https://www.anaconda.com/products/individual)
<img src="https://static.javatpoint.com/tutorial/opencv/images/installation-of-opencv.png"/><br>
* After installing it, open the Anaconda prompt and type the following command.
<img src="https://static.javatpoint.com/tutorial/opencv/images/installation-of-opencv3.png"/><br>
* Press the Enter button and it will download all the related OpenCV configuration.
<img src="https://static.javatpoint.com/tutorial/opencv/images/installation-of-opencv4.png"/><br>
* Install OpenCV in the Windows via pip command:
***pip install opencv-contrib-python --upgrade***
<img src="https://static.javatpoint.com/tutorial/opencv/images/installation-of-opencv5.png"/><br>
* Open the command prompt and type the following code to check if the OpenCV is installed or not.
<img src="https://static.javatpoint.com/tutorial/opencv/images/installation-of-opencv6.png"/><br>
### Top 5 inevitable methods  in OpenCV using Python :beginner:
* #### cv2.imread()
 The method imread, more commonly called as image read, in opencv is used for reading the images from a file path<br>
 ***Parameters: cv2.imread(filename[,flags])***<br>
 In the above parameter you can see that the mandatory requirement is the filename which can be passed as a string. The filename is the image which you want to be read by the     computer.
<img src="https://miro.medium.com/max/875/0*ruxnUTWht0BOuUlF"/>
Note: alpha channel is the one which decides the opacity/transparency of an image<br>
**Example: img = cv2.imread(r’C:\Users\MrBean.webp’,0)**<br>
* #### cv2.imshow()
As the name suggests this method is used for showing the images<br>
***Parameters: cv2.imshow(window_name,image)***<br>
The window_name should be a string value and hence will be in enclose in double or single quotes. The image shall be the image which should be<br>
**Example: cv2.imshow(“MrBean”,img)**<br>
* #### cv2.cvtColor()
cvtColor can be interpreted as convert color and this method is used for converting the image from one color space to another color space (Find what is a color space here if you don’t know about it)<br>
***Parameters: cv2.cvtColor(src, code[, dst[, dstCn]])***<br>
src is the source image whose color space you intend to change. code is the one which specifies “to which color space should the source image should be converted”. Since other parameters are not mandatory, as a beginner you can skip it for time being<br>
**Example: cv2.cvtColor(img, cv2.COLOR_RGB2GRAY)**<br>
* #### cv2.waitKey()
This function is very important, without this function cv2.imshow() won’t work properly.<br>
***Parameters: cv2.waitkey(wait time in milliseconds)***<br>
Thus if the wait time is entered as 6000, the picture will be displayed for 6s and then get closed (provided you have cv2.destroyAllWindows() in the script). If you use ‘0’ as the parmater then the image will be displayed for infinite time until you press the esc key.<br>
**Example: cv2.waitKey(0)**<br>
* #### cv2.destroyAllWindows()
This method destroys (in other words “closes”) all the windows created using the opencv methods. If you want to close a specific window, then you can pass the window name as the argument within this function<br>
***Parameters: name of a window opened using opencv (not mandatory)***<br>
Missing to provide the cv2.destroyAllWindows() at the end of the script might make the window opened to crash<br>
### Summing up the examples: :exclamation:
1. **Output for flag values of cv.imread()**<br>
<img src="https://miro.medium.com/max/875/1*yp9VgXSohg76xv9frq72Ug.png"/><br>
<img src="https://miro.medium.com/max/875/1*8z7QQOZwn0sTvF7krSaMvQ.png"/><br>
<img src="https://miro.medium.com/max/875/1*ouexiTh5qY8iTbW8kk-cqA.png"/><br>
2. **cv.cvtcolor()**
<img src="https://miro.medium.com/max/875/1*0nuTMpzubXI2orgOR2WNoQ.png"/><br>
<img src="https://miro.medium.com/max/875/1*NiexARigH-_mPcp2K8J6_Q.png"/><br>
3. **cv.waitkey()**<br>
<img src="https://miro.medium.com/max/875/1*F9KfEyaURxbDbY3ufchrpA.gif"/><br>
### Conclusion :triangular_flag_on_post:
 ###### Basic methods  to read, show, convert color and make an image wait for few seconds before it closes.



 




