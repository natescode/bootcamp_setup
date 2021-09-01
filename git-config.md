# GIT config tips and tricks


## Aliases

I have several aliases for my git commands. 

Here's what my `.gitconfig` in my home directory looks like

    [user]
        email = nate@natescode.com
        name = Nate
        github = https://www.github.com/USERNAME_HERE
        signingkey = YOUR_KEY_HERE
    [core]
        editor = \"C:\\Users\\nate\\AppData\\Local\\Programs\\Microsoft VS Code\\Code.exe\" --wait
        longpaths = true
    [alias]
        s = status
        co = checkout
        cob = checkout -b
        del = branch -D    
        br = branch --format='%(HEAD) %(color:yellow)%(refname:short)%(color:reset) - %(contents:subject) %(color:green)(%(committerdate:relative)) [%(authorname)]' --sort=-committerdate
        save = !git add -A && git commit -m 'chore: savepoint'
        undo = reset HEAD~1 --mixed
        res = !git reset --hard
        done = !git push origin HEAD
        lg = !git log --pretty=format:\"%C(magenta)%h%Creset -%C(red)%d%Creset %s %C(dim green)(%cr) [%an]\" --abbrev-commit -30
        last = log -1 HEAD
        cm = commit -m 
        ci = commit
        st = stash
        pop = stash pop
        apply = stash apply
        get = config --global 
        github = !git remote add origin && !git --set-upstream-branch    
