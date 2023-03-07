#  How to host and format a resume using Jekyle

  




This is a step introduction to how to host and format a resume using Jekyll and the relationship between these steps and the general principles of current Technical Writing.

  

## Getting Started


### Prerequisites

  



Have a resume in markdown format.

- Example: [Resume.md](https://github.com/ZAn513/ZAn513.github.io/blob/main/Resume.md)

  

### Installing

  
#### 0. About Markdown

If you don’t have a resume in markdown format, check the link in More Resources. In Etter’s book, he said Microsoft Word is not a good choice for creating documentation, but Markdown is lightweight and has a clean syntax.

#### 1. Download Jekyll using the commands below:

	~  $  gem install bundler Jekyll

#### 2. Create a new folder.

	~  $  jekyll new my-awesome-site

#### 3. Go to that folder and run it for the first time.

	~  $  cd my-awesome-site

	~/my-awesome-site  $  bundle exec jekyll serve

Next time we can just use the command:

	~/my-awesome-site  $  jekyll serve

#### 4. Now you can browse it.

Open your local browser and navigate to: [http://localhost:4000](http://localhost:4000)

Etter said, to create a more complex static website, we can use a generator like Jekyll.

5. More Resources

a. [Markdown tutorial](https://www.markdowntutorial.com/)

b. [Etter, Andrew. Modern Technical Writing. Kindle edition, Self-published, 2016](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)

c. [Jekyll website](https://jekyllrb.com/)

d. [Mike Dane's Jekyll Static Site Generator Tutorial](https://www.youtube.com/playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB/)


## Authors and Acknowledgments

-   **Zhiyin An** - Wrote the content of this README -

-  **Billie Thompson** - *Provided README Template* -

[PurpleBooth](https://github.com/PurpleBooth)
  


## FAQs

### 1. Why are we using a static website?

According to Etter’s book,

a. Speed: Static websites have no server-side application dependencies. The server needs very few hardware resources.

b. Safety: There’s no WordPress instance for someone to hack or comments section for bots to spam.

c. Simplicity: No databases.

### 2. Why is my resume not showing up in the link: [http://localhost:4000](http://localhost:4000)?

You need to use this command below in your terminal.

	~/my-awesome-site $ jekyll serve