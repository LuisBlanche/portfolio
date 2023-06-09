
## Time series classification state of the art 


### Context 
Dataswati develops [PowerOP](https://www.dataswati.com/en/powerop) as a service intended for the food processing industry. It centralises the data from the production line (sensors, settings, ingredients, recipes, etc. ) and leverages data visualisation and machine learning to help saving resources and improve quality. 

The majority of the data that is collected is time series. For many of the AI features developed for PowerOP there is a need for accurate classification of time series, or multiple time series. For instance creating an alert can be summed up to a binary classification on multiple sensor time series. This project aimed at exploring the state of the art solutions for time series classification that could be used in production for PowerOp. 
### Methodology 
![image](https://www.sktime.net/en/latest/_images/tsc.png)
A case study from a customer was picked up and the data can be directly accessed using PowerOP tooling. A litterature and web review was conducted to assess what are the state of the art algorithms, and which of them have a decent python implementation. We then test the libraries on the data and compare them both in usability and performance to assess if they could be used in production. 

The most interesting methods (applied to the case of sensor time series classification) selected were : 
- Autoencoders with [pytorch](https://pytorch.org/)
- [sktime](https://github.com/alan-turing-institute/sktime) : we used the most promising algorithms for [the time series classification benchmark](https://www.timeseriesclassification.com/) 
- [tslearn](https://github.com/tslearn-team/tslearn) : allow for fast implementation of state of the art deep learning algoritms. 

### Tools
- Python : tslearn, sktime, pytorch, pandas
- Docker for packaging 
- VSCode for development

### My involvment 
I managed and mentored a junior Data Scientist on this project to help him find the good libraries, orient him on the best practices and help him to build reproducible code. 

### Results and achievements

- successfuly apply state of the art time series classification algorithms to real world data



### References

HIVE COTE : https://arxiv.org/abs/1910.13051