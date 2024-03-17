# MultimeterReader
This Jupyter Notebook is useful to extract **multimeter readings from videos**

# How it works
1. The video is separated into frames at regular intervals
2. Each frame is manipulated using OpenCV for better reading of the display
3. Each digit is read by a Keras NN trained using the dataset from [Like MNIST, but for 7-segment display](https://connormonahan.net/2020/09/27/seven-segment-display-dataset.html])
4. The final reading is added to a Python array for later processing
