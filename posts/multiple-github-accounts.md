If you would like to handle multiple github-accounts on your machine with dedicated ssh-keys you can write a ssh-config like the following:

```shell
Host github.com-private
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_private
  IdentitiesOnly yes
Host github.com-work
  HostName github.com
  User git
  IdentityFile ~/.ssh/id_rsa_work
  IdentitiesOnly yes
```

For cloning a repository you can make use of one of the keys then like:

`git clone git@github.com-private:my-github/my-repo.git`
