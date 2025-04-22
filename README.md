# CX-4240
```
Group 18
Serena Yin, Cyra Alesha, Nadia Bozeman, Sophie Hollowell

This is the repository for all the code and materials for Group 18's CX 4240 Project

Structure
├── Datasets/
│   ├── Social Impact Bonds Data/        # Folder with all original data downloaded from the Indigo Impact Bond Dataset curated by the Government Outcomes Lab at the University of Oxford
│   ├── Synthetic Data/                  # Folder with the synthetic data supplemented by ChatGPT
│   │   ├── Structured_Projects_Data.csv
│   │   ├── Structured_Investments.csv
│   │   ├── Structured_Outcome_Metrics.csv
│   │   ├── Structured_Outcome_Payments.csv
├── Models/
|   ├── SIB_Success_Prediction.ipynb     # Notebook with models to predict the success of a Social Impact Bond
|   ├── Final Model - IRR.ipynb          # Notebook with models to predict the Internal Rate of Return of a Social Impact Bond
|   ├── CX4240_Project_Final_Exploratory_Models.ipynb    # Notebook with further models to explore what enriching the dataset in the future may look like
├── CX 4240 Presentation.pdf             # PDF of presentation slides
├── Final Report.pdf                     # PDF of final report
```

```
SIB_Success_Prediction.ipynb
This notebook explores the predictive modeling of Social Impact Bond (SIB) project outcomes. The goal is to estimate financial metrics like Success Probability based on pre-investment features, and simulate decision-making strategies for investors.

Requirements to run: 
├── Python 3.x
├── pandas, numpy, matplotlib, seaborn
├── scikit-learn
├── xgboost
```

```
Final Model - IRR.ipynb
This notebook explores the predictive mdoeling of Social Impact Bond (SIB) Internal Rate of Returns. The goal is to estimate the Internal Rate of Return based on pre-investment features, and simulate decision-making strategies for investors.

Requirements to run: 
├── Python 3.x
├── pandas, numpy, matplotlib, seaborn
├── scikit-learn
├── xgboost
```

```
CX4240_Project_Final_Exploratory_Models.ipynb
This notebook extends the predictive modeling of Social Impact Bond (SIB) outcomes by introducing and forecasting the IRR Achieved Ratio—a continuous metric representing how well a project performed relative to its target return. In addition to estimating success probability, the goal is to enrich the dataset and provide investors with deeper insights into return quality, enabling more informed, risk-adjusted decision-making strategies based on pre-investment features.

Requirements to Run:
├── Python 3.11 or lower
├── pandas, numpy, matplotlib, seaborn
├── scikit-learn
├── tensorflow

## Accessing & Reading the Files Successfully
In the notebook, when importing the datasets from the CSV files, you might need to change the location to successfully load them. Currently, they point to a relative path to a folder named "new synth data". If this not the case for you, please adjust the path as necessary.

If running this notebook in Colab, you can directly upload the synthetic data files provide and simply point to the CSV file name!

## Environment Setup
Because we use tensorflow to create our MLP models and tensorflow currently does not support more recent versions of Python (i.e. 3.12), it might be necessary for you to create a virtual environment to run this notebook.

If running this notebook in Colab, you can check the virtual environment using the following line:
├── !python3 --version
If the line returns Python 3.11.12 or lower, you should have no issue and can run the notebook as is!

If running this notebook in VSCode and you are running the notebook with a Kernel of Python 3.12 or higher, tensorflow might not be supported. You can check the version in terminal with the following line:
├── python --version

I used a Conda Kernel in VSCode, so here are instructions for creating a virtual environment witn Conda if necessary to support tensorflow:
  1. Open Terminal (View Tab -> Terminal or Ctrl/Cmd + `)
  2. Run the following line: conda create --name tf-env python=3.10
  3. Type y to proceed
  4. Run the following line: conda activate tf-env
Once successfully created, this should also show up as one of the available Kernels to select in the top right corner in VSCode.
```
