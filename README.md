# Online FLipping PDF Reader in turn.js - Kids book.

> This PDF reader has audio, good animation for flipping or just use the buttton for the next page.

### Tools used
- Adobe Photoshop.
- Text Editor :- Sublime text and Visual Studio Code. 
- Google (a lot of googling).
- the Internet.
- Netlify
- Github.

### Where & Why use the above tool 
- Photoshop yo resize my images in different dimensions (w*h):- 
	- 500*650  
	- 76*100
	- 1115*1443
- I like to use Visual Studio Code to push code on github.
- Sublime text is like my very 1st goto editor for quick start.
- Google for research on a new technology, bug solution etc.
-  the Internet to push code on github.
-  Netlify is free platform where you can deploy your frontend work, get an online link you can always share with other e.g. potfolio.netlify.com (dummy link) 
    - it is always best to connect your github to your Netlify account(signup using Github)

`  So far  so good, this is my 2nd time doing this and this time it is much easier actually. `

> The netlify link to this project  is  https://lugard-daycare-online-book-reader.netlify.app/

> NB: The number of pages of your PDF can be set or changed in the main.html on line 182....

#### How to add your local project to github
- web-based Github
  -create a new repository on the web-based Github (+ New Repository)
  - set a meaningful repository name 
  - don't create a README.md file
  - then create the repository...
- Terminal (vsCode terminal)
   - git init
   - git add .
   - git commit -m "meaningful message"
   - git remote add origin https://github.com/lailahgrant/online-pdf-reader.git
   - git push -u origin master

#### After adding your local project to Github. You will need a few steps to add new edits or deletes or just to keep track of what you're working on 
- Below are the steps you will need :
  - git add .
  - git commit -m :meaningful message"
  - git push -u origin master
  

> Make sure your root file is index.html if you're likely to deploy a site on Netlify to avoid "Page Not Found" ish 
> Reference https://community.netlify.com/t/support-guide-i-ve-deployed-my-site-but-i-still-see-page-not-found/125?utm_source=404page&utm_campaign=community_tracking

### Thur 25th Feb 2021 
` the netlify link https://lugard-daycare-online-book-reader.netlify.app/ takes alot of time to load  and after minutes of googling, figured I overloaded the repo with many images yet GitHub works best with only code in texts`

> Solution to this is https://docs.netlify.com/large-media/overview/ and it is what I'm going to try out today....!!

> After setting up my Netlify CLI, now onto setting up the Large Media https://docs.netlify.com/large-media/setup/

> # I'm completely using the documentation - no magic....

> In my local project linked to the repo - I likn it with Netlify cli 
- login in if I haven't already
  E:\lugard > netlify login
- netlify link - to link the local repo with the repo on Github and Netlify
- Run the following command for Large media
  `  netlify lm:setup `

  > This command will do the following: 
  - Enable the Large Media add-on for your Netlify site.
  - Configure Git LFS to use the Netlify Large Media service.

> After this,
> - git add .
> - git commit -m "meaningful message"
> - git push
>  - -> this push command failed, popped up an authentication, clicked it, authourized VSCode to my github and it worked.

#### Configure file tracking
> - Specify which files you would like to track with Large Media by using the `git lfs track` command

> - git lfs track "dog.jpg" "cat.gif" or
> - git lfs track "static/pdfs/**" or   
> - git lfs track "*.jpg" "*.png" 

> You can combine different types of patterns in a single command, or run the command multiple times.

> Commit your changes. When you run the git lfs track command, Git saves your tracking configuration in a `.gitattributes`  file.

> That's it... thanks for your time

> #  Enjoy...
