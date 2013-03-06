#Task0: Setting up github

Check list

Create an account in [https://github.com]

Prepare your private / public keys. For this step, first look if you already have a private / public keys. For this

    $ ls ~/.ssh/id_rsa*

If the output of the above command gives
    
    id_rsa
    id_rsa.pub

Then you have your keys. If it gives you *No such file or directory* error then you should create your files using the following command
    
    $ ssh-keygen -trsa

This command should create the two files above. Make sure they exist now.

**Setup public key in github.**

Login to Github. Go to upper right 'Account Settings' link. Then go to SSH-Keys on the left. Click on **Add SSH Keys** link. Make sure to execute the command mentioned there or copy paste the contents of ~/.ssh/id_rsa.pub file here.

Participate in the project kam-tamam [https://github.com/bibstha/kam-tamam].

Clone the repository

    $ git clone git@github.com:bibstha/kam-tamam.git
    $ cd kam-tamam

Create a random file inside **temp** folder and do first commit

    $ cd temp
    $ echo "This Is My File" > temp/myname.txt
    
You just created your first temp/myname.txt file. You now need to do following steps

    $ git status
    $ git add temp/myname.txt
    $ git commit -m 'Created my first file inside temp folder'
    $ git pull origin master
    $ git push origin master

What do these commands do?

**git status** Helps you see what files are modified or what files were new. You should
see that your file **temp/myname.txt** listed in the section **untracked files**.

**git add temp/myname.txt** adds your file so that git can start tracking the file.

**git commit -m "message"** means you now save what you did. It gets saved inside the
**kam-tamam/.git** folder which is a special folder.

**git pull origin master** trys to see if there are any changes from other users before
you send your changes.

**git push origin master** pushes all your edits and your new files to the server where
you cloned your file from.

Once you are done with the above steps, go to [https://github.com/bibstha/kam-tamam] and
go inside temp folder. You should be able to see your file there.

If you edit your file once again, do the steps above completely again. You should be able
to see your changes in the github as well.

This way other people can keep track of what you have edited or created.
