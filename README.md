# Quality Check Tool
United Way Tax Tool Code for volunteers (code to be used in clinics)

For code to work on machine, please do the following:

# United Way VITA Tax Tool: Software Installation & Setup Instructions 
## Step 1: Install Anaconda
You can download and install Anaconda (aka "conda") version 3.7 here:  https://www.anaconda.com/distribution
Conda is a "package manager," which is sort of like an "app store." It installs Python and a bunch of useful Python packages by default, and it can be used to install or update additional packages later on.

If you already have installed Python things using "pip" (a different package manager), then installing conda may cause the old Python things to work differently because they're now using the new versions installed by conda. In most cases this is fine: you can and should use conda for all your Python installation and update needs (see "why use conda?" on their website).

## Step 2: Open Jupyter Lab
This is the interface we will use to run the VITA Tool. Conda installed this for you. In most cases, you can get to it by using any of the options below:
- Opening the "Anaconda Navigator" and clicking "Launch Jupyter Lab"
- Typing "Jupyter" into your computer's search bar and clicking on "Jupyter Lab"
- Running "Jupyter Lab" in the terminal
- Jupyter opens two things:
  * A terminal / command line window. Ignore this. You won't need to do anything with it. Closing this window kills Jupyter, so don't do it unless you're done working and you have saved your work.
  * A browser tab. This is where we run the VITA Tool. It is not online, and it does not require internet to work. Jupyter runs on your computer and uses your browser to display interactive text and images. 
- If the installation worked and Jupyter opened okay, you're all set!
- If not, please check StackOverflow or shoot me an email at amynewman2@gmail.com

## Step 3: Create a Virtual Environment and Install poppler and pandas

### For Mac:
1. In Anaconda Navigator, launch Jupyter Labs.
2. In Jupyter Labs, navigate to File > New > Terminal. A new tab should open called “Terminal 1”. In this terminal, run the following commands. (NOTE: anytime you enter a command and see "Proceed ([y]/n)?" type "y")
 - conda create -n unitedway python=3.7
 - conda activate unitedway
 - conda config --add channels conda-forge
 - conda install poppler
 - conda install pandas
 - conda install xlrd

### For Windows:
1. Navigate to Anaconda3(64-bit) > Anaconda Prompt(Anaconda3)
2. Type in the following commands and press enter, then "y" for each command
 - conda create -n unitedway python=3.7
 - conda activate unitedway
 - conda config --add channels conda-forge
 - conda install -c conda-forge poppler
 - conda install pandas
 - conda install xlrd
3. Close Anaconda Navigator, then re-open Anaconda Navigator


## Step 4: Open Jupyter Lab with your unitedway environment

- Close Jupyter Labs and Anaconda Navigator
- Open Anaconda Navigator, then select unitedway from the dropdown after At “Applications on”. 
- Click “Install” for  Jupyter Labs (making sure you’re using the unitedway environment)
- Click “Launch” for Jupyter Labs

## Step 5: Download Files to Run VITA Tool
- Download from Github or email
- Unzip Folder and keep on Desktop
- Use Run_Tax_Tool.ipynb only for running the program


# United Way VITA Tax Tool: How to Open the Program
- Turn on laptop and log in
- Open Anaconda Navigator

### In Mac use either:
- Launchpad
- Your terminal (type “jupyter lab”)

### In Windows:
- Click on "Start" > Anaconda3 (64-bit) > Anaconda Navigator (Anaconda 3) - it has a green circle in front of it
- Set your Anaconda Navigator to unitedway
  - Use the dropdown next to “Applications on” to set to “unitedway”

- Click “Launch” under JupyterLab

# United Way VITA Tax Tool: How to Run the Program 

- Go to Desktop > UW_volunteers > 2019_Returns 
- Drop .pdf files into the 2019_Returns folder that you would like the tool to run
- In Jupyter Lab, navigate to  Desktop > UW_volunteers > Run_Tax_Tool.ipynb
- Click Run > Restart Kernel and Run All Cells…
- This will run all files in the 2019_Returns folder

## Output
Output will be in the following files:
- Client_output.txt
- 2019_client_tax_information.csv

### To print a copy of the Client_output.txt, navigate to Desktop > UW_volunteers > Client_output.txt and print from there. 

Instructions to Run the Tool: https://docs.google.com/document/d/1Q_kYThjvs6nUPQ1KX9c6iDNDmV-CNSKAol5-SUGGc-o/edit?usp=sharing

