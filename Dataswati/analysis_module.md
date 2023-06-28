## Analysis module for [PowerOP](https://www.dataswati.com/en/powerop), a food production line monitooring SAAS 


### Context 
Dataswati develops [PowerOP](https://www.dataswati.com/en/powerop), a Software-as-a-Service designed for the food processing industry. It collects data from various sources such as sensors, settings, ingredients, and recipes and uses advanced analytics to reduce resource consumption while improving product quality.

The analysis module helps users investigate anomalies or issues occurring along the food manufacturing process through detailed evaluation of data-driven insights. Users may query, "What is causing a specific quality issue?" or "Why is my power consumption spiking periodically?" 

If you wish to learn more about how PowerOP could benefit your organization, please visit the [official website](https://www.dataswati.com/en/powerop), you can ask for a demo on the website or or email the CEO directly at [averleyen@dataswati.com](averleyen@dataswati.com) to schedule a customized demonstration using the subject line "PowerOP Demo."


### Methodology 

There are two types of analyses, one is made from comparing data distributions, the other with a classification model explained with Shap values.

1. Distribution 
    Used to separate raw datasets into distinct groups based on a chosen target parameter (binary indicator). This approach measures variations in distributions across both subgroups. By examining these disparities during specific timespans, users can determine which factors strongly impact their results. These divergences can reveal potential causes for unexpected outcomes. For further exploration of these patterns, customers can navigate between different time frames and selected features within this interface section. Furthermore, a decision tree is used to identify ideal cutoff points distinguishing data partitions to help developing avoidance strategies.

![Histogram intesection](../assets/img/Dataswati/histogram_intersection_1.png)
   

2. Machine Learning
     An AutoML pipeline featuring configurability, accommodating various input parameters stored in a MongoDB Document, was developed by our team. With its flexible design, it caters to a range of binary classification problems. Users must only specify certain conditions, including covariates to incorporate or omit from the model, demarcated date ranges, and other relevant parameters. Following thorough configuration, the system initiates the generation of optimal classifiers. Evaluation on a designated validation subset ensures the utmost efficiency. Ultimately, the top-performing model gets chosen, and Shap Values are utilized to furnish comprehensive explanations pertaining to significant determinants. Our intuitive platform showcases these discoveries chronologically, allowing the user to examine particular instances and concentrate on noteworthy predictor effects in greater detail.
![shap values](../assets/img/Dataswati/AlertShap.svg)

### Tools

- MongoDB as the main database 
- Python : pandas, LightGBM, scikit-learn, shap, optuna, mlflow, ..
- Airflow for scheduling and pipelining 
- Docker for packaging 
- VSCode for development

### My involvment 

As the lead for this project, I rolled up my sleeves and gave it a complete makeover to transform it into a fully functional tool. We worked hand in hand with our client, consistently refining elements and bolstering features to meet ever-evolving expectations. 
### Results and achievements

- Saved a floundering project by doing a total renovation, making sure it'll last for years to come.
- Connected with clients to tackle real issues they faced, leading to breakthrough improvements thanks to us!
- This module is one of the main selling argument for PowerOP because it can be used with only historical data (no need to implement a live connection)



