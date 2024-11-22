# Supervised Learning

## About this Project
This is a supervised learning project that uses 3 algorithms on two classification problems.
The 3 supervised algorithms are:
1. Neural Networks
2. Support Vector Machines
3. k-Nearest Neighbors

Different hyperparameters are explored for each algorithm. To see which ones exactly refer to the pdf explaining the
experiment in its entirety.

Scikit-learn (python3) is used to evaluate the algorithms.

## How to run this project
## 1. Prereqs
- Python3
- pip3
- conda
- jupyter notebook
- 
## 1. Setting up environment
- The data can be found here so no need to download it externally
- Navigate to the `supervised-learning` directory using `cd supervised-learning`
- Install conda (refer to https://conda.io/projects/conda/en/latest/user-guide/install/index.html for instructions)
- Set up virtual environment:
```
conda env create -f environment.yml
conda activate supervised_learning
```

## 2. Downloading data
- The data will already be in the box link in the data folder. 
- The first dataset is 'default_of_credit_card_clients.csv'
- The second dataset is 'phishing_dataset.csv'
- There is no need to navigate to the data folder as the jupyter notebooks will automatically access the necessary datasets

## 3. Directory Structure

├── data
│   ├── default_of_credit_card_clients.csv
│   └── phishing_dataset.csv
├── images
    ├── credit-knn
    ├── credit-nn
    ├── credit-svm
    ├── phishing-knn
    ├── phishing-nn
    └── phishing-svm
├── notebooks
    ├── default-credit-payment-KNN.ipynb
    ├── default-credit-payment-NN.ipynb
    ├── default-credit-payment-SVM.ipynb
    ├── phishing-KNN.ipynb
    ├── phishing-NN.ipynb
    └── phishing-SVM.ipynb
├── results
    ├── credit-knn
    ├── credit-nn
    ├── credit-svm
    ├── phishing-knn
    ├── phishing-nn
    └── phishing-svm
├── environment.yml
├── README.md

- data: holds the datasets
- images: holds 6 directories (1 for each algorithm per dataset) containing images/plots from the perspective notebook
- notebooks: holds the jupyter notebook files
- results: holds 6 directories for .txt files for statistics about each algorithm, written from the jupyter notebooks


## 3. Running the Notebooks/Algorithms/Experimments
### 3.1 Running the code
- Ensure that you complete the setup in section 1 and 2.
- Verify your conda environment is active. You should see (supervised_learning) at the beginning of your terminal line.
- From the `supervised-learning` directory launch Jupyter Notebook using the command `jupyter notebook`
- It should automatically open 'http://localhost:8888/tree' in your browser but if not navigate there
- From there navigate to the notebooks folder. This folder contains all 6 .ipynb files (1 for each algorithm on the 2 datasets)
- Open any notebook by double-clicking on it. (Note the process for running all the algorithms/notebooks is the same here on out)
  - To run the code, click 'Run' in the toolbar then in that drop down and select 'Run All Cells'
  - This will run all your cells and may take up to an hour+ depending on the algorithm and machine it's being run on
  - You can view the progress in the output cells (most cells have a %%time to show how long each cell took and so you know when it's done)
  - While it is running there will be an hour glass in Jupyter notebook tab. When it is done it will be a notebook icon
- Do this for all notebooks to run all 6 algorithms
- 
### 3.2 Viewing the results
The notebooks automatically save all text statistics to the results folder and all plots to the images folder, just
navigate to the respective directory to view them

## 4. References
- https://www.kaggle.com/datasets/akashkr/phishing-website-dataset/data
- https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients
