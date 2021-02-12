# SSH Keys

## WINDOWS

1) Download [PuTTY](https://www.putty.org)
2) Run PuTTYgen
3) Generate a new SSH Key. Hit *Generate* and move your mouse randomly.

**EXAMPLE**

![alt text](./assets/puttygen.PNG "puttygen")

4) Save the *Public Key* and the *Private Key*. Copy the top text to Github and Gitlab.

**EXAMPLE**

![alt text](./assets/save_ssh_keys.PNG "save ssh keys")

## MAC

1) Open *terminal*

2) run `ssh-keygen`

3) Hit enter until it finishes (don't add password etc)

4) run `pbcopy < ~/.ssh/id_rsa.pub`

5) You're ready to paste the key to Github and Gitlab 

### **GITHUB**
---

Settings -> SSH & GPG Keys

![alt text](./assets/github_new_ssh.PNG "save ssh keys")


![alt text](./assets/github_save_ssh_key.PNG "save ssh keys")

### **GITLAB**
---

Preferences -> SSH Keys

![alt text](./assets/gitlab_ssh.PNG "save ssh keys")


![alt text](./assets/github_save_ssh_key.PNG "save ssh keys")