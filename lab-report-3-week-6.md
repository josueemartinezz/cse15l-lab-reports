# <center>Lab Report 3</center>
---
## Josue Martinez 

A16943817
#### CSE 15L
####  5/08/2022

## <center>Streamlining ssh Configuration
I opened the configure file in VSCode by using the ``.ssh/config`` command in my command line prompt.
I changed the original addressed host from cs15lsp22 that was directed to me and chose an different alias seen below.
![configureFile](/R3Images/configureFile.png)

Thereafter, I used this new, shorter alias, "jogoto", to log into my account. Doing so successfully.
![ssh](/R3Images/ssh.png)

This meant that any commands that I had to previously address by the entire elongated host and hostname could now be used with this new alias. I did so by copying over a file from my local computer to the remote server account, jogoto.
![scpSS](/R3Images/scpSS.png)

## <center>Setup Github Access from ieng6</center>
Here, you could see the general location of my private key to access Github.com.
![private key](/R3Images/privateKey.png)
... and here's my general public key found on Github.
![public key](/R3Images/publicKey.png)

With these declared keys, I can now run certain commands that allow me to make changes to a file/files and push the change to Github. The commands that I used were: (``add, commit, push origin main``)
![git commands using git push origin main](/R3images/gitcommandsSS.png)
...and [**here**](https://github.com/josueemartinezz/markdown-parser/commit/253219e9079c1761ebd30d808d1d229057e0ea88) you can follow the link to see the commits that occured with the ``push origin main`` git command.

## <center>Copy whole directories with ``scp -r``</center>
In order to copy whole directories, I have to do so recursively to ensure each and every file within a directory is copied successfully as well. I did this using ``scp -r`` and below you can see the process of each content being copied over to my remote account. 
![localCopy](/R3Images/localCopy.png)
Here you can see the actual copied directory using ``ls``.
![serverCopy](/R3Images/serverCopy.png)
Finally, I combined the ``scp, ;, and ssh`` commands to do it all simultaneously. 
![compound commands at one time](/R3images/compoundCommand.png)
# <center>Thank you for visiting!</center>