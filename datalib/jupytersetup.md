# Data processing through JuypterHub

While the library is the collection of datasets the data researchers can search to learn about the studies and the data sources that data scientists/researchers are using in their Mathematica studies, the JupyterHub web tool allows the scientists to analyze/process the data sources.

JupyterHub is a web based server instance for a project group to run calculations, research, collaborate on the project datasets (datasources) using Jupyter notebooks. The JuypterHub data science environment configured for the data library project groups includes Python, R, Stata languages for the users to do their data processing.


To log in,

* The JuypterHub workspace is configured for each project in the Data Library and requires the project number, the project unit (Health, Human Services, International), approximate storage capacity needed for the project data processing for the set-up. The project lead provides this information along with an approximate storage size required for the project's datasets and computation needs to the data librarian.
* The projects approved to access the Data Library will receive a separate email invitation to the JupyterHub. 
    * Note that the setting up the JupyterHub workspace for the project may take a couple of days longer than setting up the project access the Data Library to upload the datasets via packages. We recommend that project teams start adding the project details, uploading the datasets to the library and then wait for the JuypterHub email invitation to start processing the datasets within the project storage bucket.
* Signing in to the JuypterHub involves logging to two UI consoles
* Click the JupyterHub URL link you receive in the email invitation. 
   ![](images/jup_invite.png)
   
   The URL is specific for each Data Library projects, and you see the project number in the URL. 
   > Save this email with the JuypterHub credentials - it takes a week before the JuypterHub allows the user to change the password in its terminal.
* Click **Sign up** in the sign in page that appears. 
   ![](images/jup_signup.png) 
* Enter your email name as the user name (for example, enter jdoe as the user name if your Mathematica email address is jdoe@mathematica-mpr.com). Enter your email address, the password provided in the invitation, and click **Sign up**.
   ![](images/jup_createuser.png)
* You will then receive an email with a verification code for the sign-in. Enter the verification code and click **Confirm Account**.
   ![](images/jup_code.png) 

   The action then displays the JupyterHub Console login page.
   ![](images/hub_signin.png)
* Enter your email name (example jdoe), the password provided in the invitation, and click **Sign in**.
   ![](images/hub_view.png)
* You now see the JuypterHub workspace configured for your project.
