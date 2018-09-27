# About
Codebase for the Pasadena Complete Streets Coalition website

### Software requirements (these are all free)
- [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) - to keep track of and upload changes
- [Ruby](https://www.ruby-lang.org/en/downloads/) - language used to run jekyll
- [Jekyll](https://jekyllrb.com/) - our static content management system (CMS)

Github/gitpages runs jekyll on the server. The advantage of having Ruby and Jekyll on your local machine (computer) is being able to locally preview the site as you work on it.

### How to contribute
0. Become a member of PasadenaCSC and the pas-csc github group (it's free. and we can teach you.)
1. Install the above software/packages on your computer.
2. "Clone" this repository onto your local machine. 
  - (Optional) Read background: [https://help.github.com/articles/cloning-a-repository/](https://help.github.com/articles/cloning-a-repository/)
  - Run command: ``git clone https://github.com/pas-csc/website.git``
3. Write code (see: https://guides.github.com/activities/contributing-to-open-source/)
4. Commit your code, and push the changes to the server.

### How this site works
- We're using jekyll as the content manager, and [twitter bootstrap](https://getbootstrap.com/docs/4.0/getting-started/introduction/) for the front-end design.
- Most posts are formatted using a combination of [Markdown](https://daringfireball.net/projects/markdown/) and HTML. Skewed toward Markdown for the plain text, and skewed toward HTML for the fancy-pants sub-sites with more complicated layouts.
- Blog posts are in the '_posts' directory. All files should be in .md format, in Markdown, and titled YYYY-MM-DD-[Your Title].md
- Event pages are in the '_events' directory. All files should be in .md format, in Markdown, and titled YYYY-MM-DD-[Event Name].md
- Static pages (that have basic information that doesn't change often) are in the '_pages' directory, just to keep things clean.