# <center> How to host your resume on Github </center>

This is for everyone who wants to host their resume on Github Pages.

# Purpose
The purpose of this project is to show how to use [Jekyll](https://jekyllrb.com/) (a static site generator), to host
your resume on Github pages. 
* use Markdown to create your resume.
* Create a static wesbite using Jekyll on your local computer.
* use Github to host your resume online.




# Prerequisites     
* A [Github](https://github.com/) Account.
* A resume formatted in Markdown.

# Instructions
 1. Write your resume on Markdown.
 2. install Jekyll on you local computer.
 3. Pick your prefered Jekyll theme.
 4. Add your Resume to your local website.
 5. Host your website on Github.
### 1) Markdown resume.

 * what is Markdown?

   * Markdwon is a lightweight markup language for creating formatted text using plain-text editor.
 * why Markdown?
    * Markdwon gets rid of all the distractions of a formatting toolbar and mouse clicks, it also helps you to focus on your writing without lifting your fingers off of the keyboard.
    * Markdown is also the most widely used lightweight markup language in the world and has the cleanest synatx as mentione in Andrew Etter's book.
### 2) Installing Jekyll
#### what is Jekyll?
* Jekyll is a free and open source static site generator and, can be used to build websites with rich and easy-to-use navigation.
#### Installing Jekyll
1. Download and install [Ruby](https://rubyinstaller.org/downloads/)
2. Type the following when asked by Ruby cmd
  * ```
    1
    ```
  * ```
    2
    ``` 
   * ```
     3
     ```
*  ```
   Enter
   ```

  
3. Open a new command prompt window from the start menu, Install Jekyll and Bundler using this command
```
- gem install jekyll bundler
```


![](https://github.com/Tellmore01/Tellmore01.github.io/blob/main/HowToInstallJekyll.gif)



### 3) Launching your wesbite and changing theme
* Launching your wesbite
1. Open the folder where you want to place your project.
2. Right click, then select "Open in terminal".
3. Run  ```  jekyll new [name] ``` in the cmd, this will create a folder with the specified name with the project.
4. Then run ``` cd [name] ``` 
5. Lastly run ``` bundle exec jekyll serve ```
6. Copy the server address and paste it to check your website.

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
 
4. open [RubyGems](https://rubygems.org/) again and copy INSTALL.
5. Open your project files and open _congif.yml and change the theme to jekyll-theme[Name]
it should look like this : 
``` theme: jekyll-theme-hacker ```
6. Open index.md and change layout to "default".
7. Now open your project file again, right click and select "Open in terminal".
8. Run the following commands  ``` bundle install ```  then ``` bundle exec jekyll serve ```
9. Copy the server address and paste it on the web to check your website.

![](https://github.com/Tellmore01/Tellmore01.github.io/blob/main/JekyllLocalAndTheme.gif)

### 4) Adding your resume to Jekyll
1. Open index.md and paste your markdown code for your resume below layout.
2. Open your project file again, right click and select "Open in terminal".
3. Run the following command ``` bundle exec jekyll serve ```
4. Copy the server address and paste it to check your website.

![](https://github.com/Tellmore01/Tellmore01.github.io/blob/main/AddMyResToJekyll.gif)

### 5) Create a Github repository for your site
1. Open your [Github](https://github.com/) account.
2. Create a new repository by clicking on the green button with the name [username.github.io]
3. click on select and exisiting file and select all the files in your project folder and click on the green commit changes button .
4. Now search username.github.io in the web to open your website.

![](https://github.com/Tellmore01/Tellmore01.github.io/blob/main/HostResumeOnGithub.gif)

### More Resouces
* Check [Markdown tutorial](https://www.markdowntutorial.com/) for how to use Markdown.
* Modern Technical Writing, by Andrew Etter, can be found on [Amazon](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS).
* For more Jekyll themes checkout [Jekyll themes](http://jekyllthemes.org/).

### Authors and Acknowledgments
* [Awesome README](https://github.com/matiassingers/awesome-readme)


### FAQ
* Why is the theme not working?
  * Make sure you cange the layout to default in the index.md file.
* Why static websites?
  * As mentioned in Andrew Etter's book, static websites have no server-side application dependencies, no databases, and nothing to install.
* Why is Markdwon better than a word processor?

 To be Answered.


