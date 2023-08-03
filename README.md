**This repository is the code implementation for paper "Explainable Trajectory Representation Based on Dictionary Learning". The demo dataset is provided in File folder "dataset", by code in  "preprocess" you can transform the raw gps point format data into sequences of edges on roadmap, and code in  "matrix_method" can learn the optimal dictionary and trajectory  representation  simultaneously. All the code is in ipynb format. Enjoy ^_^**
# Abstract
Trajectory representation learning on a network provides us with 
great opportunities to understand vehicular traffic patterns and 
benefits numerous downstream applications. Existing approaches 
using classic machine learning or deep learning embed trajectories 
as dense vectors, which lack interpretability and are inefficient to 
store and analyze in downstream tasks. In this paper, an explainable 
trajectory representation learning framework based on dictionary 
learning is proposed. Given a collection of trajectories on a network, 
it extracts a compact dictionary of commonly used subpaths called 
“pathlets”, which optimally reconstruct each trajectory by simple 
concatenations. The resulting representation is naturally sparse 
and encodes strong spatial semantics. Theoretical analysis of our 
proposed algorithm is conducted to provide a probabilistic bound 
on the estimation error of the optimal dictionary. A hierarchical dic
tionary learning scheme is also proposed to ensure the algorithm’s 
scalability on large networks, leading to a multi-scale trajectory 
representation. Our framework is evaluated on two large-scale real
world taxi datasets. Compared to previous work, the dictionary 
learned by our method is more compact and has better reconstruc
tion rate for new trajectories. In addition, we also evaluated the 
learned representation on the travel time prediction task. The result 
shows that our method outperforms neural-network based methods 
by 4.7% in prediction accuracy while providing interpretability.