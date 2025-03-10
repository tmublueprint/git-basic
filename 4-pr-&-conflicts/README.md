# Pull Requests
You've forked, created your branch and happy with your changes, now you want to contribute back to the original repo (upstream). Because upstream doesn't let you push directly into their repo, you have to do a *pull request*.\
But before we can do that, we need to make sure we have the latest version of upstream because others might've already made changes to it. To do so you can `git pull upstream`

From then you can perform a PR by typically going to upstream, and clicking the PR tab and drafting one. [instruction by GitHub here](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)

# Conflicts
Conflicts are when something goes wrong after trying to push your changes, the typical reasons are:
- pushing an older version of code (probably because you haven't pulled)
- you and one other person make changes on the same line of code
- renaming files or moving functions around

## Resolving conflict
Resolving conflict is complex and there's no one specific way to do it. A good approach is:
1. When conflict occurs, git will tell you which file is affected
2. Look at the difference and either keep your changes or keep the other change
3. `git add file-name`
4. `git commit`

## Other methods of resolution
There are other software out there for helping with resolving conflict, for now we'll do it traditionally, but in the future we may use something like [Meld](https://meldmerge.org/)