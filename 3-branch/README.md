# What are branches ?
We can think of branches as different versions of a file
## Normal flow
Normally, you can think of files following a linear flow like so:
![alt text](image.png)
- something like this, as we add changes our file would go through different versions\
A -> B -> C -> etc

Now doing this is fine we're just working on our own code, but when we involve others it becomes complicated\
Example:
- We're working on building a rubber duck and I'm working on the flaps part but my teammate added the tail. So now my version of the duck only has flaps and is behind. We could try to time our changes together but it becomes complicated and a hassle.

## How branching works
Instead of both of us working on the main version of the rubber duck, we can "branch" from the main rubber duck and work indepently on different duck features like flaps or tail. When we're both done, we contribute back to the main duck hassle free.

Example:
![alt text](image-1.png)

## Branching commands
**Make branch:**
- To create a branch you do `git branch <branch-name>`

**Switch to branch:**
- After you've created your branch, you can switch to it by doing `git checkout <branch-name>`

Now every time you make commits, if you're in a specific branch you'd be committing to that branch specifically and pushing to that branch too without affecting the main branch (sometimes called master).

If you want to get the latest version from main, then you'd do `git pull main`
- if you setup origin and upstream, then you'd do `git pull origin main`