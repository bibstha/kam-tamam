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

Create a random file inside **temp** folder and do first commit
