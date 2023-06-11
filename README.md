# Introduction-to-Git-and-GitHub
cloudskillsboost.google


Task 6. Create a GitHub repo
If you're the sole owner of your project, you don't need to use GitHub. But if you're on a team, you can use GitHub to collaborate without stepping on each others' toes.

To create a new repo on GitHub, go to github.com and log in.

In the left pane, in the Repository section, click New.

GitHub will ask you for some basic info about your repo.

Fill out the form, then click Create repository.
GitHub will ask you if you want to start from scratch or add a local project. Since you just created a new repo, you want to push that to GitHub.

Follow the "...or push an existing repository from the command line" section and then copy the GitHub repo URL.

Return to your SSH window and run the commands:

git remote add origin <your GitHub repo URL>
git push -u origin master
  
The first command adds the local repository to your GitHub repository.
The second command pushes your local repo to GitHub.

  
  Task 7. Push a branch to GitHub
Pushing the commit in your branch to your new GitHub repo allows other people to see the changes you've made (think code review). The repository's owner can review changes prior to merging to the master branch.

Run the following command to push changes onto a new branch on GitHub, replacing branch name with a name of your branch:

git push origin <your branch name>
Copied!
Does GitHub automatically create the branch for you on the remote repository?

In GitHub, click on the Code tab. You should now see the branch name you just pushed.

Click the Compare & pull request button that is next to your branch name.

You'll now see the name of your commit. In a production environment you could leave a comment about this commit.

For this lab click Create pull request.
GitHub verifies that the files you are adding aren't in conflict with the Master copy. If everything checks out, and it should since these are new files, you will see a green check mark.

Click Merge pull request, then Confirm merge.
You'll see a "Pull request successfully merged and closed" message.

At this point you can click the Delete branch to clean up. You don't have to do this, but you may end up with a mess if you have too many branches. Notice that you'll have another chance to leave comments.
  
  
  Task 9. Create a Pull Request
Now that you have added your updates, you need to notify a repo's owner that you want to make changes to their files through a pull request. A pull request (PR) allows them to review your changes to make sure it looks good before putting your changes on the master branch (which are documentation updates in this use case, but could also be code changes or any number of other cases).

Since you are the sole owner of your repo for this lab, you don't have to create a PR to merge your changes, but it's a good idea to create one anyway to track the history of your updates.

Create your PR in GitHub
Return to your GitHub window.

Open a pull request by clicking the Pull requests tab, then New pull request. Pull requests tabbed page with New pull request button highlighted

In the Compare and review section, click on your branch name.

You'll be shown what changed in the file that you're adding to Master.

Click Create pull request.
You'll see the name of the second commit you created.

Now click Create pull request.
GitHub verifies that your changes are good.

Click the Merge pull request to add your changes into the master branch.

Click Confirm merge.
