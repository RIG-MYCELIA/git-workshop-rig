# Conflicten oplossen en voorkomen

Wanneer er meerdere wijzigingen plaatsvinden op dezelfde plek in hetzelfde bestand, dan weet Git niet welke wijziging
behouden moet worden en kan Git deze wijzigingen niet meer automatisch samenvoegen. Dit noemen we een *merge conflict*. 
*Merge conflicten* kunnen ontstaan wanneer je twee verschillende branches merged, maar ook wanneer je wijzigingen [pullt](git_commando_instructions/git-pull-from-remote.md).

Wanneer je samenwerkt aan een repo ontkom je niet aan merge conflicten. In deze oefening gaan we een merge conflict veroorzaken
om een idee te krijgen wat een merge conflict eigenlijk is en hoe je dit kan oplossen.

Voor deze oefening heb je een repository nodig met een README.md bestand. Heb je nog geen repo? doorloop dan bijvoorbeeld de tutorial
[om een nieuwe repository aan te maken via Github/Gitlab](3-remote-aanmaken-van-een-nieuwe-repository.md).  

## Stap 1: Merge conflict veroorzaken

- Maak een nieuwe branch aan vanaf je hoofdbranch (e.g. *main*) (Voor meer info zie: [branch aanmaken](git_commando_instructions/git-branch.md))
```
git checkout main
git checkout -b conflict_branch
```    

- Pas in de *conflict_branch* het README.md bestand op je laptop aan. Voeg bijvoorbeeld een extra bullet toe met een tekstje.   
  
- Onthou de plek waarop je een wijziging hebt aangebracht, bijvoorbeeld de regelnummers of de al bestaande voorgaande tekst.    
  
- Voeg de wijziging in de branch toe aan je git repo d.m.v. [git add & commit](git_commando_instructions/git-add-and-commit-files.md)    

- Ga naar je hoofdbranch (e.g. *main*) door deze uit te checken:    
`git checkout main`    

- Pas in je hoofdbranch het README.md bestand op je laptop aan **op dezelfde regels (lijnnummers) als in de *conflict_branch***.
Voeg bijvoorbeeld tekst toe.   
      
- Voeg de wijziging in de hoofdbranch toe aan je git repo d.m.v. [git add & commit](git_commando_instructions/git-add-and-commit-files.md)    

Omdat je nu op dezelfde plek in een document wijzigingen hebt gemaakt, zal een merge van deze 2 branches een *merge conflict*
veroorzaken.


## Stap 2: Merge de conflicterende branches

Om de wijzigingen in je *conflict_branch* samen te voegen met je hoofdbranch (e.g. *main*) gebruik je `git merge`.
Zie [deze tutorial](git_commando_instructions/git-merge-branch.md) voor de nodige stappen en merge zo de *conflict_branch* in je hoofdbranch.

Tijdens de merge zul je de melding krijgen dat er een merge conflict is. Om het conflict op te lossen zul je 
in het README.md bestand moeten kiezen welke van de wijzigingen je wilt behouden door de conflictmarkeringen 
(`<<<<<<< HEAD ====== >>>>>>> andere_branch`) en 'verkeerde' tekst te verwijderen.
Zie [deze tutorial](git_commando_instructions/git-merge-conflict.md) voor een stappenplan om dit te doen.


## Stap 3: Conflicten voorkomen

Conflicten zijn niet altijd te voorkomen, maar door een aantal *best practices* aan te houden kan je de grootte van en de
hoeveelheid conflicten wel verminderen.
   
- Zorg er voor dat je lokale repository up-to-date is d.m.v. [git pull](git_commando_instructions/git-pull-from-remote.md), voordat je wijzingen doorvoert.
- Zorg ervoor dat de branch waar je een branch vanaf maakt up to date is, d.m.v. [git pull](git_commando_instructions/git-pull-from-remote.md)
- Probeer jira tickets/werkzaamheden zodanig te verdelen dat je niet tegelijk aan hetzelfde bestand hoeft te werken  
- Merge tijdens het developen regelmatig de hoofdbranch in je werk-branch om een grote hoeveelheid conflicten later te voorkomen


[HOME](README.md)
