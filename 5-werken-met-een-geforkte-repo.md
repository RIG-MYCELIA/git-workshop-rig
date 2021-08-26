# Werken met een geforkte repository

Je gaat nu een kopie maken van een bestaande repository op GitHub of GitLab en deze aanpassen.    

Het kopiëren van een bestaande repository heet **forken**. Door een repository te forken, heb je zelf een kopie waarop je
admin rechten hebt en die je volledig kan wijzigen zonder dat je afhankelijk bent van de originele eigenaar.    
Forken verschilt van clonen in dat er bij forken meerdere remote repositories ontstaan.

## Stap 1: GitHub/Gitlab repository forken

Ga naar de repository die je wil forken (bijvoorbeeld deze workshop repo) en klik de *fork* knop rechtsbovenin.      
Zie ook: [Repository forken](fork-repository.md)
   
   
## Stap 2: Lokale kopie aanmaken

De volgende stap is om een lokale kopie van jouw fork te maken op je computer d.m.v. `git clone [URL]`.   
**Let op** :
pak de URL van de repo onder je eigen account, niet die van de oorspronkelijke repo.

Zie ook: [Een repository clonen](./git-clone-repository.md)


## Stap 3: Wijzigingen doorvoeren in de repository

Maak een kopie van het bestand `deelnemers/deelnemer_JK.md`.    
Hernoem het bestand naar `deelnemer_[jouw initialen of naam].md` en pas de inhoud aan in een teksteditor, zodat het 
bestand bijvoorbeeld je favoriete quote bevat.     

Ga terug naar Git Bash en voeg het bestand en de wijzigingen toe aan de Git repo d.m.v. `git add` en `git commit`.    
Zie ook: [bestanden toevoegen aan de repo](./git-add-and-commit-files.md)
 
Verifieer op GitLab/GitHub dat je deelnemersbestand in je remote repository terecht is gekomen.    


## Stap 4: Pull request aanmaken

Je gaat nu een pull request (GitHub) of merge request (GitLab) aanmaken om de beheerders van de 'upstream' repository te 
verzoeken jouw aanvullingen door te voeren in hun repository.    
   
Maak hiervoor een [pull request (GitHub)](./github-pull-request.md) of 
[merge request (GitLab)](./gitlab-pull-request.md) aan met jouw fork als **source branch** en de upstream (originele)
repo als **target branch**
   

Wacht nu tot één van de repo beheerders je wijzigingen toevoegt aan de originele repository door je PR/MR goed te keuren.    


[HOME](./README.md)
