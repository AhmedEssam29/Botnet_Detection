# Botnet Detection

Botnet detection is an important element of any organization’s cybersecurity program in order to prevent data theft, network disruption, reputational damage, and regulatory penalties.


## Table of content
1. [Data](#Data)
2. [EDA](#EDA)
3. [Models](#Models)
4. [Detect Mirai Attack](#Detect#Mirai#Attack)
5. [Detect GAFGYT Attack](#Detect#GAFGYT#Attack)



## DATA
- This dataset addresses the lack of public botnet datasets, especially for the IoT. It suggests real traffic data, gathered from 9 commercial IoT devices authentically infected by Mirai and BASHLITE.

- we aimed at distinguishing between benign and Malicious traffic data by means of anomaly detection techniques.
## EDA
1. Data Distribution:
- Class Distribution shows data Unbalance:
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture1.png?raw=true)
- Class Distribution after undersampling:
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture2.png?raw=true)

2. Feature Distribution:
- **In this section**, we spotlight the distribution patterns of two pivotal features within our dataset.
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture3.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture4.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture5.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture6.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture7.png?raw=true)



- Notably, both features reveal noticeable skewness, signaling departure from a symmetrical distribution.
- This pattern is consistent across most features in the dataset.

3. Data Before and after **Label Encoding**
- Before:
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture8.png?raw=true)
- After:
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture9.png?raw=true)

4. Measuring Features Importance and selecting the top 50 features using **extratree classifier algorithm **:
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture10.png?raw=true)

## Models:
- I tested 6 different models to check the best one performance:
This is a comparison of the six models we implemented, and given the size of our dataset, we have chosen to utilize the Neural Network model.

![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture11.jpg?raw=true)

- The learning curve for loss and accuracy:
Accuracy curve:
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture12.png?raw=true)

Loss curve:  
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture13.png?raw=true)

- The confusion matrices of Neural network on validation and test set:
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture14.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture15.png?raw=true)


## Detect Mirai Attack:
Data distribution and feature selection for Mirai Attacks 
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture16.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture17.png?raw=true)


The learning curve for loss and accuracy for Mirai Attacks  
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture18.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture19.png?raw=true)


The confusion matrices of Neural network on validation and test set for Mirai Attacks
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture20.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture21.png?raw=true)

## Detect GAFGYT Attack
Data distribution and feature selection for GAFGYT Attacks 
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture22.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture23.png?raw=true)


The learning curve for loss and accuracy for GAFGYT Attacks  
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture24.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture25.png?raw=true)

The confusion matrices of Neural network on validation and test set for GAFGYT Attacks
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture26.png?raw=true)
![alt text](https://github.com/AhmedEssam29/Botnet_Detection/blob/main/imp/Picture27.png?raw=true)

## Future Work:

As the landscape of cyber threats continually evolves, it is imperative to ensure that our botnet detection models remain agile and up to date. The proactive integration of new threat intelligence, continuous learning mechanisms, and regular model updates is crucial in staying ahead of emerging attack vectors. By embracing a dynamic and adaptive approach, we can fortify our defenses, effectively identify novel attack patterns, and maintain a resilient security posture against the ever-changing landscape of botnet activities.



