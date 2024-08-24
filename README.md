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

Please ensure you do not follow the steps to add a person to a personal project. The add a collaborator steps are slightly different including determining their level of access (read/write/admin)


e. What is the difference between git and GitHub?

f. What does git diff do?

g. What is the main branch?

h. Besides our initial commit if it is a new repository, should we directly push our changes directly into the main branch?