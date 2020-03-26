## Environment
- OS: MacOS (prefered)
- Platform: Python 2.7
- Librarys: 
	- OpenCV 2.4.13
	- appscript

## How to run it?
- run it in python
- press 'b' to capture the background model (Remember to move your hand out of the blue rectangle)
- press 'r' to reset the backgroud model
- press 'ESC' to exit

#### Capture background model & Background subtraction
Use background subtraction method called **Gaussian Mixture-based Background/Foreground Segmentation Algorithm** to subtract background. 

#### Contour & Hull & Convexity 
We now need to find out the hand contour from the binary image we created before and detect fingers (or in other words, recognize gestures)

This function will find all the contours from the binary image. We need to get the biggest contours (our hand) based on their area since we can assume that our hand will be the biggest contour in this situation. (it's obvious)

Now we have the number of fingers. How to use this information? It's based on your imagination.

I add in a keyboard simulation package named **appscript** as interface to control Chrome's dinosaur game.
