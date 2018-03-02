This repository is just to test how to use R and Rmarkdown to create a website hosted on GitHub pages. The website created by the files in this repository is at: https://daltare.github.io/Webpage_RMD_Test/

None of the content in the site is my own. All of the content was taken from an RStudio webpage, and slightly reconfigured to work with GitHub pages - the source is here: https://rmarkdown.rstudio.com/demos/12-website.zip (linked from the page here: https://rmarkdown.rstudio.com/lesson-13.html)

The changes I made to reconfigure the template files above in such a way that they'll work in GitHub pages include:
* add the file names `.nojekyll`
* within the `_site.yml` file, add (or modify) the following line: `output_dir: "."` (note that it may be preferable to use: `output_dir: "docs"` instead, as GitHub pages will support that - need to double check to be sure though). NOTE: do this before working with the files within Rstudio to render the files into a website format.

To convert the original set of files into a webpage using GitHub pages, first use Rstudio to render the source files into a website (open the website.Rproj file, then under the **Build** tab in the pane with **Environment, History...** click on the **Build Website** button; this will render all of the .md and .rmd files into html files structured as a website). Then add the whole project to a new GitHub repository, go to the **Settings** tab for the repository, scroll down to the **GitHub Pages** section, and set the source to **master branch** (or **master branch /docs folder** if using that option above).

More detailed instructions on how to create a website with Rmarkdown are available here: http://rmarkdown.rstudio.com/rmarkdown_websites.html

I also tried to learn from other GitHub pages that appear to have been made with R, for example:
* https://inbo.github.io/dwc-in-R/ (repo: https://github.com/inbo/dwc-in-R)