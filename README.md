# demo-repo

## Main concepts


directory -> folder
terminal comand line interface text commands
cli comand line interface
cd change directory
code editor word processor for writing code
repository - procject or folder where your project is kept

git  - tool 
git hub - website

## Main commands

git clone   -
git status
untrackted file means git does not now the file yet

git add 	- track your files and changes in git
git add . or git add file or git add folder
git commit 	- save your files in git
git commit -m "title of commit -m "Description of the commit"
git push 	- upload git commits to a remote repository
git pull 	- download changes from remote repo to your local machine

ls -lha >> .git

.git
├── HEAD
├── branches
├── config
├── description
├── hooks
├── index
├── info
├── logs
├── objects
├── packed-refs
└── refs



git hub 
repository = project
	gwent/curriculum-app	
		with mockups
	

git remote -v

git remote add pb git@github.victor:victor-cleber/demo-repo.git
git remote remove origin


ssh-keygen -t rsa -b 4096 -C your@email.com
#start the ssh-agent in the background
    eval "$(ssh-agent -s)" # for Mac and Linux
#Adicionar a sua chave SSH pública ao GitHub
    cat ~/.ssh/id_rsa.pub # Linux

#Modify ~/.ssh/config
    vim  ~/.ssh/config     
Host github.victor
    AddKeysToAgent yes
    HostName github.com
    UseKeychain yes
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/victor/id_ed25519

ssh-add -K ~/.ssh/id_rsa #apple

ssh -T git@github.com
ssh -T git@github.victor
ssh -T git@github.bc



key.pub -upload to the web interface
key     -make it secure with you


cat key.pub

git push "location of gitrepository" "branch"
