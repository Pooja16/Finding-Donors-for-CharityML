# Finding Donors for CharityML
## Introduction:

CharityML is a fictitious charity organization located in the heart of Silicon Valley that was established to provide financial support for people eager to learn machine learning. After nearly 32,000 letters were sent to people in the community, CharityML determined that every donation they received came from someone that was making more than $50,000 annually. 

To expand their potential donor base, CharityML has decided to send letters to residents of California, but to only those most likely to donate to the charity. 
CharityML needs to build an algorithm to best identify potential donors and reduce overhead cost of sending mail. My goal is to evaluate and optimize several different supervised learners to determine which algorithm will provide the highest donation yield while also reducing the total number of letters being sent.

##  Table of Contents:

This project contains the following files:
- `finding_donors.ipynb` : This python file has all the code that was used to put through the entire analysis. 
- `finding_donors.html` : This is the html version of finding_donors.ipynb file. 
- `census.csv` : The project dataset. 
- `visuals.py` : A Python file containing visualization code that is run behind-the-scenes. Do not modify
In the Terminal or Command Prompt, navigate to the folder containing the project files, and then use the command `jupyter notebook finding_donors.ipynb` to open up a browser window or tab to work with your notebook. Alternatively, you can use the command `jupyter notebook` or `ipython notebook` and navigate to the notebook file in the browser window that opens.

##  Summary of Results of Analysis:

I transformed skewed continuous features, normalized numerical features and data preprocessing to get data ready for the analysis. 
I created a naïve classifier as a benchmark to compare more advanced algorithms with. Evaluated and compared performance of Gradient Boosting Classifier, KNeighbors classifier and Support Vector Classifier.
Based on evaluating the machine learning algorithms Gradient Boost Classifier had the highest accuracy , f-score and performed well on both training and test datasets.

I used hyper parameter tuning to optimize performance of Gradient Boosting Classifier. I also looked at the extracting feature importance and the effect on the model performance. Accuracy and fscore are only some percentage points lesser on the model with reduced data. Even though the training time for gradient boosting is not that high but in cases where training time is an important aspect the model with reduced data would work well.

##  Software:

This project uses the following software and Python libraries:
-  [Python 2.7] (https://www.python.org/download/releases/2.7/)
-  [NumPy] (http://www.numpy.org/)
-  [Pandas] (http://pandas.pydata.org/)
-  [scikit-learn] (http://scikit-learn.org/stable/)
-  [matplotlib] (http://matplotlib.org/)
You will also need to have software installed to run and execute a [Jupyter Notebook] (http://ipython.org/notebook.html)
If you do not have Python installed yet, it is highly recommended that you install the [Anaconda] (http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 2.7 installer and not the Python 3.x installer.
