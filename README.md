#  How to host and format a resume using Jekyle

  

This is a step introduction to how to host and format a resume using Jekyll and the relationship between these steps and the general principles of current Technical Writing.

  

## Getting Started


### Prerequisites


Have a resume in markdown format.

- Example: [Resume.md](https://github.com/ZAn513/ZAn513.github.io/blob/main/Resume.md)

  

### Installing

  
#### 0. About Markdown

If you don’t have a resume in markdown format, check the link in More Resources. In Etter’s book, he said Microsoft Word is not a good choice for creating documentation, but Markdown is lightweight and has a clean syntax.

And you may use a Markdown editor online, also check the link in More Resources.

#### 1. Download and install VS Code from the website below (you may use other text editors):

	[https://code.visualstudio.com/download]

#### 2. Create a GitHub repository. (You need to have a GitHub account first.)

Go to your GitHub page and click the “New” button and name this repository:

	yourusername.github.io
![createRepo](https://github.com/ZAn513/ZAn513.github.io/blob/main/gifs/browseGHpages.gif)

#### 3. Go to the folder you want to store this project, and clone your repository using the command below:

	~$ git clone https://github.com/_username_/_username_.github.io

#### 4. Download Jekyll using the commands below:

	~  $  gem install bundler Jekyll

#### 5. Create a new folder.

	~  $  jekyll new myResume

#### 6. Go to that folder and run it for the first time.

	~  $  cd myResume

	~/my-awesome-site  $  bundle exec jekyll serve

Next time we can just use the command:

	~/my-awesome-site  $  jekyll serve

#### 7. Copy your Markdown format resume into the file named _index. md_ in your folder using any text editor (I used VS Code).

You can change the title of the website to “YourName Resume”.

![copyFile](https://github.com/ZAn513/ZAn513.github.io/blob/main/gifs/copyFile.gif)

#### 8. Now you can browse it.

Open your local browser and navigate to [http://localhost:4000](http://localhost:4000)
![browseLocal](https://github.com/ZAn513/ZAn513.github.io/blob/main/gifs/browseLocal.gif)

#### 9. Copy the files below into where you stored your project in step 2.

Index. md

_config.yml

#### 10. Commit and then push the changes to GitHub using these commands:

	~$git add --all
	~$git commit -m "Initial commit"
	~$git push -u origin main

#### 11. Now you can browse your resume using GitHub pages.

Open your local browser and navigate to: 

	yourusername.github.io
![browseGHpages](https://github.com/ZAn513/ZAn513.github.io/blob/main/gifs/browseGHpages.gif)
Now your resume has successfully appeared on your GitHub page.


### More Resources

a. [Markdown tutorial](https://www.markdowntutorial.com/)

b. [Etter, Andrew. Modern Technical Writing. Kindle edition, Self-published, 2016](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)

c. [Jekyll website](https://jekyllrb.com/)

d. [Mike Dane's Jekyll Static Site Generator Tutorial](https://www.youtube.com/playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB/)
e. [GitHub pages](https://pages.github.com/)
f. [A Markdown editor](https://pages.github.com/)
g. [VS Code](https://code.visualstudio.com/download)

## Concepts of Etter's Book

#### 1. Use Markdown.

>Etter suggests that Microsoft Word is not an ideal option for creating documentation, and instead recommends using Markdown. This lightweight format features a clean syntax and is easily compatible with various platforms and tools. Additionally, creating Markdown files is a simple process, and it is cost-efficient compared to Word, which requires payment and is only available on Windows and macOS. By utilizing Markdown, you can edit your documents anywhere and anytime, making it a convenient option for creating resumes or other documentation. In the More Resources section, you can find instructions on how to write a Markdown format file.

#### 2. Use a static website.

>According to Etter, if you want to create a more complex static website, you can use a generator like Jekyll. Steps 3-7 in the instructions involve installing and using Jekyll to create a static website. Static websites offer several benefits such as good speed, portability, and security. Additionally, they are easy to build and maintain, which makes them a practical option for creating websites. As per the instructions, you can simply copy your resume to the index.md file to complete the website and modifying it can be done directly through your GitHub repository.

>The advantage of static sites is that they do one thing and do it well, which is serving pages. If you want to enhance the appearance of your website, you can use themes in Jekyll. Moreover, there are other static site generators available, such as Sphinx, Hugo, AsciiDoc, Middleman, Metalsmith, MkDocs, and Hexo, which you can also consider using.


## Authors and Acknowledgments

-   **Zhiyin An** - Wrote the content of this README -

-  **Billie Thompson** - *Provided README Template* -

[PurpleBooth](https://github.com/PurpleBooth)
  


## FAQs

### 1. Why are we using a static website?


In Etter's book, he outlines several reasons for using a static website. Firstly, static websites are known for their speed as they do not have any server-side application dependencies, and therefore require minimal hardware resources to function effectively. Secondly, they offer a level of safety as there is no WordPress instance for potential hackers to exploit or comments section for bots to spam. Lastly, the simplicity of static websites lies in the fact that they do not require databases, which makes them easier to create and maintain.

### 2. Why is my resume not showing up in the link: [http://localhost:4000](http://localhost:4000)?

You need to use this command below in your terminal, the site will be visible on your local machine browser when you run this command.

	~/my-awesome-site $ jekyll serve