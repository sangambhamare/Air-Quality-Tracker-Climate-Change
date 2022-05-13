# Air-Quality-Tracker-Climate-Change
This project is based on Python using Azure App Service. Please read same for more information.

#Problem Statement/Opportunity :
A major scourge of our era, air pollution has an impact on not only climate change, but also the health of the public and individuals due to increased morbidity and mortality.We will use the Azure map service to track air polluted areas in this project because air pollution is a major factor in human health.If we take some precautions, we can easily reduce pollution in those areas.

#Project Description :
As multiple human activities influence the environment, there has been extensive study of the interactions between humans and their physical surroundings.Abiotic (water, lithosphere, and atmosphere) and biotic (living organisms and microorganisms) components combine to form the environment.As defined by the World Health Organization, pollution is the introduction of harmful substances into the environment.A pollutant is a solid, liquid, or gas that is produced in high concentrations and reduces the quality of our environment.With this project we are going to track air pollution, which will help prevent air pollution in polluted areas. Visual Studio Code is used to develop this project in a Python environment.This project contains CSS and HTML for designing web pages.A very important Azure service for tracking Air Quality is Azure Map Service, which shows a global map of Air Quality.

#Azure Technology Used :
1. App Service
2. Azure Maps
3. Visual Studio Code

#Set up initial environment
1. Have an Azure account with an active subscription. Create an account for free.
2. Install Python 3.6 or higher. add in python path in your environment path.
3. Visual Studio Code
4. Install Visual Studio Code and the Python Extension

#Configure environment
1.Create folder and Clon a repository and open same folder in Visual Studio Code.
2. In Visual Studio Code, select Terminal > New terminal to open the terminal.
3. python -m venv .venv This command creates a virtual environment inside the current folder. Visual Studio Code detects this change and prompts you to select the virtual environment for this folder. Select Yes.
4. Install pip packages using command pip install -r requirements.txt
5. At the root of your application code folder, create a new environment file named .env.
6. Create Azure map account add primary key in .env file - MAP_KEY=<your map key>
7. Create account on World Air Quality Index and get WQAI_API_KEY. Update WQAI_API_KEY=<WQAI api key>
  
#Run and debug the app
  1. Set up Visual Studio Code to run and debug a Flask app. 
  2. Then, use your browser to see the app in action. In Visual Studio Code, be sure that the app.py file is open in the editor. (Debug options vary based on the file you have open.) In the Activity Bar, select the Run icon. Under the Run and Debug button, select the create and launch.json file link. 
  3. In the selection drop-down, choose the Flask link. When Python:Flask shows in the Run view, select the green arrow to run the application.
  4. Expected output :
  
 * Serving Flask app "app.py"
 * Environment: development
 * Debug mode: off
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
  
Open link on brower : http://127.0.0.1:5000/
  
#Deploying App to Azure App Service
1. Deploy project to Azure App Service as part of your continuous deployment (CD) workflows.
2. Configure Azure Map key - In the Azure portal, search for and select App Services, and then select your app. In the app's left menu, select Configuration > Application settings.
3. In New application setting add key MAP_KEY and value = <your map key>
4. Also add key-value for WQAI_API_KEY
5. Check deployment after Github action build completed, website link should avilable in Github build as well as Azure App Service.


