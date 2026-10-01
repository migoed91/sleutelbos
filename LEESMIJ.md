# Sleutelbos – offline installeren

Sleutelbos is een installeerbare webapp (PWA). Je zet de bestanden één keer
online. Daarna installeer je de app op je telefoon. Vanaf dat moment werkt
hij volledig zonder internet en maakt hij nooit meer verbinding.

## 1. Eenmalig online zetten (gratis, via GitHub Pages)
1. Maak een gratis account op github.com.
2. Maak een nieuwe repository, bijvoorbeeld `sleutelbos`, en zet hem op *Public*.
3. Kies *Add file → Upload files* en upload alle bestanden uit deze map.
4. Ga naar *Settings → Pages*. Kies bij *Branch* de optie `main` en `/ (root)` en klik *Save*.
5. Na een minuut staat de app op `https://<jouw-naam>.github.io/sleutelbos/`.

De bestanden bevatten geen wachtwoorden. Je kluis ontstaat pas op je telefoon.

## 2. Installeren op je telefoon
**iPhone (Safari):** open de link, tik op Deel en kies *Zet op beginscherm*.
**Android (Chrome):** open de link, tik op ⋮ en kies *App installeren*.

Open de app daarna één keer met internet aan, zodat hij volledig wordt opgeslagen.
Daarna kun je vliegtuigmodus aanzetten om te testen of hij offline werkt.

## Goed om te weten
- Je kluis staat alleen in deze geïnstalleerde app op dit toestel. Verwijder je
  de app of wis je de browsergegevens, dan is de kluis weg. Maak daarom af en toe
  een back-up via *Instellingen → Exporteren als CSV* en bewaar die veilig.
- De app blokkeert zelf elke netwerkverbinding (`connect-src 'none'`).
- Na het installeren werkt de app alleen met de opgeslagen versie. Wil je een
  nieuwe versie gebruiken? Pas dan `VERSION` aan in `sw.js`, upload opnieuw en
  open de app één keer met internet aan.
