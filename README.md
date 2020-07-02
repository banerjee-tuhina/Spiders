# Spiders
# Social Media Monitoring– It’s Possible 
  
Fake or inaccurate news spread through social media in the country has become a serious problem, with the potential of it resulting in mob lynching, cyber-bullying, child abuse, child pornography, drug peddling, etc. Fake news can cause an unwanted political riot to a case of murder.
Social media is a platform of discussing memories and connecting with people has also become a place of murder or terrorism or cyber bullying or drug peddling using coded languages and unauthorised profiles. 
Being a large network it’s difficult to monitor such kind of medium manually (by humans) completely and provide precautions. 
Hereby, the prototype will help in controlling the trend of fake news by analysing the posts and declaring as proper or improper. Also our system is been design in a way that it reads data (text or image) and scans it whether it has any abusive or sexual content which might affect the society.   
Getting Started
These instructions will get you a copy of the prototype up and running on your local machine for development and testing purposes. 
Prerequisites
In order to run the programs on Jupyter Notebook, the following libraries need to be installed using the anaconda prompt
	tensorflow - https://www.tensorflow.org/install/pip
	Keras - https://pypi.org/project/Keras/
	opencv (cv2) - https://pypi.org/project/opencv-python/
	Pillow - https://pypi.org/project/Pillow/
	nltk - https://pypi.org/project/nltk/
	pytesseract - https://pypi.org/project/pytesseract/
	pytesseract – tesseract.exe - https://github.com/UB-Mannheim/tesseract/wiki
	scikit-learn - https://scikit-learn.org/stable/install.html
	beautifulsoup4 - https://pypi.org/project/beautifulsoup4/
Download the "Project" folder from GitHub. 

# This folder contains:

# 1. Datasets
jigsaw-toxic-comment-train.csv – This csv file provided by kaggle(google) contains comments used for toxic comment classification. 
NSFW Test Dataset – This folder images used for image classification. 
P.S. Note: For our required prototype we have used pictures which has severe vulgar content to classify image’s actions in the post or comment, to reduce cyber bullying or body shaming cases and discussions held in the social media channels.
We as students have no content or intention to offend any individual. 

# 2. Jupyter Notebooks
ToxicComment.ipynb – This jupyter notebook contains algorithm for classifying statements as toxic or not toxic. 
ImageIdentification.ipynb – This jupyter notebook contains algorithm for determining whether a given image contains nude or gory content.
DDNewsWebScraper.ipynb – This jupyter notebook contains algorithm for scraping the DD News website and storing scraped data in the form of a csv. 
IntegratedCode.ipynb – This is the main jupyter notebook which is connected to Anvil Website.
Note: This notebook contains pre-trained models for testing to reduce the runtime and for the ease of integration with anvil.works (cloud) used for User interface.

# 3. Models
ml_model.sav – This file is obtained after executing ToxicComment.ipynb. It contains the trained Naïve Bayes model for toxic comment classification.
feature.sav – This file is obtained after executing ToxicComment.ipynb. It contains the feature vectors of words obtained after applying fit transform on the dataset used for toxic comment classification. 
finalized_model.sav – This file is obtained after executing ImageIdentification.ipynb. It contains the trained CNN model for identification of images containing nude or gory content.

# 4. Installing
Once downloaded, open anaconda prompt and change the directory to open the “Project” folder. To do this, copy the path to the “Project” folder and paste the path in anaconda prompt and then activate jupyter notebook as follows :-
	cd “paste the path to folder here”
 

# 5. Running the tests
We have used anvil.works for the user interface for a better see through thus this link executes in a manner which only requires the input and runs the backend invisibly to make it look easy to run and manage for the user of the system (System Administrator).
Execute the IntegratedCode.ipynb and then click on the link to anvil website
https://NE6ULVW75QUID3GW.anvil.app/KZCJW3H3DUSKVUV4YOK7KQZT
Note: Due to computational powers we have some limitations over our system which will be worked upon as and when scaled with fast and easy computational powers.
Thus, we worked and designed the system in a way that the user need to put a hashtag for detailed analysis of the data posted.

# 6. Considerations during for the input of the prototype:

A.	If the user wants to test by posting any data he/she will use a hashtag for the same,
As per the registered hashtags we have:
1.	#image – This hashtag declares the post to be an image (As it passes through vulgarity or abusive check if has any object or it passes through toxic      sentence analysis for the text if any) controls cyber bullying and vulgarity.
2.	#news – This hashtag declares the post to be a valid news or any relevant comment on the news but not personal or controversial comment. (As it passes    through similarity check with the reference site DD national news) controls fake news.
3.	#personalviews - This deals with one’s personal views on news or any random content. (As it passes through toxic comment analysis) controls fake news      and vulgarity.
4.	#newsimage - This deals with the images which has a news content. (As it passes through extraction and a check of similarity with the new) controls        fake news. 

B.	If the user wants to test for comments,  

1.	He/ she has to use “@” followed by any username.
      Eg: @letstrytogether it’s a great work!

The requirements posted are naturally been performed in any social media platforms we used thus we as developers have considered these few points to make the system accurate and reliable.
On further development period we will be integrating the real time social media apps so that the input will be auto generated when the user posts anything on the respective social media handles.

# 7. Built With
Anvil.works –Cloud for User Interface 
JupyterNotebook - Dependency Management
ROME - Used to generate RSS Feeds

## Authors
Sakshi Butala
Tuhina Banerjee

# Team
Spiders
