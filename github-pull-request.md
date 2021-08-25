# Een Pull Request openen op GitHub

Een pull request (github) of merge request (gitlab) wordt gebruikt om de functionaliteit van de ene branch op een gecontroleerde manier 
samen te voegen met een andere branch. Het gecontroleerde zit in het volgende: Bij het maken van de pull request wordt
een overzicht gegeven van de verschillen tussen de 2 branches. Zo kan je goed controleren of je inderdaad alleen wijzigingen
hebt aangebracht op de plekken waar je wijzigingen wou maken. Het komt soms voor dat je per ongeluk iets verwijderd hebt,
of juist iets hebt toegevoegd wat niet in de repo hoort - zoals data of een hardcoded path.   
Naast dat je zelf kan controleren of je de juiste aanpassingen hebt gemaakt, kan je ook aan een mede-ontwikkelaar vragen
of die wil kijken naar jouw code. Die persoon kan dan controleren op fouten, tips geven over andere implementaties of
vragen stellen over je aanpak. Hiermee zorg je ervoor dat het werk dat uiteindelijk in de hoofdversie van je repo komt
goed werkt, 'schoon' is en daardoor overdraagbaar is naar, en reproduceerbaar voor, andere personen. Daarnaast zorgt een pull request ook voor 
onderlinge kennisuitwisseling over lopende projecten en gebruikte technieken.

De branch waar je in ontwikkeld hebt en die je wil mergen is de **source branch**   
De branch waar je naartoe wil mergen is de **target branch**

## Een PR aanmaken

- Ga in GitHub in je repo naar het tabblad *Pull requests* en klik op de groene knop: *New pull request*

<img alt="Nieuwe PR" src="images/github-PR-new-pull-request.png" width="800" />

- Kies je target en source branch

  <img alt="Kies branches voor PR" src="images/github-PR-compare-branch.png" width="800" />

- Geef een onderwerp en beschrijving op voor je pull request.    
- Klik op de knop **Create pull request**.    

<img alt="Create pull request" src="images/create-pull-request.png" width="400" />
   
### PR aanmaken tussen geforkte repo's
Voor [geforkte repos](./fork-repository.md): Wanneer je een PR wil aanmaken voor een merge tussen jouw repo en de 
upstream repo, dan kies je ook de base repository. Wanneer een repo geforkt is weet GitHub dat 
en toont de optie om de juiste repository te kiezen:    

<img alt="Comparing changes" src="images/comparing-changes.png" width="600" />


## Een PR (laten) reviewen

- Op de hoofdpagina van je pull request, onder het tabblad *Conversation*, kan je aan de rechterkant één of meerdere 
  reviewers kiezen door op *Reviewers* te klikken.
Hoeveel reviewers je kiest hangt af van de afspraken die je in je team maakt en de instellingen van je repository.
  
<img alt="Add reviewers" src="images/github-PR-add-reviewer.png" width="800" />

Onder het tabblad *Files changed* vind je het eindresultaat van alle commits in de branch. Oftewel, de veranderingen
waarvan gevraagd wordt deze te mergen in de **target branch**. Op het tabblad *commits* kan je individuele commits inzien.

- Wanneer je een vraag, tip, suggestie of opmerking hebt over een wijziging, dan kan je over de regel heen hoveren en
  op het **+** teken aan het begin van de regel klikken om een comment toe te voegen. Je kan ervoor kiezen een 
  *single comment* toe te voegen of een *review* te starten. 
  Wanneer je meerdere bestanden moet reviewen en je in één keer al je commentaar wil overbrengen, 
  dan kies je voor een *review*, wanneer er weinig wijzigingen zijn of als je niet alle
  wijzigingen langs zult gaan kan je ook een enkel comment achterlaten. Hierover kan je afspraken maken in je team of 
  gewoon je persoonlijke voorkeur aanhouden.

  <img alt="Add comment" src="images/github-PR-comment.png" width="800" />

- Om de persoon die de PR geopend heeft te laten weten dat je klaar bent met je review kan je rechtsbovening op *review changes*
  of *finish review* (in het geval van een gestart review proces) klikken. Dit geeft een aantal opties, zoals op de 
  screenshot hieronder te zien is, *comment*, *approve*, *request changes*.   
  De meeste teams kiezen er voor om alleen *approve* en *request changes* te gebruiken:   
  Met *Approve* geef je aan dat je erop vertrouwt dat PR-opener jouw commentaar goed verwerkt en dat de branch gemerged 
  mag worden zodra jouw feedback verwerkt is .   
  Met *Request changes* geef je aan dat je na het verwerken van jouw feedback nog een blik wil werpen op de wijzigingen
  alvorens je je approval geeft.

  <img alt="Finish review" src="images/github-PR-finalize-review.png" width="600" />



## Een PR mergen

- Voor je een PR merged is het best practice om, naast het verwerken van feedback, ook te reageren op alle comments.
  Hiermee maak je voor de reviewer duidelijk dat je alle comments gezien en overwogen hebt. Reacties kunnen variëren
  van een uitgebreide uitleg over de keuzes die je hebt gemaakt tot een duimpje omhoog of like als leesbevestiging.
  Ook hierover kunnen afspraken gemaakt worden in het team.

- Je kan rechts in het *Conversations* scherm zien wanneer de reviewers klaar zijn met de review en de wijzigingen 
  *approved* hebben (groen vinkje). 
  <img alt="Approved" src="images/github-PR-approved.png" width="300" />

- Onderin het *Conversations* scherm kan je je PR mergen. Er wordt aangegeven of er [merge conflicts](./git-merge-conflict.md)
  zijn, zowel dan moet je die eerst oplossen voor de branch gemerged kan worden.    
  Wanneer je niet zo bekend bent met Git kan je bij het mergen van de pull request voor de simpelste optie kiezen in de dropdown:
  *Create merge commit*: Klik *merge pull request* -> klik *confirm merge*.    
  Je kan altijd in een later stadium nog branches verwijderen of commits rebasen. Ook daarover kan je in je team afspraken maken.
  
  <img alt="Approved" src="images/github-PR-merge.png" width="600" />


Je branch is nu gemerged in de target branch! 
Vergeet de target branch niet lokaal te [pullen](./git-pull-from-remote.md).
