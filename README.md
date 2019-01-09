# LMX2487e
PLL device test program general guidelines

 Just testing........	All software development happens in branches which are later merged into the master branch. Master branch is expected to always be in releasable condition. Merging to master requires you to make a pull request from your branch to master and have it accepted in a code review by at least one other person.

 General workflow:

 1. Create an issue ticket for the task you are implementing
2. Add the issue ticket to the 'nRF91 SiP module test program development' project in the Projects tab.
3. Create a branch for the issue.
   - 'git checkout master'
   - 'git pull'
   - 'git checkout -b branch-name-ticketnumber'. The branch name should be the same as the header of the issue ticket with space replaced by -. So for example 'Create usage guidelines' with ticket number #1 turns to a branch named 'Create-usage-guidelines-1'
4. Move the issue ticket to 'In progress' status under 'nRF91 SiP module test program development' in the projects tab.
5. Develop the new code in your branch
6. Commit your changes to the branch, 'git commit -a -m "Commit message"'.
7. Push your changes to the remote server by doing 'git push'
8. Create a pull request(PR) for your branch. Set reviewers for the PR.
9. After PR has been accepted by at least one reviewer and you believe it is ready to be merged, merge the PR to master.
10. Move the issue ticket to 'Done' status under 'nRF91 SiP module test program development' in the projects tab.

 It is preferable to have an issue ticket to every task.

