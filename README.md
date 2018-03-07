# TensorFlow-ANPR
The project developed using TensorFlow to detect the License Plate from a car and uses the Tesseract Engine to recognize the charactes from the detected plate.

### Software Packs Needed
* <a href='https://www.anaconda.com/download/'>Anaconda 3</a> (**Tool comes with most of the required python packages along with python3 & spyder IDE**)<br>
* <a href='https://github.com/tesseract-ocr/tesseract'>Tesseract Engine</a> (**Doesn't need to be installed cause I included the trained OCR data along in the repository**)<br>

### Python Packages Needed
* <a href='https://github.com/tensorflow/tensorflow'>Tensorflow</a><br>
* <a href='https://github.com/skvark/opencv-python'>openCV</a><br>
* <a href='https://github.com/madmaze/pytesseract'>pytesseract</a><br>
* <a href='https://github.com/tzutalin/labelImg'>labelImg</a><br>

### ABOUT PROJECT
* TensorFlow is an open-source software library **(Deep learning)** for dataflow programming across a range of tasks. It is a symbolic math library, and also used for machine learning applications such as neural networks. So we have planned to use it for number plate detection.

#### TRAINING PHASE
#### IMAGE LABELING
* Collected the set of 100 images (Cars along with number plate) from the sources such as Google Images and Flickr. Then annotated the set of images by drawing the boundary box over the number plates to send it for the training phase.
  * The Annoation gives the co-ordinates of license plates such as **(xmin, ymin, xmax, ymax)**
  * Then the co-ordinates are saved into a **XML** file
  * All the XML files are grouped and the Co-ordinates are saved in **CSV** file.
  * Then the CSV file is converted into **TensorFlow record format**.
* The set of other separate 10 images also gone through the above steps and saved as **Test Record file** 
  
