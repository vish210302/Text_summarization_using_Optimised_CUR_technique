# Text Summarization Using Optimized CUR Matrix Decomposition Technique
## Overview
This project implements text summarization techniques based on CUR matrix decomposition, a method for low-rank approximation of data matrices. CUR decomposition is known for its interpretability, as it approximates the data matrix using subsets of its original rows and columns. This project applies two CUR-based approaches designed to improve efficiency while maintaining accuracy.

## Approaches
### Discrete Empirical Interpolation Method (DEIM)

The first approach utilizes the Discrete Empirical Interpolation Method (DEIM), as detailed by Sorensen and Embree in their paper **A DEIM Induced CUR Factorization."** DEIM selects rows and columns from the matrix using interpolatory projectors, which efficiently identify important indices for summarization.
### Fast Deterministic CUR Decomposition

The second approach employs a fast deterministic CUR decomposition method introduced by Yashutoshi Ida in **"Fast Deterministic CUR Matrix Decomposition with Accuracy Assurance.**" This method improves upon the coordinate descent approach by avoiding unnecessary updates. It evaluates optimality conditions to efficiently update parameters, thus speeding up the CUR decomposition process while ensuring accuracy.

## Evaluation
The performance of the implemented methods has been evaluated based on two criteria: precision,recall,F1- score and computation time. The following tables summarize the results:

### TABLE I. 	EVALUATION TABLE
![image](https://github.com/user-attachments/assets/221c952c-6117-4f7a-b53c-7c41e2ae43aa)
### TABLE II. 	TIME COMPARISON TABLE
![image](https://github.com/user-attachments/assets/b8ca397d-d8df-4220-bbca-61468fe8329d)

Evaluation results indicate that Precision, Recall, and F1-score remain consistent between DEIM and the Faster Deterministic Approach, indicating comparable performance while ensuring accuracy post-optimization with the latter. A comparative analysis of computational time reveals that the Faster Deterministic Approach significantly outperforms DEIM, demonstrating substantially reduced processing time.

### Purpose
This implementation aims to provide a practical and efficient solution for text summarization using advanced CUR matrix decomposition techniques. The methods included in this project are based on established research and are designed to enhance performance in terms of both speed and accuracy.

### Project Notes
This project is a research paper implementation of the CUR matrix decomposition methods outlined in the referenced papers.
The code provided replicates the approaches discussed in the research, focusing on their application to text summarization.








