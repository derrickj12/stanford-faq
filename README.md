# Welcome
If you are reading this README it means you have downloaded Tutorial.zip (bot-tutorial-master) from the [ROAR Getting Started](stanford-roar.com/#/guide) page.  You will need to complete below prerequisite steps before you can enter your bot model in a ROAR contest using one of the provided Quickstart Jupyter Notebooks. 

## Prerequisites
### Obtain a Bot Identity Token
Before you can connect to a ROAR contest via one of the provided Quickstart Jupyter Notebooks, you will need complete below steps to register your bot in the contest you wish to enter.
1. Launch ROAR web application via https://stanford-roar.com and log in. 
1. Click *View & Enter Your Bots* button to the right of the contest you wish to enter your bot in and follow the bot creation wizard <br/>
1. Make sure to save your bot identity token generated for you at step 3.  NOTE: You must complete the submit action at step 4 before you can start to use your bot identity token to connect to ROAR.

### Review Contest Description
Make sure to review the Contest Description page for the contest in which you want to enter your bot model.  You can find it by browsing the [ROAR Contests](stanford-roar.com/#/contests) view and clicking the *Read Description* button to the right of the contest name. For DTCC contest, also make sure to review the protocol.md document included in the bot-tutorial-master download which covers the raw protocol for question and prediction messages in the DTCC contest.  

## Quickstart Jupyter Notebooks
In the downloaded bot-tutorial-master bundle you will find below Quickstart Jupyter Notebooks which you can use to build a model and enter your bot into either of the two contests hosted on ROAR (namely Tutorial/Sine and DTCC).
- Quickstart-Beginner.ipynb <br/>
  This quickstart uses a last value model to predict the target for a contest in ROAR.
- Quickstart-Intermediate.ipynb <br/>
  This quickstart uses a linear regression model to predict the target for a contest in ROAR.
- Quickstart-Advanced.ipynb <br/>
  This quickstart uses a temporal convolutional network model to predict the target for a contest in ROAR.
  
### Running Locally

There are two options for running a Quickstart Jupyter Notebook locally on your machine. We recommend the docker install unless you already have a lot of the dependencies already available on your machine (e.g. Python 3.7 or higher, Jupyter, PiP) 

#### [Run with Docker](docker.md) <br/>

#### Basic Install
To run Quickstart Jupyter Notebook locally, you will need to complete below steps.
1. Install NodeJS from here: https://nodejs.dev/how-to-install-nodejs
1. Install **Python 3.7 or newer** and Jupyter if you don't have them installed already. If you need to install pip separately you can do so from [here](https://pip.pypa.io/en/stable/installing/).
1. Install dependencies by running the below commands. You will need to run the commands within `bot-tutorial-master` folder which is the parent folder of this README.md. 
   You may need to use `sudo` for pip install commands.
    ```bash
    cd bot-tutorial-master
    pip install -e bot-sdk
    pip install -r requirements.txt
    jupyter labextension install @pyviz/jupyterlab_pyviz
    jupyter labextension install @jupyter-widgets/jupyterlab-manager
    ```
1. Load one of below Quickstart Jupyter Notebooks available in `bot-tutorial-master` folder.  We recommend that you start with Quickstart-Sine.
    * `Quickstart-Tutorial.ipynb`
    * `Quickstart-DTCC.ipynb`
1. Start JupyterLab by running below command:
    ```bash
    jupyter-lab
    ```

## Deployment options

[heroku](heroku.md) <br/>
[GCP](gcp.md) <br/>
[AWS](aws.md) <br/>

# FAQ and Troubleshooting
[FAQs](FAQ.md) <br/>
