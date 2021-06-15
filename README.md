# Awesome Anomaly Detection
I forked this repo to have list of options for stall-based anomoly detection.


## Classical Method
- ~[Isolation Forest](https://cs.nju.edu.cn/zhouzh/zhouzh.files/publication/icdm08b.pdf)~ - ICDM 2008.
  - Implemented
- ~[LOF: Identifying Density-Based Local Outliers](http://www.dbs.ifi.lmu.de/Publikationen/Papers/LOF.pdf)~ - SIGMOD 2000.
  - Implemented   

- ~[Extended Isolation Forest](http://matias-ck.com/files/papers/Extended_Isolation_Forest.pdf)~
  - Implemented
- ~[Robust Random Cut Forest Based Anomaly Detection On Streams](http://proceedings.mlr.press/v48/guha16.pdf)~
  - Same as EIF?   

- ~[Support Vector Method for Novelty Detection](https://papers.nips.cc/paper/1723-support-vector-method-for-novelty-detection.pdf)~ - NIPS 2000
  - Implemented
### One-Class Classification

- ~[One-Class SVMs for Document Classification](http://www.jmlr.org/papers/volume2/manevitz01a/manevitz01a.pdf)~ - JMLR 2001. 
  - Implemented   

- [Support Vector Data Description](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.100.1425&rep=rep1&type=pdf) 

- [Can I Trust My One-Class Classification?](http://www.ipb.uni-bonn.de/pdfs/Mack2014Can.pdf)

- [Efficient Anomaly Detection via Matrix Sketching](https://arxiv.org/pdf/1804.03065.pdf) - NIPS 2018
  - useful for the anomalous command project for Brian?  
  - No Arxiv code implementation


### PCA-based

- [robust deep and inductive anomaly detection](https://arxiv.org/abs/1704.06743) - ECML PKDD 2017
  - Has promise.  
  - Code provided (https://github.com/raghavchalapathy/rcae) 
  - Test cases are images, so we need to adapt for vector/scalar inputs. 

- [A loss framework for calibrated anomaly detection](https://papers.nips.cc/paper/7422-a-loss-framework-for-calibrated-anomaly-detection.pdf) - NIPS 2018


### Clustering

- [A Practical Algorithm for Distributed Clustering and Outlier Detection](https://arxiv.org/pdf/1805.09495.pdf) - NIPS 2018

### Correlation

- [Detecting Multiple Periods and Periodic Patterns in Event Time Sequences](http://chaozhang.org/papers/cikm17a.pdf) - CIKM 2017.

### Ranking

- ~[ranking causal anomalies via temporal and dynamical analysis on vanishing correlations](https://www.kdd.org/kdd2016/papers/files/rfp0445-chengAemb.pdf) - KDD 2016.~
  - Works on Graph data, not scalar.

### Streaming

- ~[MIDAS: Microcluster-Based Detector of Anomalies in Edge Streams](https://www.comp.nus.edu.sg/~sbhatia/assets/pdf/midas.pdf) - AAAI 2020.~ 
  - We do not have graph-data.


## Deep Learning Method

### Generative Methods
- [Variational Autoencoder based Anomaly Detection using Reconstruction Probability](http://dm.snu.ac.kr/static/docs/TR/SNUDM-TR-2015-03.pdf)  

#### Auto-encoder

- [Learning sparse representation with variational auto-encoder for anomaly detection](https://ieeexplore.ieee.org/document/8386760/)

- [Anomaly Detection with Robust Deep Autoencoders](http://dl.acm.org/authorize?N33358) - KDD 2017.

- [DEEP AUTOENCODING GAUSSIAN MIXTURE MODEL FOR UNSUPERVISED ANOMALY DETECTION](https://www.cs.ucsb.edu/~bzong/doc/iclr18-dagmm.pdf) - ICLR 2018.

- [Generative Probabilistic Novelty Detection with Adversarial Autoencoders](https://papers.nips.cc/paper/7915-generative-probabilistic-novelty-detection-with-adversarial-autoencoders.pdf) - NIPS 2018
#### Variational Auto-encoder

- ~[Multidimensional Time Series Anomaly Detection: A GRU-based Gaussian Mixture Variational Autoencoder Approach](http://proceedings.mlr.press/v95/guo18a/guo18a.pdf)~ - ACML 2018
  - No code?

- [A Multimodel Anomaly Detector for Robot-Assisted Feeding Using an LSTM-based Variational Autoencoder](https://arxiv.org/pdf/1711.00614.pdf) - IEEE Robotics and Automation Letters 2018. 

#### GAN based

- [Unsupervised Anomaly Detection with Generative Adversarial Networks to Guide Marker Discovery](https://arxiv.org/pdf/1703.05921.pdf) - IPMI 2017.

- [Efficient-GAN-Based Anomaly Detection](https://github.com/houssamzenati/Efficient-GAN-Anomaly-Detection) ICLR Workshop 2018.

- [Anomaly detection with generative adversarial networks](https://openreview.net/pdf?id=S1EfylZ0Z) - Reject by ICLR 2018, but was used as baseline method in recent published NIPS paper.

### Hypersphereical Learning

- [Anomaly Detection in Dynamic Networks using Multi-view Time-Series Hypersphere Learning](https://dl.acm.org/citation.cfm?id=3132964) - CIKM 2017.

- [Deep into Hypersphere: Robust and Unsupervised Anomaly Discovery in Dynamic Networks](https://www.ijcai.org/proceedings/2018/0378.pdf) - IJCAI 2018.

### One-Class Classification

- [High-dimensional and large-scale anomaly detection using a linear one-class SVM with deep learning](https://www.sciencedirect.com/science/article/abs/pii/S0031320316300267) - Pattern Recognition 2018.

- [Optimal single-class classification strategies](https://papers.nips.cc/paper/2987-optimal-single-class-classification-strategies.pdf) - NIPS 2007.


- [Deep One-Class Classification](http://proceedings.mlr.press/v80/ruff18a/ruff18a.pdf) - ICML 2018.

- [Deep Semi-Supervised Anomaly Detection](https://openreview.net/forum?id=HkgH0TEYwH) - ICLR 2020.
  - TE: 5/25 Try this one first ! 

- [Simple and Effective Prevention of Mode Collapse in Deep One-Class Classification](https://arxiv.org/pdf/2001.08873.pdf) - IJCNN 2021

- [Explainable Deep One-Class Classification](https://openreview.net/forum?id=A5VV3UyIQz) ICLR 2021.

- [Learning and Evaluating Representation for Deep One-Class Classification](https://openreview.net/pdf?id=HCSgyPUfeDj) ICLR 2021.

### Energy-based

- [Deep structured energy based models for anomaly detection](https://arxiv.org/pdf/1605.07717.pdf) - ICML 2016

### Time series

- [A Generalized Student-t Based Approach to Mixed-Type Anomaly Detection](http://www.nvc.cs.vt.edu/~ctlu/Publication/2013/AAAI-Lu-2013.pdf) - AAAI 2013

- [Stochastic Online Anomaly Analysis for Streaming Time Series](https://www.ijcai.org/proceedings/2017/0445.pdf) - IJCAI 2017

- [Long short term memory networks for anmomaly detection in time series](https://www.elen.ucl.ac.be/Proceedings/esann/esannpdf/es2015-56.pdf)

- [LSTM-based Encoder-Decoder for Multi-sensor Anomaly Detection](https://arxiv.org/pdf/1607.00148.pdf) - ICML 2016 Workshop.

### Interpretation

- [Contextual Outlier Interpretation](https://www.ijcai.org/proceedings/2018/0341.pdf) -IJCAI 2018

### Evaulation Metrics

- [Precision and Recall for Time Series](http://papers.nips.cc/paper/7462-precision-and-recall-for-time-series.pdf) - NIPS 2018

### Geometric transformation

- [Deep Anomaly Detection Using Geometric Transformations](https://arxiv.org/pdf/1805.10917.pdf) - NIPS 2018


### FeedBack
- [Incorporating Feedback into Tree-based Anomaly Detection](https://github.com/ai/size-limit) - KDD 2017 Workshop on Interactive Data Exploration and Analytics.

- [Feedback-Guided Anomaly Discovery via Online Optimization](http://web.engr.oregonstate.edu/~afern/papers/kdd18-siddiqui.pdf) - KDD 2018.



## Anomaly Detection Applications

### KPI
- [Unsupervised Anomaly Detection via Variational Auto-Encoder for Seasonal KPIs in Web Applications](https://arxiv.org/pdf/1802.03903) - WWW 2018.
- [Unsupervised Online Anomaly Detection with Parameter Adaptation for KPI Abrupt Changes](https://www.researchgate.net/publication/338205097_Unsupervised_Online_Anomaly_Detection_with_Parameter_Adaptation_for_KPI_Abrupt_Changes) - TNSM 2019.
### Log

- [Loganomaly: Unsupervised detection of sequential and quantitative anomalies in unstructured logs](https://netman.aiops.org/wp-content/uploads/2019/07/LogAnomaly.pdf) -IJCAI 2019
- [Robust log-based anomaly detection on unstable log data](https://netman.aiops.org/~peidan/ANM2020/6.LogAnomalyDetection/LectureCoverage/2019FSE_LogRobust.pdf) - FSE 2019
- [Prefix: Switch failure prediction in datacenter networks](https://dl.acm.org/doi/abs/10.1145/3179405) -SIGMETRICS 2018
- [DeepLog: Anomaly Detection and Diagnosis from System Logs through Deep Learning](https://acmccs.github.io/papers/p1285-duA.pdf) - CCS 2017
- [Mining Invariants from Logs for System Problem Detection](https://www.usenix.org/legacy/event/atc10/tech/slides/lou.pdf) - USENIX 2010


## Survey

- ~[Anomaly detection in dynamic networks: a survey](https://onlinelibrary.wiley.com/doi/pdf/10.1002/wics.1347)~
  - We do not have graph data 

- ~[Anomaly Detection : A Survey](http://cucis.ece.northwestern.edu/projects/DMS/publications/AnomalyDetection.pdf)~
  - Rather old info. Specifically the Neural approaches.
- [A Survey of Recent Trends in One Class Classification](https://link.springer.com/chapter/10.1007/978-3-642-17080-5_21) 

- [A survey on unsupervised outlier detection in high‐dimensional numerical data](https://onlinelibrary.wiley.com/doi/abs/10.1002/sam.11161)










