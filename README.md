# Welcome
If you are reading this README it means you have downloaded `bot-tutorial-master` bundle from the [ROAR Getting Started](https://stanford-roar.com/#/guide) page.  You will need to complete below prerequisite steps before you can enter your bot model in a ROAR contest using one of the provided Quickstart Jupyter Notebooks in this bundle. 

## Prerequisites

### Obtain a Bot Identity Token
Before you can connect to a ROAR contest via one of the provided Quickstart Jupyter Notebooks, you will need complete below steps to register your bot in the contest you wish to enter.
1. Launch the [ROAR web application](https://stanford-roar.com) and log in. 
1. Click *View & Enter Your Bots* button to the right of the contest you wish to enter your bot in and follow the bot creation wizard <br/>
1. Make sure to copy the identity key generated for your bot on the following 'My Bots' page.  

**Note:** You must complete the submit action at step 4 before you can start to use your bot identity token to connect to ROAR.

### Review Contest Description
Make sure to review the Contest Description page for the contest in which you want to enter your bot model.  You can find it by browsing the [ROAR Contests](https://stanford-roar.com/#/contests) view and clicking the *Read Description* button to the right of the contest name. For DTCC contest, please review below additional resources from the `bot-tutorial-master` bundle: 
- `protocol.md`: Covers the raw protocol for question and prediction messages in the DTCC contest  
- `DTCC-Data-Exploration.ipynb`: provides historic DTCC trade data (the live data stream is also exposed via `on_broadcast` method in the  Quickstart Jupyter notebooks listed below), and also offers examples of applying different machine learning models to the DTCC data.  Note this data covers all indices, not just the four you are asked to predict for DTCC contest.

## Quickstart Jupyter Notebooks
In the downloaded `bot-tutorial-master` bundle you will find below Quickstart Jupyter Notebooks which you can use to build a model and enter your bot into either of the two contests hosted on ROAR (namely Tutorial/Sine and DTCC).
- `Quickstart-Beginner.ipynb` <br/>
  This quickstart uses a last value model to predict the target for a contest in ROAR.
- `Quickstart-Intermediate.ipynb` <br/>
  This quickstart uses a linear regression model to predict the target for a contest in ROAR.
- `Quickstart-Advanced.ipynb` <br/>
  This quickstart uses a temporal convolutional network model to predict the target for a contest in ROAR.
  
  
### How to Get Started with your Bot ###

To speed up the process, we can set up a baseline for you and give you access to a bot running in the cloud.

**This is by far the easiest option of those listed here**<br/>
**Please email bramos@stanford.edu to ask for your bot to be set up**

  
### Running Locally -- For those who want to deploy on a computer themselves (a pre-existing account, either locally or in the cloud)

**Caution: A locally-deployed model will obviously only run when your computer is awake.**

There are two options for running a Quickstart Jupyter Notebook locally on your machine. We recommend the docker based setup unless you have most of the dependencies already available on your machine (e.g. Python 3.7 or higher, Jupyter, PIP) 

#### [Run with Docker](docker.md) <br/>

#### [Run without Docker](basic.md) <br/>

## Deployment options -- For those who want to deploy in the Cloud themselves (this walks you through how to set up a Cloud account)

Once you've built and tested your model, we do not recommend that you run it locally as your bot will disconnect from ROAR contest in the event of your workstation going to sleep or getting shut down.  Hence, it is recommended that you deploy your bot model on a more stable server infrastructure such as the Public Cloud. Some cloud options and detailed deployment steps are provided below.

#### [Google Cloud Platform](gcp.md)
#### [Amazon Web Services](aws.md)

You are welcome to try out other options and share via GitHub your solution!

## FAQ and Troubleshooting
[FAQs](FAQ.md) <br/>
