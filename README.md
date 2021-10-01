## Workshop Git, GitHub en/of GitLab voor beginners
Deze repository bevat materiaal voor git workshops gegeven door het data team van het [Rijks ICT Gilde (RIG)](https://www.ubrijk.nl/service/rijks-ict-gilde). Het originele doel en auteurs zijn terug te vinden in de fork chain van deze repository of [hier](https://github.com/KennisnetwerkDataScience/git-en-github-workshop). 

Gebruik de *Losse acties* sectie om gericht hulp te krijgen bij het gebruik van een Git commando.    
Gebruik de *stappenplannen* om beter bekend te raken met hoe Git gebruikt kan worden in dagelijkse werkzaamheden.    

#### Git op de commandline
Waar in de tutorials Git Bash genoemd wordt, wordt het gebruik van Git op een unix command line bedoeld, dit is *Git Bash* of *MingW64* op Windows en de standaard 
*terminal* op Mac en Linux. Windows' *cmd* (*opdrachtprompt*) kan ook gebruikt worden (wanneer Git aan *PATH* toegevoegd wordt), 
maar daarin verschillen sommige commando's van Unix commando's, zoals bijvoorbeeld `ls` vs. `dir`. 

#### Veelgebruikte command line commandos:  
`pwd`: print working directory: Laat je huidige folder/path zien (In Windows *cmd* is dit `cd`)    

`ls`: Unix commando; afkorting voor list: Laat bestanden en folders in de huidige folder/path zien  

`cd [/path/to/folder]`: Unix & Windows commando; Change directory: Ga naar een bepaalde folder op je computer of server. 
Gebruik de *tab* toets om paden automatisch aan te vullen.
Wanneer er spaties in (een folder in) je *path* zitten, moet je aanhalingstekens om je *path* zetten: `cd "/path/with spaces/in/it"`    
Let erop dat in de Windows *cmd* de paden back slashes `\` ipv forward slashes `/` hebben 

## Inhoud
[Installeren van Git](1-installeren-van-git.md)  

[Aanmaken van een GitHub account](2-aanmaken-van-een-github-account.md)  


### Losse acties
#### Een repo maken of krijgen
- [Nieuwe repository aanmaken op GitHub](git_commando_instructions/aanmaken-nieuwe-repo-github.md)   
- [Nieuwe repository aanmaken op GitLab](git_commando_instructions/aanmaken-nieuwe-repo-gitlab.md) 
- [Lokaal een Git repo maken d.m.v. `init`](git_commando_instructions/lokale-git-init.md)  
- [Een remote repo lokaal krijgen d.m.v. `clone`](git_commando_instructions/git-clone-repository.md)
- [Een bestaande repo kopiëren d.m.v. `fork`](git_commando_instructions/fork-repository.md)
    
#### Werken met de repo  
- [Een lokale repo koppelen aan een repo op Github/Gitlab d.m.v. `remote`](git_commando_instructions/git-add-remotes.md)
- [Wijzigingen/toevoegingen aan de Git repo d.m.v. `add` en `commit`](git_commando_instructions/git-add-and-commit-files.md)   
- [Lokale wijzigingen pushen naar een remote d.m.v. `push`](git_commando_instructions/git-push-naar-remote-repo.md)
- [Remote wijzigingen pullen naar de lokale repo d.m.v. `pull`](git_commando_instructions/git-pull-from-remote.md)
- [Een merge conflict oplossen](git_commando_instructions/git-merge-conflict.md)
- [Git tekst editor gebruiken of wijzigen](./git-editor.md)

#### Samenwerken aan een repo
- [Een branch aanmaken d.m.v. `branch`](git_commando_instructions/git-branch.md)
- [Een branch mergen d.m.v. `merge`](git_commando_instructions/git-merge-branch.md)
- [Een pull request aanmaken op GitHub](git_commando_instructions/github-pull-request.md)
- [Een pull request aanmaken op GitLab](git_commando_instructions/gitlab-pull-request.md)


### Stappenplannen
[Aanmaken, lokaal krijgen en gebruiken van een nieuwe repository via Github/Gitlab](3-remote-aanmaken-van-een-nieuwe-repository.md)  
&nbsp;&nbsp; Stap 1: GitHub repository aanmaken    
&nbsp;&nbsp; Stap 2: Lokale kopie aanmaken (clonen)     
&nbsp;&nbsp; Stap 3: Wijzigingen maken in de repository (add & commit)     
&nbsp;&nbsp; Stap 4: Wijzigingen doorvoeren naar de remote repository (push)     

[Een bestaand lokaal project in een Git repo en op Gitlab/Github zetten](4-pushen-van-een-bestaand-lokaal-project.md)   
&nbsp;&nbsp; Stap 1: Maak je lokale projectfolder een Git repo        
&nbsp;&nbsp; Stap 2: Voeg bestanden toe aan je Git repo     
&nbsp;&nbsp; Stap 3: Push je Git repo naar een remote     

[Werken met een geforkte repository](5-werken-met-een-geforkte-repo.md)  
&nbsp;&nbsp;Stap 1: GitHub/Gitlab repository forken     
&nbsp;&nbsp;Stap 2: Lokale kopie aanmaken    
&nbsp;&nbsp;Stap 3: Wijzigingen doorvoeren in de repository  
&nbsp;&nbsp;Stap 4: Pull request aanmaken    

[Werken met branches](./6-werken-met-een-branch.md)     
&nbsp;&nbsp;Stap 1: Maak een nieuwe branch aan     
&nbsp;&nbsp;Stap 2: Maak wijzigingen aan in je branch     
&nbsp;&nbsp;Stap 3: Merge je branch in de hoofdbranch:     
&nbsp;&nbsp;&nbsp;&nbsp;Optie 1: Lokale merge    
&nbsp;&nbsp;&nbsp;&nbsp;Optie 2: Pull/Merge request    


[Merge conflicten veroorzaken, oplossen en voorkomen](7-conflicten-oplossen-en-voorkomen.md)  
&nbsp;&nbsp;Stap 1: Merge conflict veroorzaken  
&nbsp;&nbsp;Stap 2: Merge de conflicterende branches    
&nbsp;&nbsp;Stap 3: Conflicten voorkomen    

[Materiaal voor verdere studie](8-materiaal-voor-verdere-studie.md)  



