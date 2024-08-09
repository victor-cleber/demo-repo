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


#create a new folder out of this repo
create a file
git add da erro


create a new repo on github

add the remote on local folder 

git remote add origin git@github.com:victor-cleber/demo2.git

git remote -v vai mostrar qq git repo conectado neste repositorio local

Para configurar o upstream automatico entao nao preciso digitar origin master toda x q fizer um push
git push -u origin main
git push --set-upstream origin master


## GH workflow
Write a code 
commit changes

need a revewi
Pull request


## local git workflow
write code
stage changes   >> git add 
commit changes  >> git commit
push changes    >> git push
code review >> make a pull request



## git branching

bug branch                         ========= Fix =======
                                  |                     | 
master branch                     |                     |  
        commit#1=============commit#2=================commit#3=============commit#4===Merge===
                                |                                                       |
                feature branch  |commit#1==================commit#2=====================



git branch
git checkout -b feature-readme-instructions
git branch
git checkout main #switch betwwen branchs
branch
git checkout  feature-readme-instructions

a nova branch estava atrasada em relacao a main 
git rebase main ficou igual

alterar texto na nova branch
git add
git commit
git checkout main

a main esta atrasada em relacao a nova branch
antes de dar o merge vamos ver a diferenca no codigo

git diff nome_da_outra_branch
git diff feature-readme-instructions

git checkout 
git status
git push da erro
     git push --set-upstream origin feature-readme-instructions
     git push -u origin feature-readme-instructions

    PR is a request to have your code pulled at another branch
        delete your branch
        
