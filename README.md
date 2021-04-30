# sandbox
Quick boilerplate code for HTML/CSS projects. 

## Steps to get up and running 

Download <a href="https://www.mamp.info/en/downloads/">MAMP</a>. MAMP will prompt you to download MAMP and MAMP Pro; that's fine, just download both and use the regular version of MAMP (free). Once you have that installed, find the MAMP/htdocs folder in Finder or Windows Explorer. Rename the sandbox repository you downloaded (this one), and drop it in this folder.  

Start building your markup (HTML) first, in a file named index.html. I would recommend filling this out completely with dummy content, so that you have a realistic goal of what dimensions you will need for the various sections. For the dynamic sections (modules that will change often, like the carousel, social media feed, etc.), I would recommend just filling in a grey box or something along those lines. We are focusing on HTML and CSS right now, and those will rely on Javascript, so we want to stake out the space needed for those without wasting time on JS at this stage. 

Once you are done adding all of your content to the page, start adding your CSS for the mobile layout of the site. When adding CSS classes to your HTML elements, I would recommend prefixing your classes, so that they will not be at risk of conflicting with other stylesheets in the future. For example, instead of adding a class to a div called "container" (a very common class across a variety of frameworks and standalone stylesheets), add a unique prefix like "assp," so your class would be "assp-container." If all of your classes are prefixed like this, it makes it very easy for you (or a future designer or developer) to look through the code and separate which styles you added vs. which styles were added later. 

Completely style your mobile layout first, before moving on to tablet and desktop layouts. This way, you can write all of your necessary CSS, and then add media queries to start adding in changes as the screen gets wider. For example, if you need larger \<h1\> tags once the screen is larger than a phone, you can add:
```
@media screen and (min-width: 789px){ 
  h1{ 
    font-size: 24px; 
  }
}
```

## Git steps
