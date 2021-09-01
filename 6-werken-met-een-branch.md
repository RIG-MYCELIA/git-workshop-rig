# Werken met branches

In dit stappenplan ga je in een repository naar keuze een nieuwe branch aanmaken.    
Als je nog geen repository hebt, kan je die d.m.v. [dit stappenplan](./3-remote-aanmaken-van-een-nieuwe-repository.md)
aanmaken.

Branches worden gebruikt om losstaande stukken functionaliteit te kunnen ontwikkelen en testen. Door deze functionaliteit
in een aparte branch te zetten zit je je mede-ontwikkelaars niet in de weg met het pushen van veel losse commits. Zie het 
als het samen maken van een verslag: Iedereen typt een hoofdstuk, maar je wil niet elke regel die je typt direct delen met 
anderen. 

Een branch is een aftakking van een versie van de repo. Het is gebruikelijk nieuwe branches af te takken vanaf de hoofdbranch
(e.g. *main* of *master*). Het is ook mogelijk om een branch af te takken vanaf een sub-branch. Dit laatste is handig als je
wilt doorwerken op een stuk functionaliteit dat jij of een mede-ontwikkelaar al gebouwt heeft in een branch.

## Stap 1: Maak een nieuwe branch aan

Maak een nieuwe branch aan vanaf de hoofdbranch (e.g. *main* of *master*).

Zie ook: [Een branch aanmaken](git_commando_instructions/git-branch.md)

## Stap 2: Maak wijzigingen aan in je branch

Voeg bijvoorbeeld een plaatje toe dat je van google haalt of verander de tekst in het README.md bestand in de repo.    
Nadat je iets hebt gewijzigd of toegevoegd, voeg je deze wijzigingen toe aan de Git repo door `git add` en `git commit`
te gebruiken.

zie ook: [bestanden toevoegen aan de Git repo](git_commando_instructions/git-add-and-commit-files.md)

## Stap 3: Merge je branch in de hoofdbranch

Voeg de wijzigingen samen met de hoofdbranch van je repo (e.g. *main* of *master*).   
Dit kan je op 2 manieren doen: lokaal (via de command line of in je IDE) of remote d.m.v. een pull of merge request.

**Let op** Als je in een bestaand bestand een wijziging hebt gemaakt, kan je te maken krijgen met een 
[merge conflict](git_commando_instructions/git-merge-conflict.md)

### Optie 1: Lokale merge

Je kan kan de branch lokaal mergen in je hoofdbranch d.m.v. `git merge`

Zie: [Een branch mergen](git_commando_instructions/git-merge-branch.md)

Vervolgens kan je je hoofdbranch naar de remote repo pushen d.m.v. `git push`

Zie ook: [pushen naar remote](git_commando_instructions/git-push-naar-remote-repo.md)

### Optie 2: Pull/Merge request

Voor deze optie moet je je lokale branch eerst pushen naar remote d.m.v. `git push`.

Zie ook: [pushen naar remote](git_commando_instructions/git-push-naar-remote-repo.md)

Daarna kan je een [pull request (GitHub)](git_commando_instructions/github-pull-request.md) of [merge request (GitLab)](git_commando_instructions/gitlab-pull-request.md)
aanmaken.

[HOME](./README.md)