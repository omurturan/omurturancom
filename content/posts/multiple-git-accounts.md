---
title: "USING MULTIPLE GIT ACCOUNTS"
date: 2021-04-13T20:30:36+02:00
draft: false
---

I'm using one computer for my work projects as well as my personal projects. In our company, we use Gitlab. However, I prefer to host my side projects on Github. Therefore, I needed to configure my local git setup so that it would know which account to use whenever I do `git push`.

I have different folders for personal and work related projects. Let's assume my directory structure looks like this:

```
~/Projects
└─── personal
│    └─── super-duper-project
│    └─── another-cool-project
│
└─── work
     └─── work-project-1
     └─── work-project-2
```
I want to use different Git accounts in `personal` and `work` folders. It can easily be done modifying your git configuration.

This is how my current `~/.gitconfig` looks like:
```bash {linenos=table}
[user]
    name = Ömür Turan
    email = my-personal-email@gmail.com
[pull]
    rebase = true
[includeIf "gitdir:~/Projects/work/"]
    path = .gitconfig-work
[core]
    excludesfile = /Users/omur/.gitignore_global
```

There is only one single trick here: `includeIf`. Here I'm basically saying that if the directory is the one I specified, then include the external git configuration named `.gitconfig-work`.

And this is the content of this `~/.gitconfig-work` file:

```bash  {linenos=table}
[user]
    name = Ömür Turan
    email = omur@my-work-email.com
```
No magic. Just dead simple configuration.

However, you probably have different SSH keys for your different Git accounts. Then, you also need to modify your SSH config. I'm not going into details of how to create an SSH key. For this example, I'll just assume you already have two different SSH keys. Let's again assume that this is your `~/.ssh` directory with two differen SSH keys (work and personal):

```
~/.ssh
│   config
│   known_hosts
│   work_id_ed25519
│   work_id_ed25519.pub
│   personal_id_ed25519
│   personal_id_ed25519.pub

```

In my use case, I wanted use `work_id_ed25519` key whenever I push to Gitlab. For everything else, I still want to use my regular `personal_id_ed25519` key. I achieved this result by modifying the `config` file. This is how my configuration looks like:

```bash  {linenos=table}
Host gitlab
    HostName gitlab.com
    User git
    IdentityFile ~/.ssh/work_id_ed25519

Host *
    IdentitiesOnly yes
    IdentityFile ~/.ssh/personal_id_ed25519
    IdentitiesOnly yes
    AddKeysToAgent yes
    UseKeychain yes
```

You can probably get more creative with your ssh config but this is what I needed.

I hope this was useful. If you have any comments, please do not hesitate to reach out to me. You can find my social media handles to the left of this page.

Cheers! 🕺
