# 📚 Laboratorium 01

## 📝 Opis
To repozytorium zawiera rozwiązanie zadań z Laboratorium 1. Wszystkie zadania znajdują się w tym pliku `(README.md)`.

## 📂 Zadania

### Podpunkt 1. 
Pobrać na pulpit archiwum piosenki.zip, a następnie wypakować je, tak żeby na pulpicie był widoczny folder piosenki.

<br></br>
### Podpunkt 2. 
Otworzyć `Git Bash` z poziomu `Menu Start`, za pomocą odpowiedniej komendy przejść do folderu piosenki / otworzyć go bezpośrednio w folderze piosenki.
```bash
$ cd sciezka
```

<br></br>
### Podpunkt 3.
Wyświetlić zawartość folderu (nazwy plików, które się w nim znajdują), zwrócić uwagę na apostrofy i cudzysłowy otaczające nazwy plików.
```bash
$ ls
```
Wynik:
```bash
$ ls
'Blinding Lights.txt'     'Chained To The Rhythm.txt'   Roar.txt
"Can't Feel My Face.txt"  'Hot N Cold.txt'             'Save Your Tears.txt'
```

<br></br>
### Podpunkt 4.
Wyczyścić zawartość ekranu `(okna Git Bash’a)`.
```bash
$ clear
```
Możemy również użyć skrótu klawiszowego `Ctrl + L`

<br></br>
### Podpunkt 5.
Utworzyć foldery: `Katy Perry`, `The Weeknd`, `Shakira`.
```bash
$ mkdir "Katy Perry" "The Weeknd" Shakira
```
Wynik:
```bash
$ ls
'Blinding Lights.txt'     'Chained To The Rhythm.txt'  'Katy Perry'/  'Save Your Tears.txt'  'The Weeknd'/
"Can't Feel My Face.txt"  'Hot N Cold.txt'              Roar.txt       Shakira/
```

<br></br>
### Podpunkt 6.
Skopiować plik `Hot N Cold.txt` do folderu `Katy Perry`.
```bash
cp "Hot N Cold.txt" "Katy Perry"
```

<br></br>
### Podpunkt 7.
Przejść do folderu `Katy Perry` i sprawdzić czy plik tam istnieje.
```bash
$ cd Katy\ Perry/
```
Wynik:
```bash
$ ls
'Hot N Cold.txt'
```

<br></br>
### Podpunkt 8.
Wykonać komendę `explorer` aby otworzyć Eksplorator plików Windows w bieżącym
folderze.
```bash
$ explorer
```

<br></br>
### Podpunkt 9.
Powrócić do folderu `piosenki`.
```bash
$ cd ../
```

<br></br>
### Podpunkt 10.
Zmienić nazwę pliku `Hot N Cold.txt` na `HNC.txt`.
```bash
$ mv "Hot N Cold.txt" "HNC.txt"
```
Wynik:
```bash
$ ls
'Blinding Lights.txt'     'Chained To The Rhythm.txt'  'Katy Perry'/  'Save Your Tears.txt'  'The Weeknd'/
"Can't Feel My Face.txt"   HNC.txt                      Roar.txt       Shakira/
```

<br></br>
### Podpunkt 11.
Usunąć plik `HNC.txt`.
```bash
$ rm "HNC.txt"
```
Wynik:
```bash
$ ls
'Blinding Lights.txt'     'Chained To The Rhythm.txt'   Roar.txt               Shakira/
"Can't Feel My Face.txt"  'Katy Perry'/                'Save Your Tears.txt'  'The Weeknd'/
```

<br></br>
### Podpunkt 12.
Przy użyciu jednej komendy przenieść dwa pliki: `Roar.txt` oraz `Chained To The Rhythm.txt` do folderu `Katy Perry`.
```bash
$ mv "Roar.txt" "Chained To The Rhythm.txt" "Katy Perry"
```
Wynik:
```bash
$ ls
'Blinding Lights.txt'  "Can't Feel My Face.txt"  'Katy Perry'/  'Save Your Tears.txt'   Shakira/  'The Weeknd'/
```

<br></br>
### Podpunkt 13.
Wyświetlić zawartość folderu `Katy Perry` (bez przechodzenia do niego).
```bash
$ ls "Katy Perry"
```
Wynik:
```bash
$ ls "Katy Perry"
'Chained To The Rhythm.txt'  'Hot N Cold.txt'   Roar.txt
```

<br></br>
### Podpunkt 14.
Przenieść pozostałe trzy pliki do folderu `The Weeknd`, bez wymieniania ich nazw.
 ```bash
$ mv *.txt "The Weeknd"
```
Wynik:
```bash
$ ls
'Katy Perry'/   Shakira/  'The Weeknd'/
```

<br></br>
### Podpunkt 15.
Przejść do folderu `The Weeknd`.
```bash
$ cd The\ Weeknd/
```

<br></br>
### Podpunkt 16.
Wyświetlić pełną ścieżkę do obecnego folderu.
```bash
$ pwd
```

<br></br>
### Podpunkt 17.
Wyświetlić zawartość pliku `Blinding Lights.txt`.
```bash
$ cat Blinding\ Lights.txt
```
Wynik:
```bash
Yeah

I've been tryna call
I've been on my own for long enough
Maybe you can show me how to love, maybe
...
```

<br></br>
### Podpunkt 18.
Wyświetlić jego pięć pierwszych linijek.
```bash
$ head -n 5 "Blinding Lights.txt"
```

<br></br>
### Podpunkt 19.
Wyświetlić jego pięć ostatnich linijek.
```bash
$ tail -n 5 "Blinding Lights.txt"
```

<br></br>
### Podpunkt 20.
Wyświetlić go jeszcze raz, ale tym razem `„stronicowo”` (z przewijaniem zawartości).
```bash
$ less "Blinding Lights.txt"
```

<br></br>
### Podpunkt 21.
Wyświetlić linijki pliku `Can't Feel My Face.txt`, w których znajduje się słowo `love`.
```bash
$ grep -i "love" "Can't Feel My Face.txt"
```
Wynik:
```bash
She told me you'll never be in love, oh, oh, woo
But I love it, but I love it, oh
But I love it, but I love it, oh
All the misery was necessary when we're deep in love
She told me you'll never be in love, oh, oh, woo (yeah, yeah, yeah)
But I love it, but I love it, oh
But I love it (but I love it), but I love it, oh
But I love it (but I love it), but I love it (but I love it), oh
But I love it (but I love it), but I love it (but I love it), oh
She told me you'll never be in love, oh, oh, woo
But I love it (but I love it), but I love it (oh, I love it), oh
But I love it (but I love it), girl, I love it (but I love it), oh
But I love it (but I love it), but I love it, don't you think I can't
But I love it (when I'm with you baby), but I love it (when I'm with you baby)
```

<br></br>
### Podpunkt 22.
Wyświetlić linijki pliku `Can't Feel My Face.txt`, w których znajduje się słowo `love`, wraz z numerami linijek w których znajdują się te słowa.
```bash
$ grep -n "love" "Can't Feel My Face.txt"
```
Wynik:
```bash
9:She told me you'll never be in love, oh, oh, woo
12:But I love it, but I love it, oh
14:But I love it, but I love it, oh
18:All the misery was necessary when we're deep in love
24:She told me you'll never be in love, oh, oh, woo (yeah, yeah, yeah)
27:But I love it, but I love it, oh
29:But I love it (but I love it), but I love it, oh
31:But I love it (but I love it), but I love it (but I love it), oh
33:But I love it (but I love it), but I love it (but I love it), oh
38:She told me you'll never be in love, oh, oh, woo
41:But I love it (but I love it), but I love it (oh, I love it), oh
43:But I love it (but I love it), girl, I love it (but I love it), oh
46:But I love it (but I love it), but I love it, don't you think I can't
48:But I love it (when I'm with you baby), but I love it (when I'm with you baby)
```

<br></br>
### Podpunkt 23.
Wyświetlić liczbę linijek pliku `Can't Feel My Face.txt`.
```bash
$ wc -l "Can't Feel My Face.txt"
```
Wynik:
```bash
49 Can't Feel My Face.txt
```

<br></br>
### Podpunkt 24.
Powrócić do folderu piosenki.
```bash
$ cd
```

<br></br>
### Podpunkt 25.
Usunąć folder Shakira.
```bash
$ rm -r "Shakira"
```
Wynik:
```bash
$ ls
'Katy Perry'/  'The Weeknd'/
```

<br></br>
### Podpunkt 26.
Usunąć folder The Weeknd.
```bash
$ rm -r "The Weeknd"
```
Wynik:
```bash
$ ls
'Katy Perry'/ 
```

<br></br>
### Podpunkt 27.
Zapisać historię wykonanych poleceń do pliku `historia.txt`.
```bash
$ history > historia.txt
```
Wynik:
```bash
$ ls
 historia.txt  'Katy Perry'/
```

<br></br>
### Podpunkt 28.
Utworzyć pusty plik pusty.txt.
```bash
$ touch pusty.txt
```
Wynik:
```bash
$ ls
 historia.txt  'Katy Perry'/   pusty.txt
```

<br></br>
### Podpunkt 29.
Przejść do folderu użytkownika, bez używania komendy z `../`.
```bash
cd ~
```

<br></br>
### Podpunkt 30.
Za pomocą odpowiedniej komendy wyjść z `Git Bash’a`. 
```bash
exit
```
