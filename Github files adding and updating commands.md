git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/marzan3015/tictactoe.git

git push origin main
##error: src refspec main does not match any
##error: failed to push some refs to 'https://github.com/marzan3015/tictactoe.git'

git pull origin main --allow-unrelated-histories
##Automatic merge failed; fix conflicts and then commit the result.
git checkout --ours . 

(--ours means to keep the local files, --theirs is github repo files)

git add .
git commit -m "Merge remote repository with local project"
git push -u origin main

(then the files were uploaded)


##to delete some files-

Delete the files in the local repo first. then do the same-

git add .
git commit -m "deleted 5 files"
git push -u origin main

