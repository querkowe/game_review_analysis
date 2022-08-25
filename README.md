# game_review_analysis

```
pip install googletrans==4.0.0-rc1
pip install lightgbm

```

```
import warnings
warnings.filterwarnings("ignore")

import requests
import urllib.request
import sqlite3


import googletrans
import time
import joblib
import pickle
import os
import sys
import re
import nltk
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline

from collections import Counter
from nltk.corpus import stopwords
from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer
from sklearn.model_selection import train_test_split, GridSearchCV
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
from sklearn.metrics import confusion_matrix, classification_report
from sklearn.metrics import roc_curve, roc_auc_score
from sklearn.metrics.pairwise import cosine_similarity
from lightgbm import LGBMClassifier
from PIL import Image
from IPython.display import display
from tqdm import tqdm
from mpl_toolkits.mplot3d import Axes3D

from webdriver_manager.chrome import ChromeDriverManager
from selenium.webdriver.chrome.service import Service
from selenium.webdriver.chrome.options import Options

from selenium import webdriver
from selenium.webdriver.common.by import By
from selenium.webdriver.common.keys import Keys
from bs4 import BeautifulSoup
```
