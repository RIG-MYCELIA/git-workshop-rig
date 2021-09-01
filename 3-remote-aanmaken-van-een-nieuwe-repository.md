# Aanmaken nieuwe repository via Github/Gitlab

Je gaat nu een nieuwe, lege, repository aanmaken die je zowel lokaal als remote kan gebruiken. Dit gaat in twee stappen.   
Eerst maak je de remote repository aan op GitLab/GitHub. Vervolgens maak je een lokale kopie op je computer d.m.v. `git clone`.     
Wijzigingen voer je eerst door op je lokale kopie en `push` je dan naar de remote repository op GitLab/GitHub.

## Stap 1: Nieuwe remote repository aanmaken

Maak eerst een remote repository aan op Gitlab of Github. Geef deze een naam naar keuze en maak deze aan mét README bestand.   
[Nieuwe repository aanmaken op Github](git_commando_instructions/aanmaken-nieuwe-repo-github.md)    
[Nieuwe repository aanmaken op Gitlab](git_commando_instructions/aanmaken-nieuwe-repo-gitlab.md)

## Stap 2: Lokale kopie aanmaken

Maak lokaal een folder aan, bijvoorbeeld in je *Documenten* map, waar je je project in wil hebben en zorg vervolgens 
dat de projectbestanden lokaal beschikbaar zijn d.m.v. `git clone`.   
 
Zie: [Clone een repository naar je computer](git_commando_instructions/git-clone-repository.md)

## Stap 3: Wijzigingen maken in de repository

Je kunt nu op je eigen computer mappen aanmaken en bestanden toevoegen in de geclonede projectmap.   
Hiervoor kun je gewoon de Verkenner of andere programma's gebruiken.   
Open bijvoorbeeld het *README.md* bestand in een texteditor en type er wat tekst in.    

Je deze wijzigingen nu aan de lokale Git repository toevoegen d.m.v. `git add` en `git commit`.   

Zie: [Bestanden toevoegen aan de repo d.m.v. add en commit](git_commando_instructions/git-add-and-commit-files.md)

## Stap 4: Wijzigingen doorvoeren naar de remote repository

Als je zo ver bent, kun je alle commits van de lokale repository naar de remote repository op Github pushen d.m.v. `git push`.
   
Zie: [Lokale Git repo pushen](git_commando_instructions/git-push-naar-remote-repo.md)

Controleer of de remote repository op GitHub of GitLab is aangepast.


[HOME](./README.md)