# Getting Started with git
This assignment will go over the `git` commands and workflow we covered in lecture 2. The workflow is laid out for you step-by-step, but the exact commands are not given to you upfront--feel free to use google, git cheatsheets, [class notes](https://github.com/mlp6/Medical-Software-Design/blob/master/Lectures/GitFundamentals.md), etc to help you through this. The more you use the `git` workflow, the more you'll remember the common commands. 

## Assignment
You will be creating a "feature" in this repository, which will consist of you adding a file to this repository containing basic information about yourself using the feature-branch workflow. 

### Part 1
* Clone this repository to your `local` machine. By default you are on the `master` branch.
* Create a new branch (off of master) to implement your feature. *Name this branch in a descriptive way.* Example branch names: `add-new-button` `sk/add-submit-button`, `sk317/update-readme-links`. Note that often times a personal identifier (like `sk` or `sk317`) is added in front of your branch name.
* Create and **commit** an empty file called `info.csv` to your branch. Be sure to have a [good commit message](https://chris.beams.io/posts/git-commit/#seven-rules).
* Now populate `info.csv` with a single line that contains your `first_name, last_name, netid, full_duke_email, github_username` in a comma seperated format:
  ```csv
  Suyash, Kumar, sk317, suyash.kumar@duke.edu, suyashkumar
  ```
* Commit this change to your feature branch
* Push your `local` branch to the default `remote` (called `origin`). 
* You should now be able to see your branch on Github (which is the `remote` in this case)
* :eyes: Typically you would now create a "pull request" and have your feature changes undergo a code review. For now, we will skip ahead to the next part which is **merging your feature branch changes back into the master branch**. 
* On your local machine use `git merge` to merge the changes you made in your feature branch onto your master branch. 
* Now that your master branch has been updated with your new feature changes, go ahead and `git push` your updated master branch to the default `remote` (also called `origin` which is Github in this case)

### Part 2
Your task for Part 2 is to edit this README to add an image of your favorite plant or animal. Don't forget about the Markdown cheatsheet [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) to learn more about syntax for adding images.
* Create a GitHub issue (task) by clicking on the issues tab of the repository up top and hitting "New Issue"
* Describe the task you are about to complete and create the issue to track the task.
* :eyes: NOTE that the issue gets a number, in this case `#1`. You can use this to refer to this particular issue from anywhere in your repository.
* :eyes: NOTE: Github issues __only__ live on GitHub, they don't ever get pulled down to your `local` machine. They aren't really a git thing, they are a __GitHub__ feature. 
* On your local copy of the repository go ahead and create a feature branch to complete the task of adding an image of your favorite plant or animal to this README. Be sure to name the branch well as described above.
* Go ahead and complete the task and commit to your branch, and push to `origin`.
* Open a Pull Request
* Be sure to include the following text in your pull request description: `closes #1`, which will ensure that issue #1 is closed when the Pull Request is merged.
* Merge in the pull request to master. 
