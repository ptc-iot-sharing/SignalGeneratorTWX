## Thingworx Signal generator

### Why use it?

In many apps you have to generate data that does not look completely random. This project helps you generate that data.

### How to use it?

* If you want to generate a chart, then use the `getNoise` service  `SignalGenerator` thing. This service returns a infotable with your data. This are the required parameters:
    * `scale`: how "contiguous" you want the signal to be
    * `amplitude`: how big is the dynamic part of the signal
    * `additiveGradient`: Gain, or by how much you want each point to grow
    * `offset`: offset the signal from 0 (smallest data point)
    * `sampleTime`: 



### How it works

It uses a [Perlin Noise 1D](https://en.wikipedia.org/wiki/Perlin_noise) generator.

