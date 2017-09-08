# Arbetsprov - TODO

Läs igenom hela readme.md innan du börjar.

Denna guide är skriver med förutsättning att arbetet utförs på OSX. Alla kommandon är platformsoberoende, dock installationslänkar kan variera.

Din uppgift kommer bestå av 2 delar.
Slutprodukten ska bestå av en fungerande applikation som visas upp för IT-avdelningen.

Projektet ska skrivas i ramverket Laravel [läs mer på laravel.com](https://laravel.com/docs/5.5)

## Uppgift - TODO-applikation
### Beskrivning
Applikationen ska hantera projekt och uppgifter i projekt. Applikationen ska kunna ha **ett eller flera projekt**. Varje projekt ska innehålla en lista av **inga till många** uppgifter. Applikationen ska kunna skapa, visa, lista, ändra och ta bort uppgifter i ett projekt. Det ska också gå att skapa, visa, lista, ändra och ta bort projekt.

### Krav
    - Användaren måste ges möjlighet att skapa projekt med ett namn.
    - Projektets namn måste anges.
    - Användaren måste ges möjlighet att ändra namnet på projektet.
    - Användaren måste ges möjlighet att ta bort ett projekt med tillhörande uppgifter.
    - Användaren måste kunna se alla befintliga projekt.

    - Användaren måste ges möjlighet att skapa en uppgift med namn och beskrivning i ett projekt.
    - Uppgiftens namn måste anges.
    - Användaren måste ges möjlighet att ändra namn på uppgifter.
    - Användaren måste ges möjlighet att ändra beskrivning på uppgifter.
    - Användaren måste ges möjlighet att markera en uppgift som 'klar' respektive 'ej klar'.
    - Användaren måste ges möjlighet att ta bort en uppgift.
    - Användaren måste kunna se alla uppgifter tillhörande ett projekt.

    - Projekt och uppgifter måste sparas i en databas.

## Förutsättningar
* [Docker](https://docs.docker.com/docker-for-mac/install/)
* [Git](https://git-scm.com/download/mac)

## Setup
* Klona repot [gifted_lamport](https://github.com/50kolon2/gifted_lamport)
    * [Läs mer på help.github.com](https://help.github.com/articles/cloning-a-repository/)
* Från projektroten kör `$ docker-compose up -d`
    * [Läs mer på docs.docker.com](https://docs.docker.com/compose/)
* Installera dependencies genom att köra `$ docker-compose exec web composer install`
    * [Läs mer på getcomposer.org](https://getcomposer.org/doc/00-intro.md)
* Sidan går att nå via webläsaren på [http://localhost:8080](http://localhost:8080)

## Tips
* För att komma in i containern så man kan köra laravel-kommandon  kör `$ docker-compose exec web sh`
    * T.ex `php artisan migrate`
* För att lista alla containers kör `$ docker ps -a`
    * [Läs mer på docs.docker.com](https://docs.docker.com/engine/reference/commandline/ps/)
* Ett bra program för att hantera databasen är [Sequel Pro](https://www.sequelpro.com/)
* MySQL-databasen finns att nå på `127.0.0.1:33060`
    * Databasnamn: `dbname`
    * Användarnamn: `root`
    * Lösenord: `example`

## Kontakt
Vid frågor kontakta Sam Nydahl via sam.nydahl@smb.nu
