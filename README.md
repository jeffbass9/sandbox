# sandbox
Quick boilerplate code for HTML/CSS projects. 

## Steps to get up and running 

### MAMP

1) Download <a href="https://www.mamp.info/en/downloads/">MAMP</a>. MAMP will prompt you to download MAMP and MAMP Pro; that's fine, just download both and use the regular version of MAMP (free). Once you have that installed, find the MAMP/htdocs folder in Finder or Windows Explorer. Rename the sandbox repository you downloaded (this one), and drop it in this folder.  

### Creating a Git repository 

1) On the sandbox repo (https://github.com/jeffbass9/sandbox), click “Use this template” button. This will prompt you to create a new repo. Give it a name, and then click “Create repository from template.” 

2) Click the green “Code” button, and select “Open with GitHub Desktop.” Download GitHub Desktop when prompted. Once the download has completed, open GitHub Desktop, and sign in with your GitHub ID. Follow the prompts to “authorize desktop” and enter your password. 

3) After you are finally redirected to GitHub Desktop, click “Clone a Repository from the Internet.” Select the new repository you created from the sandbox template, change the local path to point to the “MAMP/htdocs” folder, and click “Clone.” 

4) You should then be able to open this repository in your text editor either from within GitHub Desktop (“Open the repository in your external editor”) or by navigating to the repository in Finder or Windows Explorer in the MAMP/htdocs folder. 

### Starting to code 

1) Start building your markup (HTML) first, in index.html. I would recommend filling this out completely with dummy content, so that you have a realistic goal of what dimensions you will need for the various sections. For the dynamic sections (modules that will change often, like the carousel, social media feed, etc.), I would recommend just filling in a grey box or something along those lines. We are focusing on HTML and CSS right now, and those will rely on Javascript, so we want to stake out the space needed for those without wasting time on JS at this stage. 

2) To check your progress in the browser, make sure you've launched MAMP, clicked "Start servers" and navigated to localhost:8888/your-project-name (or clicked "Open WebStart page" in MAMP and then clicked on "My Website").

3) Once you are done adding all of your content to the page, start adding your CSS for the mobile layout of the site. When adding CSS classes to your HTML elements, I would recommend prefixing your classes, so that they will not be at risk of conflicting with other stylesheets in the future. For example, instead of adding a class to a div called "container" (a very common class across a variety of frameworks and standalone stylesheets), add a unique prefix like "assp," so your class would be "assp-container." If all of your classes are prefixed like this, it makes it very easy for you (or a future designer or developer) to look through the code and separate which styles you added vs. which styles were added later. 

4) Completely style your mobile layout first, before moving on to tablet and desktop layouts. This way, you can write all of your necessary CSS, and then add media queries to start adding in changes as the screen gets wider. For example, if you need larger \<h1\> tags once the screen is larger than a phone, you can add:
```
@media screen and (min-width: 789px){ 
  h1{ 
    font-size: 24px; 
  }
}
```

### Saving

1) After reaching a good stopping point in your work, it’s a good idea to make a save point, or “commit” in Git terminology. To do this, open up GitHub Desktop, and open your repository. The window will show you which files have been changed, and what those changes looked like. Add a description of the work you did to the “Description” box, and click “Commit to main.” 

2) This will then prompt you to “Push commits to the origin remote.” This takes the copy of the repository you have on your computer and updates the master version you have hosted online, in your Github account. Click “Push origin.”
