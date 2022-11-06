# Borderline Website

This is the website for the Borderline Club at MIT. It is hosted on scripts.mit.edu.

## How to Update Website

1. Gain write access to this repository. Clone the repository onto your laptop.
```
git clone git@github.com:mitborderline/website.git
```

2. Make some changes to the website. Then when you are ready, update the GitHub repository with your changes:
```
git add -A 
git commit -m "made some changes to this website"
git push
```

3. SSH into [athena.dialup.mit.edu](http://web.mit.edu/dialup/www/ssh.html):
```
ssh <username>@athena.dialup.mit.edu
```
You'll need the password to your MIT account and then Duo to authenticate.

4. Make sure you have access to `/mit/borderline/`. In order to check, you should be able to run:
```
cd /mit/borderline/
```
without any problems. If you don't have access:

Ask a member of borderline to add you to the moira list `borderline-www` on [webmoira](https://groups.mit.edu/webmoira/). Once you are added, you should mount `/mit/borderline` onto your athena server by running:
```
attach borderline
```

Then run `cd /mit/borderline/` to go to the borderline folder. You should be able to see the live website code in the `web_scripts` folder (run `cd /mit/borderline/web_scripts`).

3. Update the live website with your changes. You may find these linux commands helpful:

Copy folder from local computer to remote server:
```
scp -r /path/of/your/local/folder username@hostname:/path/to/remote/server/folder
```

Copy a single file from local computer to remote server:
```
scp /path/of/your/local/filename username@hostname:/path/to/remote/server/folder
```

Copy entire folder to a directory ([ref](https://stackoverflow.com/questions/14922562/how-do-i-copy-folder-with-files-to-another-folder-in-unix-linux)):
```
cp -R path_to_source path_to_destination/
```

**Warning**: This is a **permanent** command!!
Remove file / Remove directory
```
rm -i file_name.txt
rm -rfI /path/to/folder/
```