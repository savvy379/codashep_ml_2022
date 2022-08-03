# CODAS-HEP ML Material 
This repo houses the ML material developed for [CODAS-HEP](https://codas-hep.org/) 2022. It is split into four lessons that include background/theory and hands on exercises (that are HEP focused when possible): 
- **Intro to ML**: background/basics of ML, conceptualizing linear regression as an ML model, and BDTs
- **Neural Networks and Convolutional Neural Networks**: basics of deep learning, i.e. MLPs and CNNs
- **Unsupervised Learning and Autoencoders**: motivation for unsupervised learning, algorithms: k-Means, PCA, t-SNE, autoencoders
- **Graph Neural Networks**: background on graphs as data representation, theory of GNNs, node classification with Cora dataset and charged particle tracking via edge-classifying GNNs

Please feel free to use these materials (with attribution) for your own teaching and learning. 

## Setup 
In order to make these tutorials as portable and widely usable as possible, they are designed to run on Google Colab rather than any specific system. To set up the repo please follow these steps: 

1. Set up a google drive account if you do not already have one 

2. Visit Google Colaboratory [website](https://colab.research.google.com/). Click on New Notebook button. A blank notebook is initialized and open. You can use this notebook like a shell to setup your repo. 

3. Run the below script (in the notebook) to mount your Google Drive
```
from google.colab import drive
drive.mount('/content/drive')
```
Select the respective Google Drive account on which you want to mount and click on sign in

4. Create a GitHub folder in your Google Drive and cd into the folder 
```
%mkdir /content/drive/MyDrive/Github/
%cd /content/drive/MyDrive/Github/
```

5. Generate a GitHub access token (if you do not already have one). 
Visit GitHub website and login to your account.  
Go to Settings, navigate to Developer settings and then click on Personal access tokens.   
Click on Generate new token button on top right corner of the page.  
Click the repo checkbox under Select scopes section.   
Click on Generate token button at the bottom of the page. 

6. In your Colab notebook, clone the repository using the following command
```
!git clone https://{git_token}@github.com/savvy379/codashep_ml_2022.git
```

You now have access to the repo and can run all notebooks in the Colab environment. You can access the repo in your GitHub folder in your Google Drive to open the notebooks. You can also use a Colab notebook as a shell to interact with github through the normal commands by putting a '!' at the beginning.

You can, of course, run the notebooks locally as well you will just need to ensure you have the required packages installed. 
