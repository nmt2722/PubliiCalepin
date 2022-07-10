# PubliiCalepin
## Testing Publii site 


### Uploading the site

- After logging-in, open your Github profile settings.
- In the left-sidebar of your profile screen, click on the Developer settings.
- On the GitHub Apps page, in the left-sidebar, click on the Personal access tokens option.
- Now we're on the Personal access tokens page; we need to make a new one for our site, so click on the Generate new token button near the top of the screen.
  On the next screen, fill out a name in the Token description section e.g. "Publii". Now in the Select scopes section, add a checkmark to the main Repo option, which     will give the token access to all aspects of managing your repository. Finally, click the green Generate token button at the bottom of the screen.
- You'll now be taken back to the Personal access tokens page, but now your new token will be visible at the top of the list. Whatever you do, don't close or refresh this page; the token will only be visible immediately after generation. Click on the Copy icon next to your token (see the image below), and copy it somewhere safe as we'll need it when setting up Publii to work with our Github Page.
> Remember: you won't be able to see the token again so make sure it's saved somewhere.
- Log-in to Github as normal, then click the plus icon in the topbar to open a submenu; now click on the New repository option to be taken to the Create a new repository screen.
- On this screen, fill out a Repository name, and leave the repository as Public (Github Pages are always public, even when the repository hosting it is made private). Next, click the green Create repository button at the bottom of the screen.
- On the edit screen for the readme, just click the Commit new file button. We're only creating this file because your repository needs at least one item to be added to create your master branch, where all your Publii files will go. This created file will be removed automatically the first time Publii is syned with our Github Page.
- After committing the file we're taken back to the file listing; click on the Settings tab near the top of the screen.
- On the settings screen, scroll to the Github Pages section; in the Source option, click on the drop-down list that by default displays None, and select Main branch from the list of options. Now click the Save button to make sure the changes are committed.
- After saving, your GitHub pages will be ready to be used as a static website host; to view your website you'll need to go to the URL provided in the green message box. Of course, your site doesn't have any files yet, but we're going to change that.
- With everything prepared on Github, we can update the connection settings in Publii to sync with the Github Page repository that we just created. First, open up Publii; if you haven't already created your website, create one and add at least one post and ensure that you've selected a theme; without them your site will not be created properly.
### Updating the site
- Now click on the Server option in the left-sidebar to open the Server Settings screen. Fill out the fields with the following information:

  - Website Url - This will be your Github repository path, which uses the format "YOUR_USERNAME.github.io/ YOUR_REPOSITORY_NAME".
  - API Server - By default, this field is already completed with the standard API server. However, if you are running your own instance of GitHub, you can change the     API server by entering it here.
  - Username - Add your Github username here.
  - Repository - Enter the name of your Github repository here (we set this in step 2 of the Github Page section above).
  - Branch - If you've been following our guide, then write main (case-sensitive) in the text field; experienced users may want to specify other settings such as gh-pages, docs etc...
  - Token - Remember the access token we saved in the first part of this guide? Enter that here so that Publii can access the repository.
  - Parallel Uploads - Defaults to '1'. Sets the number of upload streams that Publii can use when uploading your site content to GitHub Pages. Higher numbers allows for faster uploads, but can cause errors on slow connections, or an error 403 due to API upload rate limits.
  -  API rate limiting - Disable this option only if you are using Github Enterprise with disabled API rate limiting. Otherwhise disabling this option can cause deployment errors.
  
### Once all the options are set, click on the Save Settings button to store your changes. Now may be a good time to click the Test Connection button, which will check to see if Publii is able to connect to your Github Page; if not, then some of the fields may have been entered incorrectly.

Everything is now ready, so we can click the Sync your website button in the Publii sidebar to start deployment.

### Inference

