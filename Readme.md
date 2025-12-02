# Spark Coding Practice – Preparation Guide

This guide explains how to search datasets on Kaggle, practice Spark using Python notebooks, and track progress with Git and GitHub.

---

## 1️⃣ Finding Datasets on Kaggle

Kaggle provides diverse datasets ideal for Spark learning.

### Steps:
1. Visit Kaggle → **Datasets**
2. Search using keywords:
   - big data, logs, transactions, retail, streaming, finance
3. Prefer medium–large datasets (100MB+ for Spark)
4. Download the datasets

---

## 2️⃣ Setting Up Spark Notebook Workspace

Choose any of the below for PySpark/Scala Spark practice:

- vscode
- Jupyter Notebook
- Google Colab (Install Spark runtime)

### Recommended Structure:
- create a folder structure in your local setup

spark-practice/
│
├── data/ # Kaggle datasets
├── notebooks/ # Spark notebooks
├── src/ # Reusable Spark code
└── README.md

---

## 🚀 3️⃣ Version Control Using Git & GitHub

Track changes to notebooks and scripts.

# 🛠️ How to Create a Repository in GitHub

Follow these steps to create and set up a new GitHub repository:

---

## 1️⃣ Sign In to GitHub

- Open: https://github.com  
- Log in with your account

---

## 2️⃣ Create a New Repository

1. Click the **+** icon in the top-right  
2. Select **New repository**
3. Fill in the details:
   - **Repository Name** → example: `spark-practice`
   - (Optional) **Description**
   - Choose **Public** (recommended for learning) or **Private**

---

🎉 Finally, click **Create repository** to finish!

### First-time Setup:

create a file with filename as ".gitignore" inside spark-practice folder
Inside the file write the below text to avoid pushing large dataset to git repo

data/*

1) Open spark-practice folder in vscode 
2) press (control + ~). It opens terminal or power shell based on your OS.
3) Enter the below commands to initialize a new repository locally, perform initial commit and push to remote repository.

```bash
git init
git remote add origin <your-repo-url>
git add .
git commit -m "Initial commit: Project structure + dataset added"
git push -u origin main

Updating Notebooks
Whenever you add new Spark logic:

bash
Copy code
git add notebooks/<filename>.ipynb
git commit -m "Enhanced: Added DataFrame operations practice"
git push

To avoid storing heavy data files, add a .gitignore:

powershell
Copy code
data/*
!data/README.md     # Keep placeholder file only
🧪 Suggested Learning Roadmap
Week	Focus Area	Example Practice Dataset
1	RDDs, Basic DF Operations	Retail sales logs
2	Joins, GroupBy, Window Functions	Stock time series
3	Spark SQL + UDFs	Movie ratings
4	MLlib Pipelines	E-commerce records
5	Structured Streaming	Clickstream / IoT events

Commit after each week:

bash
Copy code
git commit -m "Completed Week 2: Window queries"
🎯 Objectives of the Repo
Strengthen Spark data engineering skills

Build real-world data transformation notebooks

Maintain a clean, evolving Git history

