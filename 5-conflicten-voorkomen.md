Wacht tot een aantal van de pull requests van deelnemers van de worskhop is samengevoegd met de repository van Kennisnetwerk Data Science.    
Pas daarna het README.md bestand op je laptop aan. Voeg bijvoorbeeld een extra bullet toe met een tekstje.     
    
    
<img alt="README.md aanpassen" src="images/readme-aanpassen.png" width="300" />
   

Commit de wijzigingen en push ze naar je remote repository op GitHub:

`git add -A`   
`git commit -m "Een kleine tekstuele aanpassing"`     
`git push `     

Ga naar https://github.com/jouwGebruikersnaam/deelnemerslijst.     
Klik op de knop **New pull request**.     
je krijgt nu een scherm te zien met onderstaande melding:


Je krijgt deze melding, omdat je eigen repository achterloopt op de repository van Kennisnetwerk Data Science.     
Je hebt je wijzigingen doorgevoerd op een verouderde versie van de repository.     
Hoe kun je dit voorkomen?     

Ga niet verder met het aanmaken van een pull request. Ga terug naar https://github.com/jouwGebruikersnaam/deelnemerslijst.      

Zorg er voor dat je lokale repository twee aliassen ('remotes') kent:      
* `origin` die verwijst naar de deelnemerslijst repository onder je eigen account en      
* `upstream` die verwijst naar de deelnemerslijst repository van Kennisnetwerk Data Science.     

Check welke remotes al zijn aangemaakt door het volgende commando uit te voeren:

`git remote`
   
    
<img alt="git remote" src="images/git-remote.png" width="300" />
   

De remote `origin` is dus al aangemaakt.    
Check waarnaar `origin` verwijst met behulp van het volgende commando:      

`git remote-url origin`
   
    
<img alt="git remote get-url" src="images/git-remote-get-url.png" width="300" />
   

`origin` verwijst inderdaad naar de deelnemerslijst repository onder je eigen GitHub account.

Maak nu de remote `upstream` aan met het volgende commando:


`git remote add upstream https://github.com/kennisnetwerkdatascience/deelnemerslijst`     
   
    
<img alt="git remote add" src="images/git-remote-add.png" width="300" />
   

Verifieer dat de remote is aangemaakt en naar de juiste repository verwijst:

`git remote get-url upstream`
   
    
<img alt="git remote get-url upstream" src="images/git-remote-get-url-upstream.png" width="300" />
   
NOG VERDER AANVULLEN