# Project 4: Causal Inference

### [Project Description](doc/project4_desc.md)

Term: Fall 2020

+ Team #02
+ Projec title: Causal Inference Algorithms Evaluation 
+ Team members (in alphabetical order)
	+ Siyu Duan (sd3329)
	+ Yotam Segal (ys3114)
	+ Yuwei Tong (yt2713)
	+ Hanyi Wang (hw2744)
	+ Lingjia Zhang (lz2720) 
+ Project summary: In this project, we implemented and compared different algorithms for Causal Inference on both low dimension data and high dimension data. We compared the following algorithms using L1 penalized logistic regression to estimate propensity score:
	+ Propensity Matching (linear PS)
	+ Doubly Robust Estimation
	+ Regression Estimate
	
We evaluated different methods by accuracy (difference between our estimated ATE and real ATE) and running time, and got following results:

Method | Data Type | run_time | ATE | Accuracy   
--- | --- | --- | --- | ---  
regression_estimate | lowDim| 6.618 | 2.532 | 98.7%    
regression_estimate | highDim | 4.319 | -2.951 | 98.4%
DRE | lowDim | 0.115 | 2.645 | 94.2%
DRE | highDim | 0.438 | -3.082 | 97.3%
PSM | lowDim | 3.323 | 2.586 | 96.5%
PSM | highDim | 23.656 | -3.069 | 97.7%
     


	
**Contribution statement**: All team members approve our work presented in this GitHub repository including this contributions statement. 

Siyu Duan:  Implemented L1 Panalized Logistic Regression and Doubly Robust Estimation to estimate propensity scores and ATE. Created shared doc in the team, scheduled meetings through out the project cycle, and made sure teammembers were on track of assigned tasks.  She was a presenter of this project. 

Yotam Segal: Implemented Regression Estimate Algorithms for ATE.  Consolidated codes and created the final version of the project. Yotam cross-validated and fixed team members' codes while improving their efficiency and readability. Yotam also created the communication channel we used in building this project. 

Yuwei Tong: Implemented L1 Panalized Logistic Regression, Propensity Matching, and Linear Propensity Score algorithms to estimate propensity scores and ATE. 

Hanyi Wang: Helped proof-read other teammates' code. 

Lingjia Zhang: Implemented L1 Panalized Logistic Regression and Doubly Robust Estimation to estimate propensity scores and ATE. 

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
