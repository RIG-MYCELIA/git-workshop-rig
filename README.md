## Workshop Git, GitHub en/of GitLab voor beginners
Deze repository bevat materiaal voor git workshops gegeven door het data team van het [Rijks ICT Gilde (RIG)](https://www.ubrijk.nl/service/rijks-ict-gilde). Het originele doel en auteurs zijn terug te vinden in de fork chain van deze repository of [hier](https://github.com/KennisnetwerkDataScience/git-en-github-workshop). 

## Inhoud
[Installeren van Git](1-installeren-van-git.md)  

[Aanmaken van een GitHub account](2-aanmaken-van-een-github-account.md)  


### Losse acties
- [Nieuwe repository aanmaken op GitHub](./aanmaken-nieuwe-repo-github.md)   
- [Nieuwe repository aanmaken op GitLab](./aanmaken-nieuwe-repo-gitlab.md)   
- [Wijzigingen/toevoegingen aan de Git repo d.m.v. `add` en `commit`](./bestanden-toevoegen-aan-de-repo.md)   
- [Lokale wijzigingen pushen naar een remote d.m.v. `push`](#TODO)
- [Remote wijzigingen pullen naar de lokale repo d.m.v. `pull` of `fetch`](#TODO)
- [Een remote repo lokaal krijgen d.m.v. `clone`](#TODO)
- [Een bestaande repo kopiëren d.m.v. `fork`](#TODO)
- [Een branch aanmaken d.m.v. `branch`](#TODO)
- [Een branch mergen d.m.v. `merge`](#TODO)
- [Een merge conflict oplossen](#TODO)
- [Een pull request aanmaken op GitHub](#TODO)
- [Een pull request aanmaken op GitLab](#TODO)



[Aanmaken van een nieuwe repository op GitHub](3-aanmaken-van-een-nieuwe-repository.md)  
&nbsp;&nbsp;3.1 GitHub repository aanmaken    
&nbsp;&nbsp;3.2 Lokale kopie aanmaken     
&nbsp;&nbsp;3.3 Wijzigingen doorvoeren in de repository     

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
