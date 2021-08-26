# Lokaal een Git repo maken d.m.v. init

Hiermee kan je van je lokale directory/folder een Git repo maken d.m.v. het commando `init`.  
Als je alleen wil oefenen, kan je hiervoor in je verkenner een folder aanmaken als zijnde een dummy project en daarin
een aantal bestanden zetten.   
Dit kan ook in je Git Bash:   
```
mkdir ~/dummy_project
cd ~/dummy_project
touch some_script.py
```

De tilde (`~`) is een Unix 'afkorting' voor je home directory, e.g. `C:/Users/[jouw naam]` op Windows.

### Controleer of je projectfolder al een Git repo is  
Een Git repo heeft een `.git/` folder. Dit kan je controleren in een verkenner. 
Let erop dat je hiervoor *verborgen bestanden* zichtbaar moet maken.   

Alternatief kan je in **Git CL** naar je project path gaan d.m.v.   
`cd /path/to/project/`  
en één van de volgende acties uitvoeren:  
- `git status`   
Dit geeft de volgende error wanneer er geen Git repo gevonden is:   
  `fatal: not a git repository (or any of the parent directories): .git`
  en de normale status output wanneer er wel een Git repo gevonden is.
- `ls -a`    
Dit laat alle bestanden en directories in je projectfolder zien. Wanneer de huidige folder een Git repo is, staat 
  `.git/ ` in de lijst.
  

### Maak van je projectfolder een Git repo
Ga in **Git CL** naar je project path gaan d.m.v.   
`cd /path/to/project/`      
en voer het volgende commando uit:  
`git init`  
Dit geeft als output:  
`Initialized empty Git repository in /path/to/project/.git/`  

Je projectfolder is nu een Git repo!

### Voeg een README bestand toe aan je project
Het is best practice om een README.md toe te voegen aan je projectfolder. In de README.md kan je informatie kwijt over de repository. Bijvoorbeeld wat het doel is van je repo en hoe je bepaalde 
code kan draaien. 
Nadat je je repo gepusht hebt, wordt de inhoud van dit bestand getoond aan bezoekers van de webpagina van je GitHub/GitLab repository.   
   

De extensie `*.md` staat voor een markdown bestand. Markdown is net als HTML een taal voor het opmaken van webpagina's, 
maar dan een stuk eenvoudiger.   
Klik hier voor een [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).   

Je kan je README bestand aanmaken m.b.v. een texteditor:
- Open een texteditor (e.g. notepad++, notepad, vim, nano...)
- Type wat tekst over je project (dit kan altijd later nog aangevuld of aangepast worden)
- Bij het opslaan plaats je het bestand in de hoofdfolder van je project en geef je het de naam `README.md` 
  (incl. de `*.md` extensie)
  

[HOME](./README.md)