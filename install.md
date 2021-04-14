# Installing *Git* on ta *Mac*



## Step 1 - Install *Homebrew* if you don't have it

**Copy & paste the following** into the terminal window and **hit `Return`**.
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew update && brew upgrade
```


## Step 2 - Install git
```
brew install git
brew link --force git
```


## Step 3 - Check git version and fix a path if need to
```
git --version
```

If you see a wrong version, maybe git pointed to old version

```
echo "alias git='/usr/local/bin/git'" >> ~/.zprofile && source ~/.zprofile
```

**Git is ready to use.**


## Configure your git name and email
Your name and email will be assosicated with *any* commits
```
git config --global user.name "Kirill T"
git config --global user.email "kirill@git.com"
```


