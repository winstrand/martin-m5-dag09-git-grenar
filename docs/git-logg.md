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
(klistra in)
```

Fråga: Vad är skillnaden mellan en _fast-forward_-merge och en merge som skapar en egen merge-commit? Svara med egna ord:

## 3. Konflikten

Klistra in filen med konfliktmarkörerna, precis som den såg ut innan du löste den:

```
(klistra in)
```

Fråga: Vad betyder `<<<<<<< HEAD`, `=======` och `>>>>>>> grennamn`?

Hur löste du den, och varför blev det så?

## 4. Ångra

Vad är skillnaden mellan `git restore`, `git revert` och `git reset`? Vilken är säkrast när ändringen redan är pushad?

## 5. Pull request

Länk till din pull request (på ditt eget repo):

## 6. Reflektion

Vad är det värsta som kan hända om man kör `git push --force` på en gren som andra använder?
