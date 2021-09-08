Na het maken van een GitHub-account, kun je er voor kiezen een ssh-key toe te voegen aan je account. Dit heeft als
voornaamste voordeel dat je niet telkens je gebruikersnaam en wachtwoord op hoeft te geven bij acties die je uitvoert.
Het toevoegen van een ssh-key bestaat uit de volgende stappen:

- Een ssh-key genereren
- De gegenereerde ssh-key aan je GitHub-account toevoegen
- De ssh-verbinding testen

## Een ssh-key genereren

Om een ssh-key te genereren, moeten we een aantal commando's in de terminal (Linux/Mac) of de Git Bash terminal (
Windows) uitvoeren. Open deze nu.

Plak de volgende tekst in de terminal, waarbij je het email-adres gebruikt waarmee je je GitHub-account hebt aangemaakt:

```
$ ssh-keygen -t ed25519 -C "email@adres.com"
```

In enkele gevallen wordt het Ed25519-algoritme niet ondersteund, gebruik dan dit:

```
$ ssh-keygen -t rsa -b 4096 -C "email@adres.com"
```

Dit vraagt vervolgens om een locatie om de ssh-key op te slaan. Het makkelijkst is om hier op enter te drukken en de
standaardlocatie, weergegeven tussen de haakjes, zal gebruikt worden. Mocht je een andere locatie willen gebruiken, geef
deze dan hier op.

Kies ten slotte een wachtwoord voor je ssh-key.

Na het maken van de ssh-key, voegen we deze toe aan de ssh-agent, zodat we er ook gebruik van kunnen maken. We starten
eerst de agent op, als het goed is, geeft dit als output 'Agent pid' met een getal erachter.

```
$ eval "$(ssh-agent -s)"
```

Als dat gelukt is, voegen we de ssh-key toe aan de agent. Dit gaat uit van de standaardlocatie voor ssh-keys, heb je
deze veranderd, pas dit hier dan ook aan.

```
$ ssh-add ~/.ssh/id_ed25519
```

## De gegenereerde ssh-key aan je GitHub-account toevoegen

Om de ssh-key toe te voegen aan een GitHub-account, moeten we een aantal acties op GitHub uitvoeren. Start dus om te
beginnen de browser op, ga naar GitHub en log in.

- Klik op je profielfoto rechtsboven op de pagina en klik op "Settings"
- Klik in het menu links op "SSH and GPG keys"
- Klik in de SSH sectie op de knop "New SSH key"

Nu wordt gevraagd om een titel en de key zelf. Bedenk voor titel een betekenisvolle naam en vul deze in. Vul bij "Key"
de inhoud van je ssh-key in. Deze is gemakkelijk op het klembord te plaatsen (en met Ctrl+v te plakken)
door `$ clip < ~/.ssh/id_ed25519.pub` uit te voeren in een terminal. Werkt dit niet, zoek de ssh-key dan handmatig op en
kopieer deze.

Klik vervolgens op de knop "Add SSH key" en vul je wachtwoord in als daar om gevraagd wordt.

## De ssh-verbinding testen

Nu de ssh-key gegenereerd is en succesvol aan je GitHub-account toegevoegd is, kun je testen of het werkt. Om dit te
testen, voer je het volgende commando uit in de terminal:

```
$ ssh -T git@github.com
```

Mogelijkerwijs wordt er nu een waarschuwing getoond die er ongeveer als volgt uitziet:

```
> The authenticity of host 'github.com (IP ADDRESS)' can't be established.
> RSA key fingerprint is SHA256:nThbg6kXUpJWGl7E1IGOCspRomTxdCARLviKw6E5SY8.
> Are you sure you want to continue connecting (yes/no)?
```

Controleer of de fingerprint overeen komt
met [GitHubs RSA public key fingerprint](https://docs.github.com/en/github/authenticating-to-github/githubs-ssh-key-fingerprints)
. Komt het overeen, type dan `yes` om door te gaan.

Hierna verschijnt er een bericht:
```
> Hi gebruikersnaam! You've successfully authenticated, but GitHub does not
> provide shell access.
```
Verifieer dat de gebruikersnaam klopt. Als dat zo is, is je ssh-key succesvol toegevoegd aan je GitHub-account en werkt deze naar behoren. Nu kun je bij het [clonen van een project](./git_commando_instructions/git-clone-repository.md) gebruik maken van de SSH-optie.

[HOME](./README.md)