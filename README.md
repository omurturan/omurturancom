# Hello 😊👋

This repository holds the static content for my personal website omurturan.com.

This is built using [Hugo](https://gohugo.io/) and the theme is [Anatole](https://github.com/lxndrblz/anatole/).


### Development Setup

#### Instal hugo
```
brew install hugo
hugo version
```

#### Clone the repo
```
git clone git@github.com:omurturan/omurturancom.git
cd omurturancom
```

#### Initialize the submodules
The theme is added as a submodule. So, it needs to be seperately updated.
```
git submodule init
git submodule update --remote --merge
```

#### Run for local development
```
hugo server -D
```


## Add a new blog post
```
hugo new posts/git-multiple-user.md
```
