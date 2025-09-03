# Deciding Who’s Right or Wrong: An Analysis of AITA Subreddit Using Graph Networks

## Overview
This project explores the *Am I The A\*\*hole (AITA)* subreddit to understand what influences verdict outcomes.  
We combined **text analysis** with **graph network methods** to model conversations and predict whether posts were judged *NTA, YTA, ESH, or NAH*.  

## Data
- Source: Reddit’s AITA subreddit (scraped posts + comments)  
- Structure: Submission → comment tree → network graph  
- Labels: Verdict assigned to each post  

##  Methods
- **Text Features**: Sentiment analysis, keyword frequencies, basic NLP preprocessing  
- **Graph Features**:  
  - Degree-based metrics  
  - PageRank  
  - Shortest Path Analysis  
  - k-core decomposition  
  - Clustering coefficients & community detection  

- **Machine Learning**:  
  - Traditional ML models (LogReg, SVM, Random Forest) using combined text + graph features  
  - Experimented with PyTorch Geometric for graph embeddings  

## Results
- Graph features improved prediction performance compared to text alone  
- PageRank and degree-based metrics were especially informative in differentiating verdicts  

## Visualizations
- Network graphs of comment trees  
- Community structure detection  
- Feature importance plots from ML models  

## How to Run
1. Clone the repo  
   ```bash
   git clone https://github.com/Berlyb/Deciding-Who-s-Right-or-Wrong-An-analysis-of-AITA-subreddit-using-graph-networks.git
