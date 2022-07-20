# blog-jobtracker
News &amp; Articles about NRP 77 Jobtracker

## Website Administration

This website uses quarto and GitHub Actions to publish information on a GitHub Pages site. In order to lower waiting time and dependencies, this site uses quarto's [freeze option](https://quarto.org/docs/publishing/github-pages.html#freezing-computations). 

This means the code is NOT executed on GitHub and computations need to run locally. We do so because
1) we do not mean to change blog posts once published. 
2) after years there may be quite some requirements that are hard to fulfill in order to re-render the post and therefore the entire blog. 
Note that we can unfreeze specific posts if reproducibility through GitHub Actions is important for a specific post.


### Basic Update (no code in post)

- make edits locally (or online on GitHub for smaller edits)
- git add, git commit, git push


### Updates with computations

- run `quarto render`
- git add files INCLUDING `_freeze` folder, git commit, git push


## Output

pushing to GitHub will trigger a GitHub actions pipeline that re-renders and publisches to https://kof-ch.github.io/blog-jobtracker/



