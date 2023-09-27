# Command git
## Index your changes
```git add "name file"```

## De-indexing your changes
```git reset "name file"```

## View indexed files
```git diff --cached```

## Graph
```git log --graph --oneline --decorate```

## Back commit
```git rebase -i sha1``` or 
```git reset --soft HEAD~2```

## Debug git push

```
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

## Check your SSH keys
> Make sure you have an SSH key generated on your machine
```cat ~/.ssh/id_rsa.pub```

## Check the remote repository
```git remote -v```

## If the URL is incorrect, you can change it with
```git remote set-url origin YOUR_SSH_URL```

## Test your SSH connection with GitHub
``` ssh -T git@github.com```
> If everything is in order, you should see a message like "Hello [username]! You have successfully authenticated, but GitHub does not provide shell access."

## If you don't get the success message, check that the SSH key has been added to your GitHub account
> Connect to GitHub, go to your settings, then to the "SSH and GPG keys" section.

## Check if you have an SSH key
```ls -la ~/.ssh```
> You should see files named id_rsa (your private key) and id_rsa.pub (your public key). If you don't see them, you need to generate a new key pair. see documentation
