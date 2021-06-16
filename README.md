GIT - system of version control .

GIT has repositories which can be local or remote and you can connect all of the repositories together.

gitbash is a software that is utilised to control our computer through the use of commands.

  tools needed for remote transfer of data(and more):
    -gitbash
      -install gitbash
      -install git
      -check version of git 
        git --version    
    -visual studio code
      -edit setting.json for integration of bash into VS code
       "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe",
    -github account(remote repository)
    (View and edit settings)
     git config --list
     git config --global user.name  "MikhailZyukin"
     git config --global core.editor "'C:\Users\Mikhail\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Visual Studio Code' -multiInst -nosession -noPlugin"

remote >>> local
{
step 1 :
    creation of a remote repository.
step 2 :
    create a local file by coping the remote repository.    
        git clone https://github.com/MikhailZyukin/git_instruction.git Git_instruction  
step 3 :
    Addition of changes to files recieved from the remote repository.
    make sure to open the repository folder in the integrated terminal.
     git status
     git remote -v
     git add *  (add all)
     git add README.md  (selected file)
     git commit -m 'First changes'
     git push
}


local >>> remote
{
step 4 :
    create directory (folder) for repository
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M master
    git remote add origin git@github.com:MikhailZyukin/misha.git
    git push -u origin master
    git remote add origin git@github.com:MikhailZyukin/misha.git
}
