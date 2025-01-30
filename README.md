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
6. <h3>Day2</h3> <br> <h1>Revert Changes</h1>
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
12. <h1>Branches</h1> it comes to branches