Before we can actually start coding, we need to get the codebase from the GitHub repository.
# What is a repository ?
*A repository is a place where code, files, folders are stored on GitHub.* For example, right now you're reading this md file on Blueprint's git-basic repository.
# Fork
Forking is when we're getting a clone of an existing repository owned by someone else into your GitHub list of repositories. So then any limited access restricted to that repository, now you have access to. The purpose of this is to make changes into your own forked repo then contribute back to the original repo.
## Upstream
A repository that we fork from is *upstream*
## Downstream
Our own repository that we forked is *downstream*

## Workflow
The workflow normally goes:\
changes -> downstream -> upstream

In order to accomplish this we need to setup our remote repo (upstream)
- To do so, do `git remote add upstream <repo_url>`\
where *repo_url* is the url of the forked repository.
- Then you can clone that forked repo into your device.

Typically in this case, when we have forked something, there are <u>two repository to consider</u> when we push changes
1. To push to upstream we do : `git push upstream`
2. To push to downstream (our forked repo) we do : `git push origin`
# Clone
Now to actually starting coding and making changes you'd obviously need a copy of the codebase in your computer.
- To do so you can run `git clone <repo_url>`, where *repo_url* is the url of the repo you're trying to clone.

Normally you want to fork then clone the forked repo and not directly the original repo unless you have access to that repo. 