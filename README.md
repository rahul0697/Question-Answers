# Machine Learning & Deep Learning

## Table of contents

* [Machine Learning](#machine-learning)
   * [Table of contents](#table-of-contents)
   * [ROC  AUC](#roc-auc)
   * [Concave Convex](#concave-convex)
   * [Covariance vs Correlation](#covariance-and-correlation)
   * [Cosine vs Euclidean Distance](#cosine-vs-euclidean-distance)
   * [odds vs log odds](#odds-vs-log-odds)
   * [Parametric Vs Non Parametric Classifier](#parametric-vs-non-parametric-classifier)
   * [Discriminativ vs Generative Classifier](#discriminative-vs-generative-classifier)
   * [Central Limit Theorm](#central-limit-theorm)
* [Deep Learning](#deep-learning)
  * [Table of contents](#table-of-contents)
  * [Time Distributed Layer](#time-distributed-layer)
  * [Parameters in  LSTM](#parameters-in-lstm)
  * [1D Convolution](#conv-1-D)
  
  
###   ROC  AUC
<img src = "/ROC_AUC.jpeg"/>  


###   Concave Convex   
<img src = "/concave_convex.jpeg"/>
  
  
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
  <img src="https://github.com/rahul0697/Question-Answers/blob/master/covarinace.jpeg" /> 
  <img src="https://github.com/rahul0697/Question-Answers/blob/master/Correlation1.jpeg" />
  <img src="https://github.com/rahul0697/Question-Answers/blob/master/correlation2.jpeg" />
</p>

### odds vs log odds
odds =  
![odds](https://latex.codecogs.com/gif.latex?%5Cfrac%7B%5Ctextrm%7Bthe%20ratio%20of%20something%20happening%28i.e%20%7B%5Ccolor%7BGreen%7D%20Winning%20game%7D%29%7D%7D%20%7B%5Ctextrm%7B%7Bthe%20ratio%20of%20something%20not%20happening%28i.e%20%7B%5Ccolor%7BRed%7D%20Not%7D%20%7B%5Ccolor%7BGreen%7D%20Winning%20Game%7D%29%7D%7D%7D)  
> Suppose I won 5 games and lost 3 games. so odds in favour of winning = 5/3 = and odds in favour of lossing = 3/8  
> probability is different than odds.     
probability =   
![probability](https://latex.codecogs.com/gif.latex?%5Cfrac%7B%5Ctextrm%7Bthe%20ratio%20of%20something%20happening%28i.e%20%7B%5Ccolor%7BGreen%7D%20Winning%20game%7D%29%7D%7D%20%7B%5Ctextrm%7B%7Bthe%20ratio%20of%20something%20not%20happening%28i.e%20%7B%5Ccolor%7BRed%7D%20Loosing%7D%20&plus;%20%7B%5Ccolor%7BGreen%7D%20winning%20Game%7D%29%7D%7D%7D)      
> pr(winning game) = 5/8 and pr(loosing game) = 3/8    
> odds in favour of winning = pr(winning)/pr(loosing) = pr(winning)/(1-pr(winning)) = 5/8    
#### odds:  
>Odds against Winning = 3/8, 8/16 , 5/32 etc => odds against winning will have a range 0 to 1.   
>Odds in favour of Winning = 8/3, 16/8, 32/5 etc => odds in favour of winning will have a range from 1 to infinity.   
>Odds are not Symmetric, since 8/3 and 3/8 has different range. 
#### Log odds:
> Log odds against winning = log(3/8), log(8/16), log(5/32)   
> Log odds in favour of winning  = log(8/3), log(16/8), log(32/5)  
>Since log(3/8) = -log(8/3) =>Symmetric in both range  

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

### Discriminativa vs Geneartive Classifier
| Discriminative Classifier  | Generative Classifier |
| ------------- | ------------- |
|  Discriminative models learn the (hard or soft) boundary between classes. | Generative models model the distribution of individual classes |
| SVM, Neural Network, Decision Trees, Linear Regression, Logistic Regression | Naive Bayies, GMM, HMM  |

### Central Limit Theorm
Definition - The central limit theorem says that the probability distribution of the average will closely approximate a normal distribution.  
Whatever distribution you choose, sample mean will tends towards normal distribution.
>To apply central limit theorm, you should be able to calculate mean of samples.
>Cauchy Distribution's mean is undefined, so its difficult to define central limit theorm in this case.

### Time Distributed Layer
> https://machinelearningmastery.com/timedistributed-layer-for-long-short-term-memory-networks-in-python/

### Parameters in  LSTM
> https://stackoverflow.com/questions/38080035/how-to-calculate-the-number-of-parameters-of-an-lstm-network/56614978#56614978
### 1D Convolution

