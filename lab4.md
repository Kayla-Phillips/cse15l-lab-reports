# Lab Report 4: Vim
## Step 4: Log into ieng6
* Keys pressed: ssh k3phillips@ieng6-201.ucsd.edu `<enter>`
* Commands used: A possible command to use for this step would be the up arrow to view bash history. However, I currently had no history.
## Step 5: Clone your fork of the repository from your Github account (using the SSH URL)
* Keys pressed: (Copy SSH link from GitHub) git clone `<cmd>` + v `<enter>`
* Commands used: In this step I used command v as a shortcut to paste the link from GitHub into my terminal.
## Step 6: Run the tests, demonstrating that they fail
* Keys pressed: ls `<enter>` cd cs `<tab><enter>` ls `<enter>` bash test.sh `<enter>`
* Commands used: In this step, I used ls and cd to locate the test script by listing the directories and files in the current directory and changing directory. I also utilized `<tab>` to auto-fill the directory name.
## Step 7: Edit the code file to fix the failing test
* Keys pressed: vim Li `<tab>` .java `<enter> <shift>` + `L` jjjjjjjlllllll r2 `<esc>`
* Commands used: In this step, I used `<tab>` to auto-fill the file name. I used `<shift>` + `L` to move the cursor to the bottom of my screen. I used j and l to finish moving the cursor to the spot of the error. Then, I pressed r2 to replace the current position with 2. 
## Step 8: Run the tests, demonstrating that they now succeed
* Keys pressed: :wq! `<up><up><enter>`
* Commands used: I used :wq! to save the file and exit vim. I then used the up arrow to access my bash history and rerun the test script.
## Step 9: Commit and push the resulting change to your Github account
* Keys pressed: git commit -a -m "Changed index" `<enter>` git push `<enter>`
* Commands used: I used -a which is an option for the git commit command to add all of the altered files to the commit. Then, I used -m to add the commit message. Then, I pushed the commit to GitHub using git push.
