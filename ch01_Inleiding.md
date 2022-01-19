# Inleiding

## Leeswijzer

Dit document beschrijft hoe Logius, afdeling Standaarden (hierna: Logius) de OAuth-NL profiel standaard beheert en hoe de bijbehorende governance is ingericht. In dit document wordt verder OAuth-NL gebruikt als afkorting voor de "NL GOV Assurance profile for OAuth 2.0" standaard.

## De NL GOV Assurance profile for OAuth 2.0 standaard (OAuth-NL)

De OAuth-NL standaard omvat een specifiek profiel voor het OAuth 2.0 profiel en is bedoeld om de beveiliging te verbeteren, grotere interoperabiliteit te waarborgen en bij te dragen aan een gestructureerde toepassing door Nederlandse Overheids organisaties.

De OAuth-NL is gebaseerd op het [International Government Assurance Profile (iGov) for OAuth 2.0 - Draft 03’ (Kortweg: het iGov-profile)](https://openid.net/specs/openid-igov-oauth2-1_0.html) van de "OpenID Foundation".  

Het nut en de werking van de standaard zijn duidelijk berschreven op de website van het Forum standaardisatie en voor de leesbaarheid hieronder over genomen:

### Nut

> NL GOV Assurance profile for OAuth 2.0 legt bindende afspraken vast over het gebruik van de de standaard OAuth 2.0 bij de Nederlandse overheid. In combinatie met onderliggende standaard OAuth 2.0 zorgt NL GOV Assurance profile for OAuth 2.0 ervoor dat de autorisatie van gebruikers van REST APIs van de overheid op een uniforme en eenduidige plaatsvindt
> [Bron: Forum standaardisatie](https://www.forumstandaardisatie.nl/open-standaarden/nl-gov-assurance-profile-oauth-20)

### Werking

> OAuth 2.0 is een open standaard voor de beveiliging van applicaties die gegevens uitwisselen met behulp van REST APIs. Met OAuth 2.0 kunnen gebruikers een website of webapplicatie autoriseren om hun persoonlijke gegevens via een REST API op te halen bij een ander systeem, zonder daarbij hun gebruikersnaam en wachtwoord uit handen te geven. OAuth 2.0 maakt hiervoor gebruik van ‘tokens’ die toegang geven tot specifieke gegevens van één gebruikersaccount voor een bepaalde duur.
> OAuth 2.0 is een generieke standaard die meestal nog aanvullende afspraken vereist voor de toepassing in specifieke domeinen. NL GOV Assurance profile for OAuth 2.0 legt nadere afspraken vast over het gebruik van OAuth 2.0 bij de Nederlandse overheid. Zo bepaalt NL GOV Assurance profile for OAuth 2.0 hoe applicaties zich bij elkaar moeten registreren en hoe autorisatiecodes veilig uitgewisseld moeten worden. OAuth 2.0 laat daarin namelijk nog te veel implementatieopties vrij.
> [Bron: Forum standaardisatie](https://www.forumstandaardisatie.nl/open-standaarden/nl-gov-assurance-profile-oauth-20)

### Status

De actuele versie van de OAuth-NL is v1.0. Deze versie is op 09-07-2020 door het OBDO vastgesteld op advies van het Forum Standaardisatie.  
De status van de standaard is ‘Verplicht (pas toe leg uit)’. Dit houdt kort gezegd in dat Nederlandse overheden en instellingen uit de (semi) publieke sector verplicht zijn deze standaard toe te passen op het moment dat zij REST API’s gaan gebruiken voor het ontsluiten van overheidsinformatie en/of functionaliteit naar gebruikers van websites, apps of webapplicaties. Dit is ook specifiek beschreven in het toepassingsgebied van de standaard:

> NL GOV Assurance Profile for OAuth 2.0 moet worden toegepast bij applicaties waarbij gebruikers of ‘resource owners’ impliciet of expliciet toestemming geven aan een dienst van een derde om namens deze toegang te krijgen tot gegevens via een REST API waarvoor ze recht van toegang hebben. Zie voor meer informatie over het [pas toe of leg uit beleid.](https://www.forumstandaardisatie.nl/node/229)

- De verplichting is gepubliceerd door het Forum Standaardisatie op:  
  - [forumstandaardisatie.nl/open-standaarden/nl-gov-assurance-profile-oauth-20](https://forumstandaardisatie.nl/open-standaarden/nl-gov-assurance-profile-oauth-20)
- Versie 1.0 van de OAuth-NL standaard is gepubliceerd op:  
  - [publicatie.centrumvoorstandaarden.nl/api/oauth/v1.0](https://publicatie.centrumvoorstandaarden.nl/api/oauth/v1.0)
- De laatste versie van de OAuth-NL is gepubliceerd op:  
  - [publicatie.centrumvoorstandaarden.nl/api/oauth/](https://publicatie.centrumvoorstandaarden.nl/api/oauth/)
- De laatste concept versie van de OAuth-NL standaard is gepubliceerd op:  
  - [logius-standaarden.github.io/OAuth-NL-profiel/](https://logius-standaarden.github.io/OAuth-NL-profiel/)
 
## Bomos

Logius richt de beheerorganisatie in conform het Beheer en OntwikkelModel voor Open Standaarden (BOMOS). Ook het beheer van de OAuth-NL standaard is op basis van BOMOS ingericht. Voor de beheerorganisatie heeft Logius een generiek beheermodel opgezet, waar het beheerplan van de OAuth-NL standaard is afgeleid.  

![Bomos model](media/Bomos_model_v2.svg "Bomos model")
> Figuur 1. Bomos model

Voor meer informatie over BOMOS zie ook de ['Publicatie-BOMOS-2i.pdf'](https://www.forumstandaardisatie.nl/sites/default/files/BFS/4-basisinformatie/publicaties/Publicatie-BOMOS-2i.pdf) van het Forum standaardisatie.  
BOMOS onderscheidt verschillende levenscyclusfases waarin een standaard zich kan bevinden. Deze fase bepaalt mede op welke beheeronderdelen meer of minder wordt ingezet. De verschillende fases zijn:  

1.Creatie/ontwikkeling
2.Introductiefase
3.Implementatie/groei
4.Volwaardige toepassing
5.Uitfaseren

![Bomos_levenscyclus](media/Bomos_levenscyclus_v2.svg "Bomos levenscyclus")
> Figuur 2. Bomos levenscyclus

De OAuth-NL standaard bevindt zich in de implementatie/groei fase. De eerste versie van de standaard is 16-03-2016 aangemeld bij het Forum Standaardisatie en op 09-07-2020 op de lijst van verplichte standaarden opgenomen. Vanuit verschillende overheden is samengewerkt aan de standaard en de verwachting is dat de deze standaard nog slechts beperkt ontwikkeling door gaat maken. Het gebruik en de toepassing van de OAuth-NL standaard groeit nog en is nog geen comodity bij alle overheden, hierdoor is van een volwaardige toepassing bij de beoogde doelgroep nog geen sprake.  

Dit heeft gevolgen voor het beheer van de standaard. Naast de groei in de aantallen toepassingen van de standaard is ook relevant dat eerst nog minor en major wijzigingen in de standaard op een correcte manier worden doorgevoerd en er veel informatie beschikbaar is die gebruikers helpt bij de implementatie van de standaard. Daarom is er komende tijd vooral aandacht voor:

- Het in de praktijk bestendigen van het beheer van de standaard;  
- Doorontwikkeling van de standaard;  
- Groei in het aantal toepassingen van de standaard;  
- Monitoring van het gebruik van de standaard;  
- Groei van de community rond de standaard.  

