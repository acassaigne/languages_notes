# git / github

## tow ssh keys to work to differents account repositories

I got one professional git account and a personal github account.

My default ssh key are for professional account, so I created a specific ssh
configuration for personal account.

I started to create a `.config` file in `.ssh` directory.

The content is:

```
Host perso-gh
    # The host that has the remote Git repository
    Hostname github.com
    # Username for remote SSH user (For GitHub, everyone uses the name `git`)
    User firstname.lastname@my_email.org
    # Path to your private SSH key
    IdentityFile ~/.ssh/perso_id_rsa
```

Now I can clone personal github repository, like this:

```bash
git clone git@perso-gh:acassaigne/languages_notes.git
```

Inpisred by https://www.devdungeon.com/content/how-specify-ssh-key-git-repository
