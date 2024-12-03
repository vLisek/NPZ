# 📚 Laboratorium 05

## 📝 Opis
To repozytorium zawiera wyjaśnienia poszczególnych komend z laboratorium 05. Wszystkie zadania znajdują się w tym pliku `(README.md)`.

## 📂 Zadania


##  Komendy 🧑‍💻

### Podpunkt 1. 
`git restore`
Przywraca zmiany z ostatniego commita lub usuwa zmiany w plikach roboczych (ang. working directory).

### Podpunkt 2. 
`git restore --staged`
Usuwa pliki ze staging area (indeksu), ale nie modyfikuje ich w roboczym katalogu.

### Podpunkt 3. 
`git commit --amend -m "..."`
Edytuje ostatni commit, umożliwiając zmianę wiadomości lub dodanie nowych plików.

### Podpunkt 4. 
`git commit --amend --no-edit`
Nadpisuje ostatni commit bez zmiany jego wiadomości.

### Podpunkt 5. 
`git stash`
Tymczasowo zapisuje zmiany, oczyszczając katalog roboczy, aby móc przełączyć się na inne zadanie.

### Podpunkt 6. 
`git merge`
Łączy zmiany z wybranej gałęzi do aktualnej gałęzi.

### Podpunkt 7. 
`git rebase`
Przenosi commity z jednej gałęzi na wierzch innej, zachowując liniową historię.

### Podpunkt 8. 
`git reset --soft HEAD^`
Cofnięcie ostatniego commita, pozostawiając zmiany w staging area.

### Podpunkt 9. 
`git reset --mixed HEAD^`
Cofnięcie ostatniego commita, przenosząc zmiany do katalogu roboczego.

### Podpunkt 10. 
`git reset --hard HEAD^`
Usunięcie ostatniego commita oraz wszelkich zmian z katalogu roboczego i staging area.

### Podpunkt 11. 
`git rebase -i HEAD~2 (squash)`
Łączenie dwóch ostatnich commitów w jeden w celu uproszczenia historii.

### Podpunkt 12. 
`git checkout hash_commita`
Przełącza na stan kodu z konkretnego commita (na podstawie jego hasha).

### Podpunkt 13. 
`git branch -d`
Usuwa lokalną gałąź, jeśli została zmergowana do innej gałęzi.

### Podpunkt 14. 
`git branch -D`
Wymusza usunięcie lokalnej gałęzi, nawet jeśli nie została zmergowana.

### Podpunkt 15. 
`git revert`
Tworzy nowy commit cofający zmiany wprowadzone przez wybrany commit.

### Podpunkt 16. 
`git rm`
Usuwa pliki z katalogu roboczego i staging area.

### Podpunkt 17. 
`git rm --cached`
Usuwa pliki ze staging area, pozostawiając je w katalogu roboczym.

### Podpunkt 18. 
`git archive`
Tworzy archiwum (np. ZIP) z wybraną wersją projektu, bez repozytorium Git.
