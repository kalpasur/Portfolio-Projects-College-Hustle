# College Hustle — Portfolio Projects

A collection of academic, DataCamp, and practice projects completed while learning data analytics, machine learning, deep learning, and Python. Each section explains the problem, approach, and the best file to open first.

> **How to use this README:** Select **Open notebook** to view a Jupyter notebook on GitHub, or **Run the project** to open the main Python entry point. Notebooks that use local datasets may need to be downloaded or run from their project folder so relative paths work.

## Project Index

| # | Project | Area | Start here |
|---|---|---|---|
| 1 | [A/B Testing with Cookie Cats](#1-ab-testing-with-cookie-cats) | Experiment analysis, retention | [Open notebook](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/B%20Testing%20with%20Cookie%20Cats/notebook.ipynb) |
| 2 | [Data Analytics Workspace Archive](#2-data-analytics-workspace-archive) | Data analysis | [Open notebook](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/DC%20Workspace%20Archieve/notebook.ipynb) |
| 3 | [Event Venue Ramp Prediction](#3-event-venue-ramp-prediction) | Data science, classification | [Open notebook](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Datacamp%20Data%20Scientist%20Certification/Certification_Workspace/notebook.ipynb) |
| 4 | [Dog and Pet Image Classifier](#4-dog-and-pet-image-classifier) | Computer vision, CNNs | [Run project](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Dog%20Classifier/check_images.py) |
| 5 | [Insurance Claim Predictor — Assessment Files](#5-insurance-claim-predictor--assessment-files) | Insurance data, predictive analytics | [Open project folder](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/tree/main/Insurance%20Claim%20Predictor) |
| 6 | [Name Game: Gender Prediction from Names](#6-name-game-gender-prediction-from-names) | Fuzzy matching, data analysis | [Open notebook](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Name%20Game%20Gender%20Prediction%20using%20Sound/notebook.ipynb) |
| 7 | [Naïve Bees — Image Dataset](#7-naïve-bees--image-dataset) | Deep learning, image classification | [Open project folder](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/tree/main/Na%C3%AFve%20Bees%20Deep%20Learning%20with%20Images) |

---

## 1. A/B Testing with Cookie Cats

**Goal:** Investigate whether moving the first in-game gate from level 30 to level 40 affects player engagement and retention in the mobile puzzle game *Cookie Cats*.

**What the notebook does**
- Explores an A/B test involving 90,189 players assigned to the level-30 or level-40 gate group.
- Compares game-round activity and 1-day and 7-day player retention.
- Uses bootstrap resampling to assess uncertainty in the difference between groups.
- Interprets the results to support a product decision about gate placement.

**Tools:** Python, pandas, data visualization, A/B testing, bootstrap analysis.

**Files**
- [Open the Jupyter notebook](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/B%20Testing%20with%20Cookie%20Cats/notebook.ipynb)
- [View the dataset — cookie_cats.csv](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/B%20Testing%20with%20Cookie%20Cats/datasets/cookie_cats.csv)

**Takeaway:** The notebook's analysis reports higher 1-day and 7-day retention for the level-30 group than for the level-40 group. The notebook contains the calculations and plots supporting that conclusion.

## 2. Data Analytics Workspace Archive

**Goal:** Preserve a data-analysis workspace and its associated task material.

The folder contains a Jupyter notebook, an Indian stock-market spreadsheet, a data analytics task PDF, and an image illustrating missing values. This section is documented as a workspace archive rather than claiming a specific model or result that is not clearly described by the available file names.

**Tools / materials:** Jupyter Notebook, spreadsheet data, data-quality inspection.

**Files**
- [Open the Jupyter notebook](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/DC%20Workspace%20Archieve/notebook.ipynb)
- [Indian stock-market spreadsheet](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/DC%20Workspace%20Archieve/Data%20Analytics-%20indian%20stock%20market%20final%20sheet.xlsx)
- [Data analytics task PDF](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/DC%20Workspace%20Archieve/Data%20analytics%20Task.pdf)
- [Missing-values image](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/DC%20Workspace%20Archieve/missing_values.jpeg)

**Execution note:** Open the notebook first. Some archived workspaces depend on local files and may require the dataset paths to be adjusted when running outside the original environment.

## 3. Event Venue Ramp Prediction

**Goal:** Analyze event-venue information and predict whether a venue has a ramp, a feature relevant to wheelchair accessibility.

**What the project contains**
- A notebook for the analysis and prediction workflow.
- An event-venue dataset.
- A saved prediction model and supporting visualizations / model artifacts.
- A presentation titled *Analysis and Prediction of Wheather event venue has a ramp*.

**Tools / methods:** Python, pandas, machine learning, classification, feature-importance analysis. The saved artifacts include a Keras H5 model and a model.json file.

**Files**
- [Open the Jupyter notebook](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Datacamp%20Data%20Scientist%20Certification/Certification_Workspace/notebook.ipynb)
- [View the event-venues dataset](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Datacamp%20Data%20Scientist%20Certification/Certification_Workspace/data/event_venues.csv)
- [View the project presentation](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Datacamp%20Data%20Scientist%20Certification/Analysis%20and%20Prediction%20of%20Wheather%20event%20venue%20has%20a%20ramp.pptx)
- [Feature-importance image](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Datacamp%20Data%20Scientist%20Certification/Certification_Workspace/Feature_importance.png)

**Execution note:** Start with the notebook; it is the main documented workflow. Re-running it may require installing the notebook's dependencies and keeping the relative dataset path intact.

## 4. Dog and Pet Image Classifier

**Goal:** Classify images with pretrained convolutional neural networks, compare predictions with labels inferred from image filenames, and evaluate how well the models distinguish dogs from other pets and objects.

**What the Python workflow does**
- Extracts pet labels from image filenames.
- Runs image classification with pretrained AlexNet, VGG, or ResNet models.
- Compares predicted labels with the supplied labels.
- Marks whether the actual and predicted classes are dogs and calculates summary statistics.
- Includes sample pet images and separate uploaded-image examples.

**Tools:** Python, PyTorch / torchvision, PIL, pretrained CNNs, image classification.

**Files**
- **Main entry point:** [check_images.py](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Dog%20Classifier/check_images.py)
- [Image classification comparison](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Dog%20Classifier/classify_images.py)
- [Pretrained model wrapper](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Dog%20Classifier/classifier.py)
- [Extract labels from filenames](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Dog%20Classifier/get_pet_labels.py)
- [Calculate evaluation statistics](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Dog%20Classifier/calculates_results_stats.py)
- [Adjust results for dog / non-dog labels](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Dog%20Classifier/adjust_results4_isadog.py)

**Run it:** Open a terminal in the Dog Classifier folder and run:

    python check_images.py

Check the script's command-line arguments and ensure its Python dependencies and image files are available. The classifier loads pretrained model weights depending on the installed PyTorch / torchvision version.

## 5. Insurance Claim Predictor — Assessment Files

**Goal / context:** This folder groups the data and assessment brief for an insurance-claim prediction exercise.

**Included files**
- [Employee data](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Insurance%20Claim%20Predictor/Dataset/employee_data.csv)
- [Insurance data](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Insurance%20Claim%20Predictor/Dataset/insurance_data.csv)
- [Vendor data](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Insurance%20Claim%20Predictor/Dataset/vendor_data.csv)
- [Python assessment brief (PDF)](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Insurance%20Claim%20Predictor/Python%20Assessment.pdf)

**Current limitation:** The repository folder contains the datasets and assessment PDF, but no Python entry-point script or notebook is currently included in the tracked files. Open the assessment and data files to understand the task; add the implementation notebook or script here if you want this project to be runnable directly from the repository.

## 6. Name Game: Gender Prediction from Names

**Goal:** Explore author-name data from *The New York Times* children’s picture-book bestseller lists and estimate author gender by matching names against baby-name datasets.

**What the notebook does**
- Uses baby-name data and NYSIIS-style name keys to find approximate matches.
- Applies fuzzy matching where exact matches are unavailable.
- Examines the gender distribution of authors across years and visualizes trends.
- Discusses why some names remain unmatched, including the possibility of authors born outside the United States.

**Tools:** Python, pandas, NumPy, matplotlib, fuzzy string matching, exploratory data analysis.

**Files**
- [Open the Jupyter notebook](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Name%20Game%20Gender%20Prediction%20using%20Sound/notebook.ipynb)
- [Baby-name dataset — NYSIIS](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Name%20Game%20Gender%20Prediction%20using%20Sound/datasets/babynames_nysiis.csv)
- [Baby-name dataset — Social Security Administration](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Name%20Game%20Gender%20Prediction%20using%20Sound/datasets/babynames_ssa.csv)
- [Yearly NYT kids' bestseller data](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/blob/main/Name%20Game%20Gender%20Prediction%20using%20Sound/datasets/nytkids_yearly.csv)

## 7. Naïve Bees — Image Dataset

**Goal / context:** A collection of bee images associated with a deep-learning image-classification exercise.

**Files:** [Browse the project folder and image dataset](https://github.com/kalpasur/Portfolio-Projects-College-Hustle/tree/main/Na%C3%AFve%20Bees%20Deep%20Learning%20with%20Images).

**Current limitation:** The tracked folder currently contains image files but no notebook or Python training script. Consequently, there is no verified execution file to link yet. Add the model-training notebook or script when available, and this section can be expanded with the architecture, training setup, evaluation metrics, and results.

---

## Running the notebooks

1. Open a notebook link above and use GitHub's notebook viewer to read it.
2. To execute a notebook, download or clone the repository and open it in Jupyter Notebook, JupyterLab, or a compatible environment such as Google Colab.
3. Install the libraries imported by that notebook.
4. Keep the expected folder structure and dataset paths, or update the paths if you move files.

    git clone https://github.com/kalpasur/Portfolio-Projects-College-Hustle.git
    cd Portfolio-Projects-College-Hustle

Not every folder currently contains a runnable implementation. Where only datasets or assessment files are present, this README says so rather than implying that code or results are available.

## Repository structure

- **B Testing with Cookie Cats/** — A/B test notebook and dataset
- **DC Workspace Archieve/** — archived analytics notebook and supporting files
- **Datacamp Data Scientist Certification/** — venue ramp prediction project and artifacts
- **Dog Classifier/** — Python image-classification workflow and sample images
- **Insurance Claim Predictor/** — assessment brief and datasets
- **Name Game Gender Prediction using Sound/** — notebook and name datasets
- **Naïve Bees Deep Learning with Images/** — image dataset

---

*This README documents the files currently tracked in the repository. Project results and execution instructions should be updated as implementations evolve.*
