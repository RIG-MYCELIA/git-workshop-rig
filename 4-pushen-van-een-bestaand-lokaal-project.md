# Een lokaal project op GitLab of GitHub zetten
Wanneer je lokaal al bezig bent geweest met een project en het wil delen via Git, dan kan je van je lokale
directory een Git repo maken d.m.v. het commando `git init`. Vervolgens kan je de bestanden die je wil delen toevoegen
aan je repo d.m.v. `git add` en `git commit`. De gemaakte Git repo kan je hierna pushen naar een remote platform, zoals GitLab of Github. 
Dit kan meestal direct d.m.v. een `git push` commando met de nodige variabelen, of indirect door een nieuw project aan te
maken op het platform naar keuze.

## Stap 1: Maak je lokale projectfolder een Git repo

Maak je lokale project een Git repo d.m.v. `git init` en voeg een README.md toe.   
Zie aanvullende instructies hier: 
[Lokaal een Git repo maken d.m.v. `init`](git_commando_instructions/lokale-git-init.md)  
  
## Stap 2: Voeg bestanden toe aan je Git repo
Voeg bestanden toe aan de repo d.m.v. `git add` en `git commit`   
Zie aanvullende instructies hier:
[Voeg bestanden toe aan je repo](git_commando_instructions/git-add-and-commit-files.md)


## Stap 3: Push je Git repo naar een remote

Je kan de repository op Github/Gitlab zetten door een nieuw project aan te maken op het platform en je repo
daar naartoe te pushen.  
Alternatief kan je in het geval van GitLab de repository direct sturen d.m.v. een `git push` commando met de nodige variabelen. 

### Push je lokale repo naar een nieuw project/repo op Gitlab of Github

Om een lokale repo te pushen naar een nieuw aangemaakt remote project zijn 2 stappen nodig: 

1. Maak eerst een remote repository aan op Gitlab of Github. Zorg ervoor dat je deze **zonder README** aanmaakt.   
[Nieuwe repository aanmaken op Github](git_commando_instructions/aanmaken-nieuwe-repo-github.md)   
[Nieuwe repository aanmaken op Gitlab](git_commando_instructions/aanmaken-nieuwe-repo-gitlab.md)   

2. Vervolgens stel je je nieuw aangemaakt project in als **remote** d.m.v. `git remote` en push je je repo d.m.v. `git push`.   
Zie :
[Lokale wijzigingen pushen naar een remote d.m.v. `push`](git_commando_instructions/git-push-naar-remote-repo.md)


### Push je lokale repo direct naar Gitlab via de command line

GitLab biedt de mogelijkheid een nieuwe repository via de command line aan te maken en te pushen. Github heeft op dit 
moment niet die functionaliteit.   

Op de **nieuwe repository/project** pagina van GitLab kan je onderaan klikken voor het commando dat voor jouw repository werkt.
Dit ziet er als volgt uit:
`git push --set-upstream git@gitlab.com:[USERNAME]/$(git rev-parse --show-toplevel | xargs basename).git $(git rev-parse --abbrev-ref HEAD)`

`$(git rev-parse --show-toplevel | xargs basename)`   
Dit pakt de naam van je huidige project op basis van de directory naam.  

`$(git rev-parse --abbrev-ref HEAD)`   
Dit pakt de huidige branch naam (vaak main)   

Simpeler gezegd kan je het commando dus als volgt vormgeven:   
`git push --set-upstream git@gitlab.com:[USERNAME]/[PROJECTNAAM].git [HOOFDBRANCH]`   
Voer dit commando uit in de hoofdfolder van je project (i.e. waar ook de **.git/** folder staat) en vanuit je hoofdbranch (vaak **main**)
 

[HOME](./README.md)


