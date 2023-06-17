# git Cheat Sheet
### Github Configuration
1. Git auf dem local PC installieren
2. Nach Git installation auf Maschine git einrichten
```
    git config --global user.name <Name>
    git config --global user.email <github E-Mail adresse (ggf. private)>
```
3. ändert den Branche von master -> main
```
    git config --global init.defaultBranch main
```
4. git output farbig darstellen
```
    git config --global color.ui auto
```
5. Branche verwaltung zu mergin 
```
    git config --global pull.rebase false
```
6. github commit message über "git commit" statt "git commit -m" separates fenster
```
    git config --global core.editor "code --wait"
```

7. ssh key erstellprüfen 
```
    ls ~/.ssh/id_ed25519.pub
```
8. ssh key erstellen 
```
    ssh-keygen -t ed25519 -C <github e-mail>
```
9. ssh key anzeigen
```
    cat ~/.ssh/id_ed25519.pub
```  
10. dann ssh Key in Github Einstellungen kopieren 
auf [github](https://github.com/)
11. Verbindung auf Maschine verifizieren
```
    $ ssh -T git@github.com
```
Fingerprint verifizieren [mit der offizielle Github Seite](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection) 

### Git und Githup workflow :
* Bei der URL darauf achten, ob SSH,HTTPS,CLI ausgewählt ist
```
    git clone git@github.com:USER-NAME/REPOSITORY-NAME.git
    git push or git push origin main (Both accomplish the same goal in this context)
```
* Commands für den workflow:
    - `git add .`
    - `git commit -m "Änderungsnachricht"`
    - `git commit`
* Commands für status check und hisorie log 
    - `git status`
    - `git log`
    - `git remote -v`
* The basic Git syntax is program | action | destination.