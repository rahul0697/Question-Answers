# Machine Learning & Deep Learning

## Table of contents

* [Machine Learning](#machine-learning)
   * [Table of contents](#table-of-contents)
   * [Covariance vs Correlation](#covariance-and-correlation)
   * [Cosine vs Euclidean Distance](#cosine-vs-euclidean-distance)
   * [Parametric Vs Non Parametric Classifier](#parametric-vs-non-parametric-classifier)
* [Deep Learning](#deep-learning)
  * [Table of contents](#table-of-contents)
  * [Time Distributed Layer](#time-distributed-layer)
  * [Parameters in  LSTM](#parameters-in-lstm)
  * [1D Convolution](#conv-1-D)
  
###  Covariance vs Correlation
- variance(x) =  
![varinace](https://latex.codecogs.com/gif.latex?%5Csum_%7Bi%3D0%7D%5E%7Bn%7D%5Cfrac%7B%28x-%5Cbar%7Bx%7D%29%5E2%7D%7Bn-1%7D)
- covariance(x,y) =  
![covariance](https://latex.codecogs.com/gif.latex?%5Csum_%7Bi%3D0%7D%5E%7Bn%7D%5Cfrac%7B%28x-%5Cbar%7Bx%7D%29%28y-%5Cbar%7By%7D%29%7D%7Bn-1%7D)
- Covariance shows trends between features of data: positive Trend(cov(x,y)>0), negative trend(cov(x,y)<0), No Trend(cov(x,y)=0)
- cov(x,y) >0 => with increase in x, y increases and vice versa. 
- cov(x,y) < 0 => with increase in x, y decreases and with increase in y x decreases
- cov(x,y) =0 => nothing can be said. No relationShip exists. with increase in x, y increases, decrease or remain Constant.
- Covariance is not easy to interpret, since we can not compare magnitude of covariance values.     
<p float="left">
  <img src="https://github.com/rahul0697/Question-Answers/blob/master/covarinace.jpeg" width="300"/> 
  <img src="https://github.com/rahul0697/Question-Answers/blob/master/Correlation1.jpeg" width="300"/>
  <img src="https://github.com/rahul0697/Question-Answers/blob/master/correlation2.jpeg" width="300"/>
</p>

      
### Cosine vs Euclidean Distance 
> Why is cosine similarity better in measuring similarity between vectors than Euclidean in Vector Space model? 
 - Euclidean distance is not a good measure of similarity in high dimension. 
 - Cosine similarity is generally used as a metric for measuring distance when the magnitude of the vectors does not matter. 
 - Cosine similarity is specialized in handling scale/length effects, like the word count of  same word in different document. 
 - [machine-learning-mastery](https://machinelearningmastery.com/parametric-and-nonparametric-machine-learning-algorithms/)
### Parametric vs Non Parametric Classifier
> Parametric Classifier : Decision Surface is known. Small dataset is not a problem here.
 - Linear Regression
 - Logistic Regression 
 - Perceptron  
> Non-Parametric Classifier : Decision surface is not known, we learn it from the data. Large Data -> better decision Surface  
- Deep Neural Network  
- SVM(Kernels)  
- KNN  
- Decision Tree  
### Time Distributed Layer
> https://machinelearningmastery.com/timedistributed-layer-for-long-short-term-memory-networks-in-python/

### Parameters in  LSTM
> https://stackoverflow.com/questions/38080035/how-to-calculate-the-number-of-parameters-of-an-lstm-network/56614978#56614978
### 1D Convolution

