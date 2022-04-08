# How to *Remotely* log-in to your ieng6 account
First make sure that you have done the prerequiste for the lab by changing your password

We will start by opening vs code and opening the terminal
It should look a little something like this
<!--- add picture of VSCODE terminal here-->

Once completed we can log into our account

Copy this code with your account name
cs15lsp22abc@ieng6.ucsd.edu
__Note: use your account, it most likely wont be abc__

It should prompt you for a password 
<!-- ask for password image-->
Type in your password and it should look like this!

__Note: The computer isn't going to make little asteriks when you type your password. It will look blank. Just type in your password and press enter when done__

Once you've logged in the computer should output a big wall of text and look like this.

<!-- Insert that image here-->

Once inside we can try some commands
Here are some of my recommendations
- cd
- ls
- cd perl5
- cd ~

After I run these commands this is what my terminal looks like, see if yours matches
<!---  add image of this part ig-->

Now were going to learn how to copy and move files over using `scp`

Create a file in VS Code called `WhereAmI.java`

Once created just copy this code down

<!-- add image of the code-->

after running the code using the javac and java commands lets try to move this over to our account

Type this command into the terminal

scp WhereAmI.java cs15lsp22zz@ieng6.ucsd.edu:~/

Once you're logged in type `ls` and you should see your file in your account!

<!--- add image of this --->

Typing your password can get a little annoying :(

Theres an awesome solution to this problem that is ssh keys

ssh keys in the grand scheme of things creates a private key and a public key that allows easier access into your server account

Lets start by opening the terminal on your client computer

Type this code in 

ssh-keygen

Your computer should load up something like this

__Note: When you get to the paraphrase part DO NOT type anything just press enter__

<!--- add image here -->

If we try logging into the server now you should gain access without having to type a password






