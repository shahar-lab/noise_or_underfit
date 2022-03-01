# noise (working_title)
git repo accompanying the project 

## Background 
Theory-driven computational modeling allows estimation of latent cognitive and neural variables.  
Nonetheless, studies have found that computational models can systematically fail to describe some individuals.  
Presumably two factors contribute to this shortcoming:  
1. Higher internal noise (stochasticity in behavior).
2. Deployment of different model (unknown to the researcher).  

However, when measuring behavior of individuals on cognitive task, these two factors are entangled and therefore hard to dissociate.  
Here we examine (in-silico) the use of advances in data-driven machine learning algorithms disentangled this two factors.  

## Dataset and objective
The dataset inclueded behavior of 500 artificial agent of 5 theoretical models (100 agent from each model):
1. Model-Free RL (MF). 
2. Model-Based RL (MB). 
3. Habitual model (habit). 
4. Win-Stay, Lose-Shift (WSLS). 
5. k-Dominant hand (kdh).  

Each agent was simulated on the reduce Two-Step task (TST) for 5 blocks containing 200 trials each. 
Post simulation we pretended that the true generative theoretical model of each agent is unknown and sought to ask if Recurrent neural network (RNN) and Logistic regression (LR),   
two models we considered as theory-independent models can help classify each agent underlying theoretical model. 

## Leave-one-block out cross-validation (LOOCV)
To test this we act as follow. At each round (5 in total) we assumed that all agents came from only one theoretical model and compared the fit (predictive accuracy) of the assumed theoretical model against the fit of RNN and LR. We adapted an Leave-one-block out cross-validation approach. were for each agent 

- <img src="https://latex.codecogs.com/gif.latex?O_t=\text { Onset event at time bin } t " /> 






![image](https://github.com/yoavger/noise_or_underfit/blob/main/plots/method.png)
![image](https://github.com/yoavger/noise_or_underfit/blob/main/plots/roc_0.png)
![image](https://github.com/yoavger/noise_or_underfit/blob/main/plots/bar_plot.png)
![image](https://github.com/yoavger/noise_or_underfit/blob/main/plots/noise_2.png)







