# Git Assignment - michelberger-a

a. What is an issue?
An issue can be used to track to do lists, bugs, requests and quite literal "issues" in the code. Issues are structured in which they will appear in list form, making it easy to approach and understand from a problem solving session. Issues can be created and read within GitHub. As mentioned in the lesson, one class participant described an issue, similar to an IT Ticket.  
In an issue, some information is required to be filled out. A title for the issue is needed, and a description. The description will usually contain the checklist and other additional information that deems an issue to be resolved. Alongside this, you can add Assignees - other people/users that can review the work. You can add labels - a way to tag the issue with certain categories. You can add Projects - by assigning the issue to a specific project within the repository. Then there are Milestones - a way to mark progress within an issue and project.  
When you are satisfied with the issue, you can click the green button at the bottom to submit the issue. 

b. What is a pull request?
A pull request is a request used as a potential merging of files from one branch to a destination branch (usually main). The capabilities of pull requests allow teams/users to resolve issues, bugs, or edit the code and save the work in a separate branch, so that the main code is unaffected. Other users/team members can review the code, and once the consensus finds the code is plausible, the branch can be merged into the main branch.  
A pull request has its own tab on the repository page in github. Within each pull request, there are several features to consider. Within each request, you can see the "start" of the request, and the subsequent commits with the summary message(s). Additional features as listed above, Reviewers, Assignees, Labels etc. can be included in the pull request. Although a pull request can be created, it does not mean it has been applied, until the "Merge Pull Requst" button at the end has been clicked. This will allow the merging of the files/code from the branch into the target branch.

c. Describe the steps to open a pull request?

Setting Up the Branch and File(s)  
- You fill first need to select a repository of interest and create a branch as a copy of the main branch. This step can be completed through GitHub
- You will need to clone the repository url to access files. Move into the git directory you've set aside for this work. Also create the new branch on your local computer to edit the files through
- Once this is setup, edit your files, then stage (add) the file, commit, and push to GitHub (see steps below)
- As a reminder, this push should be directed at a branch which is NOT the main

git checkout -b <new-branch-name>  
code <file-name.extension>  
#save changes  
git add -A  
git commit -m "update commit message here"  
git push  
#if the branch is new, you may receive an error and will need to use this code to push to the stream  
git push --set-upstream origin <new-branch-name>  

now you can check if the files edited have been updated

Creating the Pull Request  
- On GitHub, go to the repository you have been working in
- Along the top ribbon of the screen, click into "Pull Requests"
- In the top-right corner, click the green button "New pull request"
- Along the top of the new page, under compare changes, two new drop down boxes have appeared with an arrow inbetween. This arros shows the directionality of the merging files
- In the first box, base:, select the main branch of the repository (or the target branch) 
- In the second box, compare:, select the branch you have pushed edits and changes too (typically the branch you defined earlier)
- Lower on the screen, there will be a panel displaying the changes made across the merge. You can review these changes and then select "Create pull request" in the top right corner
- In the new page, you can edit the title of the pull request, and should provide a description of the pull request. This description should explain the details of changes, and other related information. 
- In addition to the title and description, more information can be provided. This includes, again, Reviewers, Assigned, Labels, Projects, and Milestones, all as different tages to get users to review or categories the pull request. 
- Review the rest of the page, including the summary of previous commits for the two branches involved in the pull request
- Once statisfied, you can click the green button "Create pull request"
- Now another new page will appear. This will summarize the details involved in the request, using the information provided in the previous steps. Yourself and other users can review this information and then confirm the request to merge the information within the identified branches. 


d. Describe the steps to add a collaborator to a repository (share write permissions)

- To start the process of adding a collaborator, you will need to find the repository within your GitHub account you would like to share. 
- Along the ribbon at the top of the screen, select the "Settings" box with the gear icon
- On the new page, there is a panel on the left hand of the screen, the first option under General is Collaborators. Click there. 
- The page will update to show "Who has access" and a panel underneath with a green box that says "Add people". Click that button
- A pop-up will appear that allows you to search for users by username, full name or email. Use this box to identify the collaborator you'd like to add
- Click on their name when it appears, and then click the green button that says "Add <user-name> to this respository"
- That user will receive an email invitation to join the repository. Once they accept, they will be able to collaborate on the repository. 

Please ensure you do not follow the steps to add a person to a personal project. The add a collaborator steps are slightly different including determining their level of access (read/write/admin).


e. What is the difference between git and GitHub?

Git: is a version control system. It can track changes of files/code that is being edited. It is a command-line tool that can be used on the local computer but connect with repositories on GitHub. Git is an effective and efficient version control system. When using Git to track changes, it will only update files that have had edits. Through Git, you can created branches off a GitHub respository, edit the files, push changes back to the branch and track the changes. This will allow easy collaboration between team members and other collaborators involved. 
Git uses a check-summing mechanism to track changes which is effective in storing data and making it difficult to have untracked changes, similar to blockchain. Git can access files through three states, Committed, Modified and Staged. The workflow in Git involves three steps. First to modify the files in the working directory. Second, to stage files in a staging area. Third, to commit the changes to a directory. 

GitHub: is a platform that can be found online or through a desktop based app. This platform allows collaborators, scientists, developers and any other data enthusiasts to store code and files. Many projects on github are publicly available. GitHub integrates functions of Git such as change tracking version control. 

Differences:
- Git is a software (language), GitHub is more of platform/service that can store files, code but uses Git functionality
- Git is a command line program, GitHub is an online service with a nicer interface and user friendly experience compared to git
- Git is used for version control and file editing, GitHub stores projects and code in organized repositories, branches etc. (which can be edited as well)
- Git is used on the local computer, GitHub is used through online web-services (but there is a desktop app that can be downloaded)
- Git is free to use and can be used on practically any computer without complications, GitHub needs internet and an account signup, GitHub also has an availabe paid platform
- for changes Git requires a workflow process of git add, git commit and git push, in GitHub, changes can be made directly online and saved like typical word files (although a similar process to Git) and introduce pull requests, issue tracking, actions, and adding collaborators for a project-based approach

f. What does git diff do?

git diff can be uses to show changes between commits and branches. It will allow you to compare and contrast changes between commits at different steps, or between branches within a directory. 

If you add a path file after git diff, the changes for that specific file will be highlighted in green and red lines. With the option --staged, this will show the changes in the staging area after using git add to beging the process of pushing changes. 

You can also compare two branches through git diff. After entering git diff, if you type out the two branches to compare, separating their names by a space, you will see the changes between the two branches. Similarily, if you extend the file path to include specific file names, those will also display the change made. 

Overall, git diff will preview changes made between files or branches, prior to a full add, commit and push workflow. 

g. What is the main branch?

The main branch is often the "central" or default branch as the primary host of files and code for a project. The main branch is usually where the "good copy" of the files are stored as they will be used for professional based projects between collaborators. Semantic models can be designed to display the relationship of additional branches to the main branch. 

The main branch, sometimes referred to as the central or master branch will store the project ready files. This is often where final/good copy files are pushed too. Collaborators may make copies/create branches of this main branch to re-design, edit and experiment with files/code. If satisfied, users will create pull requests, to merge experimental branch files to the main branch, after careful review and consideration from other collaborators. Many of these branches will follow specific naming conventions, according to the team and project, to highlight what the branch is being used for. Often times, the main branch is protected, meaning files cannot be merged into the branch through pull requests until they pass outlined requirements, such as two reviewers to confirm. Often, these steps are included in a workflow. Certain steps must be completed in different branches before they can be merged to the main.

The central/main branch is important to maintain clean and organized files. This allows teams to succeed in project development and avoid conflict. 


h. Besides our initial commit if it is a new repository, should we directly push our changes directly into the main branch?

It is among a best practice to NOT push changes directly to the main branch. Every team/project may have their own standards, but branching is a strategy that allows collaborators to tweak and experiment codes/files, and store without creating conflict. 

With branching, a user is free to experiment with code and will not put the overall project code at risk. This will allow other collaborators to review code/files and open discussion about edits. This will help prevent merging files with errors or bugs into the main branch. Testing may also occur to check the code for correct outputs, such as autograder tools reviewing correct answers to questions. Aside from the code, this strategy may prevent project conflicts and disagreements between collaborators. 

With completion and review of a branch. A pull request can be created to merge files from the side branch to the main branch. Once again, a process can be created allowing collaborators to review changes, completion of a checklist, and editing of changes prior to a merge to the main branch. Main branches may be protected by rule sets to allow a side branch to merge to the main branch. 

Overall, changes should be pushed to a side branch instead of the main branch. This will provide opportunity for collaborators to review code to ensure it is appropriate. A strategy involving the creation and review of side branches will help avert workplace conflicts. 