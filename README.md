# 기부단체 추천 알고리즘 

🏆**Patent No. 4020230231908 registered on December 20, 2023**

🏆**2023 GIST startup night**

## 📂Overview

<table>
  <tr>
    <td style="text-align:center;"><img src="images/005.png" alt="Image 1" width="300"/></td>
    <td style="text-align:center;"><img src="images/008.png" alt="Image 2" width="300"/></td>
  </tr>
</table>

🌐[1004-finder|천사발굴단 on *instagram*](https://www.instagram.com/1004_finder/)

### What it does

This project implements an algorithm to recommend suitable donation organizations to donors. It effectively clusters and recommends donation organizations. The system leverages machine learning to recommend donation organizations based on donors' preferences, aiming to improve accessibility for small and new donation organizations.

### Why we used this technology

The system uses machine learning to analyze donors' donation preferences and effectively cluster donation organizations to recommend the most suitable ones. **This enhances donor satisfaction and improves the transparency and accessibility of donation organizations.** 



## 📂Methodology

This project collects and preprocesses data from donors and donation organizations to implement an algorithm that clusters and recommends donation organizations. Clustering is based on the characteristics of donation organizations, and the recommendation algorithm uses K-NN (K-nearest neighbor search).

### Technical Details

#### Data Preprocessing

This stage involves collecting and preprocessing donor and donation organization data.

- **Donor Data Collection**: Collects donor preference data.
- **Donor Data Preprocessing**: Cleans and transforms collected donor data into the required format. Donor data consists of responses to donation-related questions.
- **Donation Organization Data Collection**: Gathers various characteristic information of donation organizations, including the number of employees, total assets, liabilities, net assets, business revenue, etc.
- **Donation Organization Data Preprocessing**: Removes duplicate data and processes data into a format suitable for clustering. Extracts characteristic information of donation organizations, removes redundancies, and transforms data into a dataset ready for clustering.

#### Donation Organization Recommendation

This stage analyzes donor data to recommend suitable donation organizations.

- **Donation Organization Clustering**: Analyzes donation organization data and groups donation organizations into multiple clusters. Organizations with similar characteristics belong to the same cluster.
- **Donation Organization Recommendation**: Recommends suitable donation organizations based on donor data. Uses the K-NN algorithm to recommend donation organizations belonging to clusters most similar to the donor.



## 📂Requirement

### Dependencies

- Python 3.x
- pandas
- scikit-learn
- numpy

### Setup

1. Install Python 3.x
2. Install required packages:

```
sh
코드 복사
pip install pandas scikit-learn numpy
```



## 📂Implement

### Demo

1. Prepare donor and donation organization data.
2. Run the algorithm with the following command:

```
sh
코드 복사
python donation_recommendation.py
```

### Screenshot

![image-20240519221354172](images/1.png)

![image-20240519221338881](images/2.png)



## 📂Hierarchy

```
project-root/
├── clustering.py
├── dim_reduction.py
├── features.py
├── parameters.txt
├── test.py
├── to_numpy.py
├── tree.dot
├── unsupervised-random-forest/
│   ├── __pycache__/
│   ├── notebooks/
│   │   ├── README.md
│   │   ├── sklearn_comparison.png
│   │   ├── synthetic_data.py
│   │   ├── unsupervised_random_forest.py
├── attributes.txt
├── more_than_10.txt
├── non_numeric.txt
├── numeric.txt
├── requirements.txt
├── statistics.txt
├── Result/
│   ├── 4/
│   ├── 5/
├── feature_plots/
│   ├── Discrete/
│   ├── Numeric/
├── src/
│   ├── __pycache__/
│   ├── 2021_data_analysis.py
│   ├── clustering.py
│   ├── dim_reduction.py
│   ├── features.py
│   ├── parameters.txt
│   ├── test.py
│   ├── to_numpy.py
│   ├── tree.dot
```



## 📂Contributors

- Junmyung Lee
- Jangwon Hwang
- Jaehee Lee

