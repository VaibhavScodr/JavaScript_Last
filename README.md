# JavaScript_Last
<h3>Day1</h3>29/01/2025
i am starting javascript again for lastly
1. what is version control? <br>
it keeps trackes to your work or footprint over the process of making project and product
(to manage the version of the software)

#version control is always distributed becaus the changes are always being happend

2. stages of files or status? <br>
<ol>
  <li>modified</li>
  <li>staged</li>
  <li>commited</li>
</ol>
A. git local  <br>
1. check installetion -> open terminal -> git --version  <br> 
2. configure it with github ->go to github -> and in terminal config <br>
3. (a) git config --global user.email "----||----"  <br> (b) git config --global user.name "vaibhavScodr" <br> <br>
4.Now there are two ways to do this in order to work with github <br> (1) you can make the repo on the git hub and can clone it on the vs code by using <h3>git clone "--link--"</h3> <br>
(2) second you can do what that make your own diretory over the VS code and run and write everything on it than make it take it in the github by using <h3>git init</h3> 
also you can check it by using ls -a. <br>
5. Now becaus you have connected to the github and have proper connection so just make some handy command which are (a)git status--> git add .--> git commit -m "some msg"--> git push origin main.. <br>
6. <h3>Day2</h3>  <h1>Revert Changes</h1>
7. now for the back information of the git hub history or to see which are the new commits us command as <h3>git log</h3> <br>
the latest snapshot will be at head <h4>Head->main</h4> <br>
8. How can we revert the changes in the git <br>
there are three stages <pre>
               modified
                  |
                added
                  |
                commited
</pre>  <br>
9. Now at the level of modified use command <h3>git restore file.ext</h3> by this all modification will be reverted <br>
10. Not at the level of added you have to run command <h3>git restore --staged file.ext</h3> becaus it is staged or added it now go to the -->modified level then --> no changes <h3>git restore file.ext</h3> <br> 
11. Now at the level of commited you have to run command <h3>git reset --soft HEAD~1</h3> it takes you level to the added stage <br> also there are two types of git reset at the level of commit <br> 1. is <h4>git reset --soft HEAD~1</H4> <br>
2. is <h4>git reset --hard HEAD~2</h4> <br>
12. <h1>Branches</h1> it comes to branches <br>
13. brach is the pointer pointes to the latest commmit where my HEAD is. and the other branches are the part of the main branch which pointes to the diffrent diffrent snapshot's
14.  <pre> 
                                             (commit)--->(commit)---(commit)
                                                ^
                                                |
                                                |                          HEAD-->main
                                                |                              |
     (commit)--->(commit)--->(commit)--->(commit)--->(commit)--->(commit)--(commit)
                                     |
                                     |
                                     ^
                                  (commit)--->(commit)               
</pre>  it means the braches are the pointers which pointes to the commites andmain branch pointes to the latest commit by default and you start branches whereever commit you need to modified it.  <br>
15. For the list of the branches run command <h3>git branch</h3>   <br>
16. For the new branch run command <h3>git branch new_branch</h3>    <br>
17. For jumping on the new branch you made just nade <h3>git checkout branch_name</h3> <br>
18. other way by which we crete branch and automatically jump on it is <h3>git checkout -b new_b</h3> <br>
19. For delete the branch we use command <h3>git branch -d branch_name</h3>   <br>
20. For renaming the branch we use command <h3>git branch -m new_name</h3> <br>
21. Another concept is <h3>git stash </h3> by using this we can take the changes in modified file locally saved for use and when it is needed apply these to real changes <h3>git stash apply</h3>  <br>
22. <h4>Merge Branchs</h4>  i want to integrete tha work of all branch for production is known as merge <br>
23. Use command <h3>git checkout -b newb --> touch new.php --> git checkout main --> git merge newb --> git push origin main</h3>  <br>
24. Merge conflicts 