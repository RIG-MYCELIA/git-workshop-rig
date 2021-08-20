## Workshop Git, GitHub en/of GitLab voor beginners
Deze repository bevat materiaal voor git workshops gegeven door het data team van het [Rijks ICT Gilde (RIG)](https://www.ubrijk.nl/service/rijks-ict-gilde). Het originele doel en auteurs zijn terug te vinden in de fork chain van deze repository of [hier](https://github.com/KennisnetwerkDataScience/git-en-github-workshop). 

## Inhoud
[Installeren van Git](1-installeren-van-git.md)  

[Aanmaken van een GitHub account](2-aanmaken-van-een-github-account.md)  


### Losse acties
###### Een repo maken of krijgen
- [Nieuwe repository aanmaken op GitHub](./aanmaken-nieuwe-repo-github.md)   
- [Nieuwe repository aanmaken op GitLab](./aanmaken-nieuwe-repo-gitlab.md) 
- [Lokaal een Git repo maken d.m.v. `init`](./lokale-git-init.md)  
- [Een remote repo lokaal krijgen d.m.v. `clone`](./git-clone-repository.md)
- [Een bestaande repo kopiëren d.m.v. `fork`](fork-repository.md)
    
###### Werken met de repo  
- [Een lokale repo koppelen aan een repo op Github/Gitlab d.m.v. `remote`](./git-add-remotes.md)
- [Wijzigingen/toevoegingen aan de Git repo d.m.v. `add` en `commit`](git-add-and-commit-files.md)   
- [Lokale wijzigingen pushen naar een remote d.m.v. `push`](git-push-naar-remote-repo.md)
- [Remote wijzigingen pullen naar de lokale repo d.m.v. `pull`](git-pull-from-remote.md)
- [Een merge conflict oplossen](./git-merge-conflict.md)

###### Samenwerken aan een repo
- [Een branch aanmaken d.m.v. `branch`](./git-branch.md)
- [Een branch mergen d.m.v. `merge`](./git-merge-branch.md)
- [Een pull request aanmaken op GitHub](#TODO)
- [Een pull request aanmaken op GitLab](#TODO)


### Stappenplannen
[Aanmaken van een nieuwe repository via Github/Gitlab](./remote-aanmaken-van-een-nieuwe-repository.md)  
&nbsp;&nbsp; Stap 1: GitHub repository aanmaken    
&nbsp;&nbsp; Stap 2: Lokale kopie aanmaken (clonen)     
&nbsp;&nbsp; Stap 3: Wijzigingen maken in de repository (add & commit)     
&nbsp;&nbsp; Stap 4: Wijzigingen doorvoeren naar de remote repository (push)     

[Een bestaand lokaal project in een Git repo en op Gitlab/Github zetten](./pushen-van-een-bestaand-lokaal-project.md)   
&nbsp;&nbsp; Stap 1: Maak je lokale projectfolder een Git repo    
&nbsp;&nbsp; Stap 2: Voeg bestanden toe aan je Git repo     
&nbsp;&nbsp; Stap 3: Push je Git repo naar een remote     

[Forken van een bestaande GitHub repository](4-bijdragen-aan-een-repository-van-een-ander.md)  
&nbsp;&nbsp;4.1 GitHub repository forken  
&nbsp;&nbsp;4.2 Lokale kopie aanmaken     
&nbsp;&nbsp;4.3 Wijzigingen doorvoeren in de repository  
&nbsp;&nbsp;4.4 Pull request aanmaken

[Conflicten oplossen en voorkomen](5-conflicten-oplossen-en-voorkomen.md)  
&nbsp;&nbsp;5.1 Upstream remote aanmaken  
&nbsp;&nbsp;5.2 Upstream en lokale repository samenvoegen    
&nbsp;&nbsp;5.3 Conflicten oplossen     
&nbsp;&nbsp;5.4 Conflicten voorkomen      

[Materiaal voor verdere studie](6-materiaal-voor-verdere-studie.md)  


#### Git op de commandline
Waar Git Bash gebruikt wordt, wordt het gebruik van Git op een unix command line bedoeld, dit is *Git Bash* of *MingW64* op Windows en de standaard 
*terminal* op Mac en Linux. Windows' *cmd* kan ook gebruikt worden (wanneer Git aan *Path* toegevoegd wordt), 
maar daarin verschillen sommige commando's van Unix commando's, zoals bijvoorbeeld `ls` vs. `dir`. 

#### Veelgebruikte command line commandos:  
`ls`: Unix commando; afkorting voor list: Laat bestanden en folders in de huidige folder zien  
`cd [/path/to/folder]`: Unix & Windows commando; Change directory: Ga naar een bepaalde folder op je computer of server. 
Wanneer er spaties in (een folder in) je *path* zitten, moet je aanhalingstekens om je *path* zetten `cd "/path/with spaces/in/it"` 
