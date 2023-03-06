# SSH Key git Tutorial

**1º Step:** Open the git bash terminal and digit the comand line next:
```
ssh-keygen -t rsa -b 4096 -C "youremail"
```

**2º Step:** After executing the command and finishing the creation of the key, access the SSH folder:
```
cd ~/.ssh/
```

**3º Step:** Copy the key in id_rsa.pub, after executing the command below:
```
cat id_rsa.pub
```

**4º Step:** Login to your git hub then go to settings, click on SSH and GPG keys.

**5º Step:** Create a new SSH key and paste the copied key.

**6º Step** Now to finish, go back to the terminal and run the following command inside the .ssh/ folder:
```
ssh -T git@github.com -i id_rsa
```