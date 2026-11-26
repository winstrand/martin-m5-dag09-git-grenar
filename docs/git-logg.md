# Git-logg

Klistra in utskrifter och svara på frågorna. Det här är din dokumentation av dagens arbete.

## 1. Utgångsläget

Skriv ut `git log --oneline --graph --all` direkt efter att du klonat. Klistra in här:

```
$ git log --oneline --graph --all
* 5a5841d (HEAD -> main, origin/main, origin/HEAD) Modul 5 i TypeScript med Vite
* 3804533 Add files via upload
* f7a13a4 Add files via upload
* c9a0075 Initial commit
```

## 2. Merge utan konflikt

Klistra in `git log --oneline --graph --all` efter merge:

```
$ git log --oneline --graph --all
*   f962648 (HEAD -> main) Merge branch 'meny-nyheter'
|\
| * 827db04 (meny-nyheter) Lägg till te på menyn.
* | 8ec2815 Lägg till telefonnummer
|/
* 5a5841d (origin/main, origin/HEAD) Modul 5 i TypeScript med Vite
* 3804533 Add files via upload
* f7a13a4 Add files via upload
* c9a0075 Initial commit
```

Fråga: Vad är skillnaden mellan en _fast-forward_-merge och en merge som skapar en egen merge-commit? Svara med egna ord:
fast-forward 'rätar' ut main så att det är en rak linje, då det inte finns några andra som blokerar. I annat fall så ligger ändringarna parallellt och då får man en 'båge' som visar att det är två olika spår

## 3. Konflikten

Klistra in filen med konfliktmarkörerna, precis som den såg ut innan du löste den:

```
# Öppettider

Vardagar: 07–18
<<<<<<< HEAD
Helger: 10–17
=======
Helger: 09–18
>>>>>>> oppettider-sommar
Röda dagar: stängt

```

Fråga: Vad betyder `<<<<<<< HEAD`, `=======` och `>>>>>>> grennamn`?
<<<< - Visar var HEAD (huvud branchens) innehåll börjar i konflikten
==== - Visar var HEAD slutar och nästa börjar i konflikten

> > > > - Visar var grenens unika delar i konflikten slutar

Hur löste du den, och varför blev det så?
Jag valde att lägga till båda för att sedan ändra till ett helt nytt värde på raden som diffade

## 4. Ångra

Vad är skillnaden mellan `git restore`, `git revert` och `git reset`? Vilken är säkrast när ändringen redan är pushad?

## 5. Pull request

Länk till din pull request (på ditt eget repo):

## 6. Reflektion

Vad är det värsta som kan hända om man kör `git push --force` på en gren som andra använder?
