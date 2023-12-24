---
title: "LSTM-based Realtime Dst Index Predictor"
excerpt: "<img src='/images/dst.png' width='615'>"
collection: portfolio
---

In this self-guided project, I created a Flask web application for real-time forecasting of the Disturbance storm time (Dst) index using a Long Short-Term Memory (LSTM) neural network model. The application employs Selenium for web scraping, extracting pertinent data from two distinct data fetching URLs (https://wind.nasa.gov/mfi_swe_plot.php and https://www.sidc.be/SILSO/DATA). In headless Chrome mode, the script navigates through the HTML content of the specified pages, capturing Magnetic field Components (B,Bx,By,Bz),Plasma Velocity, and Proton Number Density(Np) [Hourly Updated] along with Daily Sunspot Number[Daily Updated]. The pre-trained LSTM model, implemented with TensorFlow and Keras, is loaded for Dst index prediction based on the scraped data. The script orchestrates a background scheduler from apscheduler to periodically invoke the web scraping and prediction process at a predefined interval, specifically every hour. Flask routes are established to provide JSON-formatted current values and to render a web page (index.html) showcasing the predicted Dst index values. (Hosted on GCP (Google App Engine))
<br>Model Infromation:

<br>Model: sequential
<br>_______________________________________________________________________________________
<br>Layer (type)&nbsp;&nbsp;&nbsp;&nbsp; Output Shape&nbsp;&nbsp;&nbsp;&nbsp;Param #
<br>===================================================
<br>lstm1 (RNN)&nbsp;&nbsp;&nbsp;&nbsp;(None, 34, 256)&nbsp;&nbsp;&nbsp;&nbsp;278528
<br>lstm2 (RNN)&nbsp;&nbsp;&nbsp;&nbsp;(None, 256)&nbsp;&nbsp;&nbsp;&nbsp;525312
<br>dense (Dense)&nbsp;&nbsp;&nbsp;&nbsp;(None, 2)&nbsp;&nbsp;&nbsp;&nbsp;514
<br>===================================================
<br>Total params: 804354 (3.07 MB)
<br>Trainable params: 804354 (3.07 MB)
<br>Non-trainable params: 0 (0.00 Byte)
<br>_________________________________________________________________________________________
<br>Test RMSE: 12.85
<br>Link to GitHub Repository for this project can be found [here](https://github.com/deepghuge/DstIndex)  (this is not the one that is hosted on GCP, can be can be recreated on a local system) 

