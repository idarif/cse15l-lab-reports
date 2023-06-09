**LAB REPORT 4**
 - was not able to sign because forgot password and are no longer able to change it they way we were showed in the beginning of the quarter
- step 5  i pressed keys: `git clone <space> https://github.com/idarif/lab7`
![Image](lab4SS1Clone.png)

- step 6 showed that the tests failed
  keys pressed: `bash test.sh`
![image](lab4SSTstFail2.0.png)
  
 - step 7 edit code to fix errors
  typed in `vim Listexamples.java`
  after running that this code popped up 
  ![image](lab4SS3Edit.png)
  i changed index1 to index 2 by clicking keys `<up> <up> <up> <up> <up> <right> <back> <1>`
 - run tests after editing and compiling they passed
  i used keys: `$ javac -cp ".;lib/hamcrest-core-1.3.jar;lib/junit-4.13.2.jar" *.java`
  and `$ java -cp ".;lib/junit-4.13.2.jar;lib/hamcrest-core-1.3.jar" org.junit.runner.JUnitCore ListExamplesTests`
  ![image](lab4SSTstPass3.0.png)
  
  - step commit and push, 
  keys used: `git init` `<enter>` then `git status` then `<enter>` this is what showed up
   ![image](lab4SScomPU1.png)
   
   
  keys used: `git add ListExamples.java` `<enter>` then `git status` then `<enter>` this is what showed up
  ![image](lab4SScomPU2.png)
  
  after that  ityped in `git commit` then in the vim page pressed `i` to start editing and wrote the message
  `<"Adding the file named ListExamples.java">` then clicked `<esc>` then `<:wq> <enter>` and this is what showed up
  
 ![image](lab4SScomPUcom.png)
 
 
 i then tried making a key and push the repository i was able to commit the changes but was having trouble pushing it even after making a key following thr step in the lab tasks
 - i typoed ssh-keygen and got this i then copied `/c/Users/ilyas/.ssh/id_rsa.pub`

 ![image](lab4SSHKey.png)
  - then did `cat /c/Users/ilyas/.ssh/id_rsa.pub` 
  - then `ssh-keyscan -t rsa github.com >> ~/.ssh/known_hosts`
  - then did `ssh -T git@github.com`
  - and got this
  ![image](lab4SSKeySteps.png)
  then when i tried pushing i got these errors
  after i typed 
   - git remote add origin https://github.com/idarif/Lab-Report-4.git
   - git push origin main
   - git push
  
  ![image](lab4ssPushFail.png)
