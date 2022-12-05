# Labb 2 - Micro services och Test

Ett sätt att bygga upp funktionalitet åt en större organisation eller företag är att tillämpa
arkitekturmönstret mikrotjänster, vilket både löser en hel del problem men samtidigt introducerar
nya svårigheter.

Denna labben går ut på att utveckla två stycken ``microservices`` och en ``API-Gateway`` som tillsammans utgör en webbtjänst. **Varje** medlem i gruppen ansvarar för var sin ``microservice`` eller ``gatewayen`` men också för ``enhetstesterna`` för en av de andra.

Alla microservices ska utvecklas enligt **TDD**, alltså ``enhetstester`` ska skrivas först för varje publik metod i varje ``microservice`` och ``gatewayen``. Ni behöver inte följa TDD strikt utan kan skriva enhetstester som testar slutgiltiga funktionaliteten direkt. Alltså ni måste inte göra första iterationen om ni inte vill det.

Vi vill kunna lägga till samt läsa information
från tjänsterna vilket gör att dessa behöver supporta minst **GET** och **POST**. Men vill man kan man
även implementera **PUT** och **DELETE**.


### [Creating a simple API Gateway in ASP.NET Core](https://medium.com/streamwriter/api-gateway-aspnet-core-a46ef259dc54)
## Genomförs i grupp er om 3 personer

## Labben består av 3 delar 

## Del 1:
Ni ska tillsammans i gruppen enas om en webbtjänst som ska byggas. 
Ni ska också tillsammans skriva API-specifikationer för samtliga ``microservices`` och ``gateway``. Bestämma vilken typ av databas som ska användas och vem som ansvarar för vilken del. Sätt sedan upp repo och projekten med alla relevanta ``Interface`` och ``databasmodeller`` för att kunna skriva ``tester``.


### Förslag på projekt:
En tjänst lagrar pizzor med deras namn, ingredienser
och pris medans en annan fristående tjänst lagrar beställningar på pizzor.

En tjänst som lagrar information om användare så som namn, adress,
länk till profilbild m.m. och en annan tjänst som lagrar meddelanden med en rubrik, text, datum samt id för vilken användare som postat meddelandet.
## Del 2.0: UnitTester
Varje medlem i gruppen ansvarar för att skriva ``enhetstester`` för en ``microservice`` (eller ``gateway``) som någon annan i gruppen ska implementera.

## Del 2.1: Microservices och API-Gateway
Efter att ``enhetstesterna`` är färdiga ansvarar var och en för en egen microservice (eller ``gateway``) som ska följa specifikationerna och passera de tester som är skrivna.

Upprepa 2.0-2.1 Tills ni är klara.

## Del 3: Reflektioner och Analys
När man är färdig med både sina tester och sin ``microservice`` (eller ``gateway``) ska alla skriva en kortfattad analys av arbetet. Här ska man analysera sitt eget arbete. Svara på dessa frågor men utöka gärna om det behövs.
* Vad har du lärt dig om enhetstester och TDD?
* Vad har du lärt dig om ``microservices``?
* Vad hade du gjort annorlunda om du fick uppgiften igen?

## VG-Uppgift
För att använda alla endpoints utom GET frågor så vill vi veta identiteten på den som anropar våra
tjänster. Lägg till funktionalitet för att hantera JWT i api gateway och även skicka vidare den
informationen till bakomliggande tjänster.

### [JWT Authentication for Microservices in ASP.NET Core](https://medium.com/streamwriter/jwt-authentication-for-microservices-in-asp-net-core-b350c1a3e9fa)


## Redovisning

Ni ska lämna in det som behövs för att köra projektet med eventuella anvisningar. Ett tips kan vara att jobba i ett github-projekt och bjuda in mig i det.

## Bedömning

### Krav för G
* Alla publika metoder i alla microservices och i gatewayen ska ha relevanta tester.
* Ni har en(eller flera) API-spec för alla delar
* Frågorna i steg 3 är besvarade tydligt och med självreflektion
* Det ska gå att utföra minst **Get** och **Post** requests på båda microservices.
* Ni har utvecklat projektet på ett sätt som är löst kopplat
  
### Krav för VG

* Extra uppgift för VG är genomförd
* Man har tillämpat SOLID i utvecklingen

## Deadline är 23/12-2022 kl 23:59
Sen inlämning innebär komplettrering i Februari.