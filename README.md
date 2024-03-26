# MultimeterReader
This Jupyter Notebook is useful to extract **multimeter readings from videos**

# Warning
This notebook was written by Achille Merendino for the A1 Group of Laboratorio di Elettromagnetismo e Circuiti 2024
This software comes with no warranty whatsoever and you should always double check its output.
I have tested this software with footage from the laboratory and my own multimeter at home, it had $\sim$ 98% accuracy in both cases, but still DO NOT TRUST IT BLINDLY!

# How it works
1. The video is separated into frames at regular intervals
2. Each frame is manipulated using OpenCV for better reading of the display
3. Each digit is read by a Keras NN trained using the dataset from [Like MNIST, but for 7-segment display](https://connormonahan.net/2020/09/27/seven-segment-display-dataset.html)
4. The final reading is added to a Python array for later processing

# Some screenshots
This is my multimeter!

![Misurator Icon](https://achilleme.com/static/multimeter_reader/multimeter.png?)

And this is the display after a little bit of OpenCV

![Misurator Icon](https://achilleme.com/static/multimeter_reader/display_cv.png?)

Finally, the final plot

![Plot](https://achilleme.com/static/multimeter_reader/plot.png?)
