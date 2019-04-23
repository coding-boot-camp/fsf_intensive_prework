# Lesson \#5 - Feature Branching

Part of working as a team is sharing code. Git and GitHub were created exactly for this purpose! Since software developers work in this collaborative manner, they need to leverage git effectively to share their code in as unobtrusive manner as possible.

Git is, by default, set up so that you push your changes directly into the `master` branch. 

The `master` is the default branch of your repository, and as its name suggests, is the master source for your project. 

As you might have guessed, we do not want to push directly to our master branch, and in fact, when working on a team, you likely will not have access to do so.

To get around this, we use a workflow called **Feature Branching**. The main idea behind feature branching is that all feature development should take place in a dedicated branch rather than pushing directly to the master branch. 

Here's how you can work in this kind of environment:

1. Create a new branch. 

2. Then, all changes to our repository (additions, modifications, or deletion) are made inside this branch. 

3. We then commit our changes, and push them to the remote source (GitHub). 

4. Once the branch has been pushed to the remote, we open a Pull Request. 

5. Once the Pull Request has been made, there will very often be automated tests that run to ensure that your modifications to not break the working application. 

6. Pull Requests also initiate a discussion about the changes you've committed, and generally have to be approved by someone else on the team. That person (or entire team) will review your changes to make sure that everything is in order. 

7. Once any concerns have been addressed and the Pull Request has been approved, the modified code is merged into the master branch. 

A great benefit of this process is that, once merged, Pull Requests act as a record of changes to the codebase, just like a save file!

<p align="center">
  <img src="https://raw.githubusercontent.com/coding-boot-camp/enterprise-prework-assets/master/assets/feature-branch.png" width="600" title="feature-branch.png">
</p>

To create a new branch:

1. `cd` into the repo directory
2. Create and switch to a new branch using `git checkout -b new-branch-name`
3. Make the changes to your repository that you desire
4. Stage the changes using `git add -A`
5. Commit the changes using `git commit -m "some message"`
6. Push the changes using `git push origin new-branch-name`
7. Navigate to your GitHub repository in your browser
8. On the `Pull requests` tab, create a new pull request

To switch between existing branches, you do not need the `-b` flag in your `git checkout` command.

To merge your changes into master, and update your local repository with those changes:

1. On GitHub, merge the Pull Request you created.
2. On your computer, switch back to your master branch using `git checkout master`
3. Pull the updates from the remote server with `git pull`