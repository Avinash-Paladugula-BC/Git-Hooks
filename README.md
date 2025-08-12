After creating a repository create a file commit-log.md using the touch command

we can use vi commit-log.md command to  write some content to the file.
Now to write the post-commit hook navigate to the file : .git/hooks/post-commit
write the script that needs to be executed once the commit is done
After writing the script and saving it, to make it an executable file use the command: chmod +x post-commit  -->> now the file is executable

To test the hook some commits needs to be made. So I've created files and adding some content to it and commiting after adding the content to each file.

After every commit the commit-log.md file is being updated with the date, time and the commit message

The post-commit hook will be helpful when we want to automate the tasks just like triggers. When ever a new commit is made we can implement few steps using the post-hook.
