# DevOps Demo Repo.

## Topic 1 - Git Version Cantrol

## Git Version Cantrol

### Register yourself to github.com & done the verfication. 

### Create a new repo with the name : DevOps-301-Mindtree-2020Oct17

### Lets clone our newly create Repo. 
```
git clone https://github.com/amitvashisttech/devops301-mindtree-17Oct2020.git
```

### Go inside the Repo & Create your first commit
```
cd devops301-mindtree-17Oct2020/
echo "Hello World" > Hello.txt
git status
git add Hello.txt
git status
git commit -m "New file - Hello.txt"
git log
```

### Git Global Configuration 
```
git config --global user.name "Amit Vashist"
git config --global user.email "amitvashist7@outlook.com"
git config --list
git config --global core.editor vi
```

### Push the code to Origin
```
git push
```


### Git Branch 



### Git Credentials Helper
```
git config credential.helper store
git push 
```
