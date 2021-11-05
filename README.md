# Penguins web app deployed on Heroku

The deployed web app is live at https://penguin-classification-strmlit.herokuapp.com/

This web app predicts the species of penguins as a function of their input parameters (bill length, bill width, flipper length, body mass, sex and island).

There are multiple files in this repository. You can check out my other repository to know about the classification project in detail. Here I will be talking only about the deployment process.  
Project Link - https://github.com/danishkhan0510/Data-Science-Apps-with-Streamlit  

First you need to visit https://www.heroku.com/ and sign up. Once you have authenticated your email address you can visit your heroku dashboard. Click on the "New" icon and select 'Create new app'. You will be directed to a new page where you can give your app a unique name and go ahead. In the deployment method you can select GitHub which would then require you to connect to your GitHub account. Once done, type in your repository name and click deploy. Now sit back and relax while all your dependencies are installed and finally you will see a "View" icon. Clicking it would take you to your web app. Go ahead and share the link with all your friends!
 
 **requirements.txt** - This file will contain all the libraries that you have used in the app.py file. You need to provide the exact version of the library you have used while testing the app. Heroku will install those same versions so that the app can run smoothly. This is needed because maybe your app is not compatible with some newer versions of the library which would hinder the deployment process.  

**setup.sh** - This is a shell file which you need for deployment. Just go ahead and use it directly.

**Procfile** - The “web” means that it’s a web app. The Procfile pretty much specifies the commands once you run the app on Heroku. We specify the shell file that we created above and then call Streamlit to run app.py.
