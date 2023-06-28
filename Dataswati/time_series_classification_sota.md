
## Time series classification state of the art 


### Context 

Dataswati develops [PowerOP](https://www.dataswati.com/en/powerop), a Software-as-a-Service designed for the food processing industry. It collects data from various sources such as sensors, settings, ingredients, and recipes and uses advanced analytics to reduce resource consumption while improving product quality.

The goal of this project was to investigate innovative approaches for accurately classifying time series, particularly those derived from sensors, as part of implementing certain AI functionalities within PowerOP. Achieving precision across numerous instances of time series played a pivotal role in establishing effective alarm systems, among other crucial applications. By examining contemporary methods in this area, we sought to identify suitable technologies that would meet high standards required for operational deployment within PowerOP.


If you wish to learn more about how PowerOP could benefit your organization, please visit the [official website](https://www.dataswati.com/en/powerop), you can ask for a demo on the website or or email the CEO directly at [averleyen@dataswati.com](averleyen@dataswati.com) to schedule a customized demonstration using the subject line "PowerOP Demo."

### Methodology 
![image](https://www.sktime.net/en/latest/_images/tsc.png)
To advance this project's objectives, a specific case study provided by one of our clients was chosen as the basis for testing different methodologies. Accessible through the PowerOP platform, the data associated with the given situation served as our primary resource for trials. In pursuing the state-of-the-art in time series classification, our initial steps involved conducting literature reviews and online surveys to pinpoint the top techniques currently available, along with their Python implementations. Ultimately, all were subjected to the challenge of analyzing the client-provided time series data, so as to gauge their overall effectiveness and applicability within the context of our goals.

Some of the most interesting methods (applied to the case of sensor time series classification) selected were : 
- Autoencoders with [pytorch](https://pytorch.org/)
- [sktime](https://github.com/alan-turing-institute/sktime) : we used the most promising algorithms for [the time series classification benchmark](https://www.timeseriesclassification.com/) 
- [tslearn](https://github.com/tslearn-team/tslearn) : allow for fast implementation of state of the art deep learning algoritms. 

### Tools
- Python : tslearn, sktime, pytorch, pandas
- Docker for packaging 
- VSCode for development

### My involvment 
I guided and trained a junior colleague working alongside on this venture, ensuring he became familiarized with appropriate tools and methodologies while producing reliable workflows encompassing open source software.

### Results and achievements

- Successfully applied modern time series classification methods to actual data from the real world.



### References

Cote J., & Hwang S.-K. (2019). : Highlighting Important Variants and Ensembles. arXiv preprint arXiv:1910.13051. <https://doi.org/10.48550/arXiv.1910.13051>

