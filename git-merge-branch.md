# Een branch mergen

Wanneer je klaar bent met het bouwen van functionaliteit in je ontwikkelbranch, dan wil je deze functionaliteit samenvoegen met de
rest van de repo zodat het eindproduct compleet is.   
Zie het 
als het samen maken van een verslag: Iedereen typt een hoofdstuk en uiteindelijk wil je die hoofdstukken samenvoegen.

In principe kan je lokaal elke branch in elke andere branch mergen (dit zal in meer of mindere mate [merge conflicts](./git-merge-conflict.md)
geven) en het resultaat pushen naar de remote repo.   
Het is echter **best practice** wanneer je samen aan een repo werkt om hier **pull requests** voor aan te maken. Wanneer
je alleen werkt, en branches dus alleen voor eigen overzicht gebruikt, dan is direct mergen geen probleem.

De branch waar je in ontwikkeld hebt en die je wil mergen is de **source branch**    
De branch waar je naartoe wil mergen is de **target branch**

1. Zorg dat je alles in je source branch [ge-add en ge-commit](./git-add-and-commit-files.md) hebt en dat deze up to 
   date is met eventuele remote versies van je source branch d.m.v. 
   `git pull` ([pullen](git-pull-from-remote.md)) en 
   `git push` ([pushen](git-push-naar-remote-repo.md)).
   

2. Ga naar de target branch waarin je je ontwikkel branch wil mergen, d.m.v. `git checkout [target_branch]`  

   e.g.: `git checkout main`    
  

3. Zorg dat de target branch up to date is door te [pullen](./git-pull-from-remote.md) met `git pull`


4. Merge de source branch in de target branch:
   
`git merge [source_branch]` 

e.g.: `git merge nieuwe_feature`


5. Los eventuele [merge conflicts](./git-merge-conflict.md) op


6. [Push](./git-push-naar-remote-repo.md) de target branch naar remote
