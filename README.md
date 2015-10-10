# ECG + HTM

Real-Time Electrocardiogram(ECG) Anomaly Detection System using HTM

## Abstruct

In this projects, We build real-time Electrocardiogram(ECG) anomaly detection system using HTM.
This system will detect Palpitation, Arrhythmia and Heart Rate anomaly.

To collect data, we use some hardware, 
[SparkFun SEN-12650](https://www.sparkfun.com/products/12650) and [Arduino](https://www.arduino.cc/). 
This system's total cost is under $50.

## Usage

### Take data

```
$ python2.7 take_data.py
```

### Plot with Gnuplot

```
$ gnuplot
plot "< head -1000 sample_ecg.txt" with line
```

## System Structure

### Software

Use [NuPIC](https://github.com/numenta/nupic).

Write here more detail.

### Hardware

* [SEN-12650](https://www.sparkfun.com/products/12650) - SparkFun's Single Lead Heart Rate Monitor
	* [AD8232](http://www.analog.com/en/products/application-specific/medical/ecg/ad8232.html) installed.
	* [Good tutorial](https://learn.sparkfun.com/tutorials/ad8232-heart-rate-monitor-hookup-guide/connecting-the-hardware)
* [Arduino Pro Mini](https://www.arduino.cc/en/Main/ArduinoBoardProMini) 

## Data

Real-Time streaming data from ECG device.

## TODO

Take ECG data with anomaly.
