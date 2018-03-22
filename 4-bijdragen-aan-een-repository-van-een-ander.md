Je gaat nu een kopie maken van een bestaande repository op GitHub en deze aanpassen.    
Het gaat om een eenvoudig project: een overzicht van deelnemers aan deze workshop.   

## Stap 1: GitHub repository forken
   
Ga naar https://github.com/KennisnetwerkDataScience/deelnemerslijst.    
   
Zorg er voor dat je bent ingelogd op GitHub.    
   
Klik op **Fork**. Deze knop vind je in de rechter bovenhoek van je scherm.    
    
    
<img alt="Fork repository" src="images/git-fork.png" width="300" />
   
   
Het kan even duren, maar uiteindelijk wordt er een kopie van de repository aangemaakt onder jouw eigen gebruikersnaam.    
   
   
<img alt="Forked repository" src="images/git-fork-repo.png" width="600" border="1" />
   
   
## Stap 2: Lokale kopie aanmaken

De volgende stap is om een lokale kopie te maken op je computer.    

Open Git Bash.  
Navigeer naar de map waar je de repository wilt opslaan.      
   
`$ cd "D:/Jouw map naam"`    

Kopieer de remote repository naar je lokale computer met het volgende commando:   

`$ git clone https://github.com/jouwGebruikersnaam/deelnemerslijst.git`   
   
   
<img alt="Clone deelnemerslijst" src="images/git-fork-clone.png" width="400" />
   
    
Navigeer naar de lokale repository.   

`$ cd "D:/Jouw map naam/deelnemerslijst"`


## Stap 3: Wijzigingen doorvoeren in de repository

Maak een kopie van het bestand `deelnemers/willy-tadema.md`.    
Hernoem het bestand en pas de inhoud aan in een teksteditor, zodat het bestand een aantal wetenswaardigheden over jou bevat.     
Je kunt eventeel een afbeelding toevoegen. Plaats dit bestand in de map `images` en zorg er voor dat je de verwijzing in het markdown bestand aanpast.    
Open het bestand README.md. Voeg een extra bullet toe met jouw naam en een verwijzing naar het bestand dat je zojuist hebt aangemaakt.   

Ga terug naar Git Bash.    
   
Zet de wijzigingen klaar voor de commit:    
    
`$ git add -A`
   
Voer vervolgens de commit uit:    

`$ git commit -m "Info over <jouw naam> toegevoegd"`    
   
Push je lokale commit naar je remote repository op GitHub:    
   
`$ git push`
   
   
<img alt="git add, commit and push" src="images/git-fork-add-commit-push.png" width="400" />
   
 
Verifieer dat de deelnemerslijst in je remote repository op GitHub nu gegevens over jou bevat en dat de verwijzingen goed werken.    


## Stap 4: Pull request aanmaken

Je gaat nu een pull request aanmaken om de beheerders van de 'upstream' repository van Kennisnetwerk Data Science te verzoeken jouw aanvullingen door te voeren in hun repository.    
   
Ga naar https://github.com/jouwGebruikersnaam/deelnemerslijst.    
   
Zorg er voor dat je bent ingelogd op GitHub.    

Klik op **New pull request**.
    
    
<img alt="New pull request" src="images/new-pull-request.png" width="300" />
   

Je krijgt nu een scherm te zien met daarin de wijzigingen in jouw repository ten opzichte van die van Kennisnetwerk Data Science.     
Merk op dat de beschrijving die je hebt meegegeven in je `git commit` commando zichtbaar is in dit scherm.   
Klik op de knop **Create pull request**.    
     
    
<img alt="Comparing changes" src="images/comparing-changes.png" width="400" />
   
    
Geef een onderwerp en beschrijving op voor je pull request.    
Klik op de knop **Create pull request**.    

    
<img alt="Create pull request" src="images/create-pull-request.png" width="400" />
   

Wacht nu tot één van de GitHub beheerders van Kennisnetwerk Data Science je wijzigingen toevoegt aan de originele repository met een **Merge pull request**.    


[Volgende](5-conflicten-oplossen-en-voorkomen.md)
