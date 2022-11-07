# <center> How to host your resume on Github Pages </center>

This is for everyone who wants to host their resume on Github Pages.

## Purpose
The purpose of this project is to show how to use [Jekyll](https://jekyllrb.com/) (a static site generator), to host
your resume on Github pages. 
* Use Markdown to create your resume.
* Create a static website using Jekyll on your local computer.
* Use Github to host your resume online.




## Prerequisites     
* A [Github](https://github.com/) Account.
* A resume formatted in Markdown.
* A text editor of your choice.

## Instructions
 1. Write your resume on Markdown.
 2. Install Jekyll on your local computer.
 3. Pick your preferred Jekyll theme.
 4. Add your Resume to your local website.
 5. Host your website on Github.
 
### 1) Markdown resume.

 * What is Markdown?

   * Markdown is a lightweight markup language for creating formatted text using plain-text editor.
   
 * Formatting  a resume

   * A good formatting practice from Modern Technical Writing.
       *  Simple Content
	      * Make sure that your document is easy to understand and can be seen by someone skimming through the document by writing the main point as a header and then going into more detail under the header.
       


 
###  2) Installing Jekyll
#### What is Jekyll?
* Jekyll is a free and open-source static site generator and, can be used to build websites with rich and easy-to-use navigation.
#### Installing Jekyll
1. Download and install the latest version of [Ruby](https://rubyinstaller.org/downloads/).
2. A command line window will pop up when you are done installing. 
3. Press 1 and then enter to install MSYS2 base installation. 
4. Press 2 and then enter to install MSYS2 system update.
5. Press 3 and then enter to install MSYS2 and MINGW development toolchain.


  
3. Open a new command prompt window from the start menu, Install Jekyll Bundler using this command
```
 gem install jekyll bundler
```


![](https://github.com/Tellmore01/Tellmore01.github.io/blob/main/HowToInstallJekyll.gif)



### 3) Launching your website and changing the theme
* Creating a Jekyll project
1. Open the folder where you want to place your project.
2. Right click, then select "Open in terminal".
3. Run  ```  jekyll new [name] ``` in the cmd, this will create a folder with the specified name with the project.

* Launching the Jekyll project
1. Run ``` cd [name] ``` 
2. Run ``` bundle exec jekyll serve ```
3. Lastly copy the server address which is [http://localhost:4000/]() by default, and paste it in a browser to view your website.

* Changing the Theme

Now that you have hosted the website locally, you can change the website's theme.
1. Go to [RubyGems](https://rubygems.org/) and search for jekyll-theme-[Name].
2. Choose the theme and copy GEMFILE.
3. Open your project files, then open Gemfile and paste under ```  gem "minima", "~> 2.5" ```
it should look like this:
 ``` 
 gem "minima", "~> 2.5"
 gem 'jekyll-theme-hacker', '~> 0.2.0'
 ```
 
4. Open [RubyGems](https://rubygems.org/) again and copy INSTALL.
5. Open your project files and open _congif.yml and change the theme to jekyll-theme[Name]
it should look like this : 
``` theme: jekyll-theme-hacker ```
6. Open index.md and change layout to "default".
7. Change config.yml to match your info.
8. Now navigate to your project file again, right click and select "Open in terminal".
9. Run the following commands  ``` bundle install ```  then ``` bundle exec jekyll serve ```
10. Copy the server address and paste it on the web to check your website.

![](https://github.com/Tellmore01/Tellmore01.github.io/blob/main/JekyllLocalAndTheme.gif)

### 4) Adding your resume to your website
1. Open index.md and paste your markdown code for your resume below layout.
it should look like this:
``` 
layout: default
---
*** insert code here *** 
```
3. Add a title by typing title: Your title , it should look like this:
``` 
layout: default
title: Mostafa's Resume 
---
*** insert code here *** 
```
4. Navigate to your project your project file again, right click and select "Open in terminal".
5. Run the following command ``` bundle exec jekyll serve ```
6. Copy the server address and paste it to check your website.

![](https://github.com/Tellmore01/Tellmore01.github.io/blob/main/AddMyResToJekyll.gif)

### 5) Create a Github repository for your site
1. Open your [Github](https://github.com/) account.
2. Create a new repository by clicking on the green button with the name [username.github.io]
3. Click on select and existing file and select all the files in your project folder and click on the green commit changes button .
4. Now search username.github.io in the web to open your website.

![](https://github.com/Tellmore01/Tellmore01.github.io/blob/main/HostResumeOnGithub.gif)

### More Resources
* [Awesome README](https://github.com/matiassingers/awesome-readme).
* Check [Markdown tutorial](https://www.markdowntutorial.com/) for how to use Markdown.
* Modern Technical Writing, by Andrew Etter, can be found on [Amazon](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS).
* For more Jekyll themes checkout [Jekyll themes](http://jekyllthemes.org/).


### Authors and Acknowledgments
##### Reviewers:
* Ryan Dotzlaw
* Victoria Kogan
* Aqil Mukhi

A special Thanks to Nicke Manarin for the screen recording software, [ScreenToGif](https://github.com/NickeManarin/ScreenToGif).

### FAQ

Some frequently asked questions with answers.

* Why is the theme not working?
  * Make sure you change the layout to default in the index.md file.
* Why static websites?
  * As mentioned in Andrew Etter's book, static websites have no server-side application dependencies, no databases, and nothing to install.
* Why is Markdown better than a word processor?
  * It provides a simple, fast environment that lets you get straight to the writing.
  * It's easy to learn and the results are easy to read.
  * It gets rid of all the distractions of a formatting toolbar and mouse clicks, it also helps you to focus on your writing without lifting your fingers off of the keyboard.
  * It is also the most widely used lightweight markup language in the world and has the cleanest syntax as mentioned in Andrew Etter's book.

