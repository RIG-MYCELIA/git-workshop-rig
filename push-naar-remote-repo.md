# Push lokale repo en/of lokale wijzigingen naar een remote

## Stel je remote repository in

#### Controleer of je repository al een remote heeft    

Ga naar je projectdirectory:   
`cd /path/to/project/`   

Roep de ingestelde remotes in:   
`git remote -v`   
Als dit niks teruggeeft, dan heb je nog geen remote repository ingesteld. Anders zie je iets vergelijkbaar met dit:    
```
origin  git@github.com:[USERNAME]/[PROJECTNAAM].git (fetch)
origin  git@github.com:[USERNAME]/[PROJECTNAAM].git (push)
```  

Als de URLs inderdaad overeenkomen met het bedoelde project en de bedoelde bestemming (Gitlab/Github), dan kan je door
naar **Push je repository**

#### Voeg een remote toe aan je lokale repository

Op de hoofdpagina van je project (e.g. `www.github.com/[USERNAME]/[PROJECTNAME]`) op Github of Gitlab vind je een 
dropdown menu knop:   
**Clone** (Gitlab)   
<img alt="Git areas" src="images/clone-knop-gitlab.png" width="600" />  
of **Code** (Github)    
<img alt="Git areas" src="images/clone-knop-github.png" width="600" />  

In het clone dropdown menu kan je (o.a.) kiezen uit clonen met SSH of met HTTPS. Wanneer je nog geen ssh hebt ingesteld 
gebruikt je de HTTPS URL.   
Kopieer de URL en ga naar je Git Bash:   
`git remote add origin [CLONE URL]`   

Controleer of je remote is toegevoegd voor zowel `push` als `fetch`:   
`git remote -v`   
Je ziet iets vergelijkbaar met dit:    
```
origin  git@github.com:[USERNAME]/[PROJECTNAAM].git (fetch)
origin  git@github.com:[USERNAME]/[PROJECTNAAM].git (push)
```  

## Push je repository

Nadat je bestanden of wijzigingen hebt toegevoegd aan je lokale repository 
(Zie: [add en commit](./bestanden-toevoegen-aan-de-repo.md)) en een remote hebt ingesteld, 
kan je je repository pushen:   
`git push origin main`   
oftewel:   
`git push [REMOTENAAM] [BRANCHNAAM]`

In het geval van een HTTPS remote URL, kan het zijn dat je je Gitlab/Github username en wachtwoord moet invoeren.   
In het geval van een SSH remote URL, kan het zijn dat je je passphrase van je ssh sleutel moet invoeren.

<img alt="Push" src="images/new-repo-push.png" width="400" />   

Voer het `git status` commando uit.   
Merk op dat de lokale en remote repository weer met elkaar synchroon lopen.
   

<img alt="Status after push" src="images/new-repo-status-after-push.png" width="400" />    
   

Controleer of de remote repository op Github is aangepast.

Wanneer je default remote/upstream goed ingesteld zijn, kan je dit versimpelen naar enkel `git push`.
Hierbij kom je soms wel de volgende melding tegen:   
```
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main
```

Git geeft hierbij direct een oplossing voor je probleem: `git push --set-upstream origin main`

Voor meer info, voer `git push --help` uit.


