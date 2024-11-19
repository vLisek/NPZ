# 📚 Laboratorium 02

## 📝 Opis
To repozytorium zawiera rozwiązanie zadań z Laboratorium 2. Wszystkie zadania znajdują się w tym pliku `(README.md)`.

## 📂 Zadania
### Uruchomić Git Bash.
<br></br>
### Podpunkt 2.1. 
Ustawić globalną nazwę użytkownika oraz email użytkownika.
```bash
$ git config --global user.name "student"
```
```bash
$ git config --global user.email "student@ur.edu.pl"
```
Utworzyć folder o nazwie piosenki. 
```bash
$ mkdir piosenki
```
```bash
$ cd piosenki
```
Zainicjalizować w nim puste repozytorium Git:
• Katalog roboczy będzie zawierał pliki projektu (na potrzeby tego laboratorium pliki tekstowe),
• Folder `.git` (reprezentujący repozytorium lokalne, wraz z przechowalnią). 
```bash
$ git init 
```

<br></br>
### Podpunkt 2.2. 
Utworzyć pusty plik tekstowy `moves.txt` za pomocą edytora tekstowego lub:
```bash
$ touch moves.txt
```

<br></br>
### Podpunkt 2.3. 
Sprawdzić stan katalogu roboczego i przechowalni. W jakim stanie jest `moves.txt`?
```bash
$ git status
```
Wynik:
```
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        moves.txt

nothing added to commit but untracked files present (use "git add" to track)
```

<br></br>
### Podpunkt 2.4. 
Dodać obecną w katalogu roboczym wersję pliku `moves.txt` do przechowalni (co także włącza śledzenie tego pliku).
```bash
$ git add moves.txt
```

<br></br>
### Podpunkt 2.5. 
Sprawdzić stan katalogu roboczego i przechowalni. W jakim stanie jest `moves.txt`?
```bash
$ git status
```
Wynik:
```
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   moves.txt
```

<br></br>
### Podpunkt 2.6.
Wykonać migawkę projektu, czyli zatwierdzenie obecnych wersji plików z przechowalni do repozytorium lokalnego (commit):
• wpisać poniższą komendę,
• po otworzenia edytora VIM z domyślnym przykładem opisu, napisać w pierwszej linijce „Utworzenie moves” (jeśli litery się nie pojawiają to wcisnąć „i”),
• następnie:
    – wcisnąć Esc,
    – wcisnąć Shift oraz ; (żeby powstał :),
    – wpisać litery wq (write i quit),
    – wcisnąć Enter. 
```bash
$ git commit
```

<br></br>
### Podpunkt 2.7.
Sprawdzić stan katalogu roboczego i przechowalni.
```bash
$ git status
```

<br></br>
### Podpunkt 2.8.
Utworzyć nową gałąź o nazwie snoop-dogg (ale pozostać na gałęzi master).
```bash
$ git branch snoop-dogg
```

<br></br>
### Podpunkt 2.9.
Wyświetlić nazwy obecnie istniejących gałęzi. Która gałąź jest obecnie ustawiona?
```bash
$ git branch --list
```
Wynik:
```bash

```

