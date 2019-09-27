# responsivegogs

Gogs responsive as a class project.

You will make the open source git program accessible and responsive.

1. Start by surfing to https://gogs.selab.ca, signing up if necessary and signing in.
2. Once you are signed in save the `website complete` of the page by right clicking and doing `Save as ...`
![save as webpage complete](https://rhildred.github.io/responsivegogs/READMEImages/step1.png)
3. Create a new folder and save the website complete in it.
4. Rename the only .html file as `index.html`
5. Go to your github and create a new repository
6. open a git bash shell and follow the steps on github to get your project on github.

```

echo "# Responsive Gogs" >> README.md
git init
git add *
git commit -m "first commit"
git remote add origin https://github.com/rhildred/responsivegogs.git
git push -u origin master

```

7. Back in Github verify that the code is there and go to the settings screen
![save as webpage complete](https://rhildred.github.io/responsivegogs/READMEImages/settings.PNG)
8. Scroll down to the github pages portion of the settings page and set the source branch to `master`
![save as webpage complete](https://rhildred.github.io/responsivegogs/READMEImages/githubpages.PNG)
9. Follow the link that comes up to your site. Note that it might take some time for it to be active.
![save as webpage complete](https://rhildred.github.io/responsivegogs/READMEImages/link.PNG)

## Levers for making the site responsive and accessible.

The last time I built Gogs on my system I included a `selab.css` and `selab.js` file for you to make your changes in. Once you have made your initial push to github you can also edit the `index.html` file.

I included a dark theme from [https://github.com/Kos-M/GogsThemes](https://github.com/Kos-M/GogsThemes). You can get it into your project with:

```
/* put your css changes here */

@import url("dark_theme.css");

```

## The axe accessibility tool

You will want to use a tool to check the accessibility of your changes. I used [axe](https://chrome.google.com/webstore/detail/axe/lhdoppojpmngadmnindnejefpokejbdd). Add it to your browser by following the preceding link. 

Axe won't work on a file:// link. You will also need a vscode plugin to serve your content on [http://localhost:8080/index.html](http://localhost:8080/index.html). The one that I used is by YuichiNukiyama. 
![Preview on Web Server](https://rhildred.github.io/responsivegogs/READMEImages/vscodeExtension.png)

If you right mouse click on your .html file choose `Launch On Browser` to see your code in chrome. 

![Launch on Browser](https://rhildred.github.io/responsivegogs/READMEImages/LaunchOnBrowser.png)

In chrome right click and do `inspect` to bring up the developer's tools. In the developer's tools click on `axe`.

![Developer tools Axe](https://rhildred.github.io/responsivegogs/READMEImages/GoIntoAxe.png)

Finally you can run `Analyze` to see the accessibility problems.

![Analyze](https://rhildred.github.io/responsivegogs/READMEImages/Analyze.png)

I find Gogs perfect for my product development and consulting needs. Hopefully you will be able to refresh the look of it by making it accessible and responsive.

