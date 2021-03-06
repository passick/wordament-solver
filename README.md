wordament-solver
================

App that helps you play the Wordament game for WP/iOS. Here is a [video](http://youtu.be/Y5DAmTRAxzU) demonstrating the way it works.

## Usage


1. Firstly, you have to install `tesseract` (`tesseract-ocr` in Ubuntu's repos) and `OpenCV` (Ubuntu installation guide is [here](https://help.ubuntu.com/community/OpenCV)) (make sure that `pkg-config --libs opencv` prints some filenames)
2. `git clone https://github.com/passick/wordament-solver.git`
3. `cd wordament-solver`
4. `make`
5. `./squares`
6. Put your phone with the launched game session near the webcam and wait until the letters will get recognized.
7. Press any key to capture the image and let the app find all the words.
8. Enjoy.

## Comments

* This app was tested only with the default wordament color scheme. Some problems may occur with different schemes.
* Either/Or cells recognition has not been tested.
* Number of words found is usually a little bit smaller than what wordament suggests. I blame the differences in my wordlist and wordament's wordlist.
* This app has only been tested on Ubuntu 13.04. I am almost 100% sure that it won't work on Windows.

## Todo list

- [ ] Add GUI
- [ ] Make robot for fully automatic gameplay (xD)

## Acknowledgements and link

* `squares.cpp` example from OpenCV for giving me a headstart
* [How to integrate Tesseract OCR and OpenCV](http://opencv-code.com/tutorials/how-to-integrate-tesseract-ocr-and-opencv/)
* [Automatic perspective correction for quadrilateral objects](http://opencv-code.com/tutorials/automatic-perspective-correction-for-quadrilateral-objects/)
* [Detecting simple shapes in an image](http://opencv-code.com/tutorials/detecting-simple-shapes-in-an-image/)
