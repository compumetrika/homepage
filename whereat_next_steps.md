Where at: 



# Where At

Ok, just switching to doing the [first version](https://gohugo.io/tutorials/github-pages-blog/):

## Deployment via /docs folder on master branch

As described in the GitHub Pages docs, you can deploy from a folder called docs on your master branch. This requires to change the Hugo publish directory in the site config (e.g. config.toml):

    publishDir: "docs"

After running hugo, push your master branch to the remote repo and choose the docs folder as the website source of your repo (in your GitHub project, go to “Settings ” -> “GitHub Pages” -> “Source” -> Select “master branch /docs folder”). If that option isn’t enabled, you likely haven’t pushed your docs folder yet.

This is the simplest approach but requires the usage of a non-standard publish directory (GitHub Pages cannot be configured to use another directory than docs currently). Also the presence of generated files on the master branch may not be to eveyone’s taste.






# Previously:

working through:

    https://gohugo.io/tutorials/github-pages-blog/

at this section: 

Building and Deployment

Now check out the gh-pages branch into your public folder, using git’s worktree feature (essentially, it allows you to have multiple branches of the same local repo to be checked out in different directories):

    rm -rf public
    git worktree add -B gh-pages public upstream/gh-pages

Getting this error from second command:

    fatal: Refusing to point HEAD outside of refs/

Googled this: "github error fatal: Refusing to point HEAD outside of refs"



