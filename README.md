# UHM Descartes Project Site

If you are changing the structure of this site, you will want to consult the documentation for the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) Jekyll theme.  If you are simply adding content, you shouldn't need to know much more than what is presented below.

Here's how to do it.

## 1. Obtain write permission to the repo

First, you must have write access to <https://github.com/uhm-descartes/uhm-descartes.github.io>. 

A quick way to see whether you have write access is to check whether or not there is a "pencil icon" in the upper right corner of the [README.md](https://github.com/uhm-descartes/uhm-descartes.github.io/blob/master/README.md) file. If you don't see a pencil, contact Prasad or Philip with your github username and one of them will provide you with permissions.

## 2. Set up your gitpod.io workspace

The simplest way to edit this site is by using <https://gitpod.io>:

<img src="README-screenshots/gitpod-1.png"/>

Click the "login" link, then "Continue with GitHub", then login to GitHub. You will eventually get to the "Workspaces" page:

<img src="README-screenshots/gitpod-2.png"/>

Click the "New workspace" button, then paste the following into the text field:

```
https://github.com/uhm-descartes/uhm-descartes.github.io
```

Select the item "github.com/uhm-descartes/uhm-descartes.github.io" that will appear, so the page looks like this:

<img src="README-screenshots/gitpod-3.png"/>

Now press the "Continue" button to build the workspace.

You will see a VS Code Editor UI appear in the browser window, and a Terminal window pop up and begin loading libraries (in green text). Wait until the libraries are all loaded and a command prompt (in blue) appears in the Terminal window:

<img src="README-screenshots/gitpod-4.png"/>

Now type `bundle exec jekyll serve` into the terminal window.  After a few seconds, a dialog box will pop up. You can choose "Make public":

<img src="README-screenshots/gitpod-5.png"/>

Once that's done, move the mouse over the "Server address" line in the terminal window and a "Follow link" window will appear:

<img src="README-screenshots/gitpod-6.png"/>

Click it, and the site will appear in a new browser tab:

<img src="README-screenshots/gitpod-7.png"/>

Installation is now complete. You can now edit and (when ready) publish the site. 

## 3. Edit the site

Editing the site is an iterative process of:

1. Making changes to the source files for the site. 
2. Verifying that the site builds and that your changes reflect your intent.

To make changes to the source files, just edit them using the browser tab containing the VS Code Editor UI. In most cases, the files you will want to edit are in the `_pages` directory. 

To edit pages, you will want to use "Markdown" syntax.  If you don't know Markdown already, you can read the [GitHub Flavored Markdown](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) reference page for details. 

In many cases, you will see that after you make changes to a file (and save it using control-s), the terminal window will produce output indicating that Jekyll has noticed the changes and has rebuilt the site. 

In that case, simply switching to the browser tab containing the built site and hitting the refresh button will be enough to reveal your changes. 

In other cases (such as when you edit config files), you may need to restart the Jekyll server to see the changes.  In this case, select the Terminal window, then press `control-c` (to terminate), followed by `control-p` (to retrieve the previous command, which is `bundle exec jekyll serve`), then `return` (to restart Jekyll).

## 4. Publish the site

When you are done editing, you should commit and publish your changes. This means sending your edited source files from gitpod.io to github.com.  The github.com repo is configured to automatically build and publish the site whenever commits are made to the repo. 

### 4.1 Give GitPod permission to write to the repo

If you are a first time user of GitPod, you need to give GitPod permission to commit changes to GitHub. Here's how to do it:

First, open a new browser and go to <https://gitpod.io>

<img src="README-screenshots/gitpod-12.png"/>

Now click on the avatar associated with you at the top right of the page to pull down a menu of items:

<img src="README-screenshots/gitpod-13.png"/>

Select “User Settings” to go to this page:

<img src="README-screenshots/gitpod-14.png"/>

Select “Git Providers” to go to this page:

<img src="README-screenshots/gitpod-15.png"/>

Now click the three vertical dots next to “GitHub”:

<img src="README-screenshots/gitpod-16.png"/>

Select “Edit Permissions” to pop up the following dialog box:

<img src="README-screenshots/gitpod-17.png"/>

Make sure all of the permissions are selected, then click “Update Permissions”.

Now GitPod has all of the permissions necessary to commit your changes, which we'll do in the next section.

### 4.2 Commit your changes to master

To publish the site, first notice that after editing a file, a blue dot will appear over the "Source Control" icon on the left side of the VS Code browser tab:

<img src="README-screenshots/gitpod-8.png"/>

Click that icon to reveal the Source Control pane:

<img src="README-screenshots/gitpod-9.png"/>

Enter a brief message in the top pane (such as "Fix home page"), then click the down arrow to the right of the orange "Commit" button to reveal choices. 

<img src="README-screenshots/gitpod-10.png"/>

Please select "Commit and Sync". (This will both push your changes to GitHub, and update your GitPod workspace with any changes committed by someone else to GitHub since you start working.)

If you now go to the "Actions" tab of the GitHub repository page, you'll see that GitHub is now building the site:

<img src="README-screenshots/gitpod-10.png"/>

Once there is a green arrow to the left of the "pages build and deployment" action, you should now be able to see your changes reflected in the published site at <https://uhm-descartes.github.io/>.

## 5. Beyond basic markdown

If you want to go beyond basic markdown, you will need to consult the [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/) documentation. Philip has done some basic customization of the defaults; you can contact him for guidance. 

## NRT Project Sites

You can find helpful examples of the content and structure of our site by looking at other NRT sites.  Here's links:

* https://futurerivers.uw.edu/
* https://aim-nrt.pratt.duke.edu/
* https://nrt.asu.edu/citizen-centered-smart-cities-living/
* https://nrt.unl.edu/
* https://nrt.catss.umn.edu/
* https://www.auburn.edu/cosam/climate_resilience/
* https://umaine.edu/conservationscience/
* https://dev.nrt.ua.edu/
* https://sites.google.com/stonybrook.edu/quads-nrt/home
* https://nrt.ku.edu/
* https://sites.udel.edu/midas-nrt/


### Project Board

To help coordinate updates, please see the site [Project Board](https://github.com/orgs/uhm-descartes/projects/1/views/1).
