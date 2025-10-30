# Wstęp
Proste (mam nadzieję) wytłumaczenie programowania w C dla ludzi z mojej klasy którzy mniej ogarniają. Docelowo chce tłumaczyć wszystko z lekcji, ale zobaczymy jak wyjdzie. Na razie opisze nowości które drugiej grupie spowodowały lekkie problemy
# Tablice
A więc tablice. Ehh. Tablica tak właściwie, to zbiór z matmy (nie mylić z przedziałem). Jest jednak parę różnic. W tablicy elementy mogą się powtarzać i <ins>**mogą zawierać tylko jeden typ danych**</ins>. To ważne. Ale tablice mogą mieć różny typ danych.
```C
int tablica0[5];
float tablica1[5];
double tablica2[5];
```
Kod powyżej tworzy trzy tablice. Każda może zmieścić 5 elementów. Każda składa się z danych o innych typach. Definuje się je jak zmienne, tylko po nazwie dodaje [], w którym zapisuje się maksymalną ilość elementów. I tu zaczynają się lekkie schody.
```C
int tablica[3] = {9, 18, 27};
tablica[0] == 9;
tablica[2] == 27;
```
Liczbę elementów zapisujemy licząc od 1. Jak zapiszemy `int tablica[1]`, to zapiszemy w tablicy jeden element. Jednak numer elementu liczymy od 0. Tak jak zapisałem wyżej. Tablica ma trzy elementy, z czego element numer 0 równy jest 9, a element numer 2 jest równy 27. Element numer 3 nie istnieje w tej tablicy, bo byłby to 4 element w tej tablicy. Kumamy? mam nadzieję. Jeśli chcemy wywołać zmienną z tablicy, piszemy nazwę tablicy i po niej (bez spacji) piszemy numer elementu w []. O tak: `tablica[0]`. 
Na marginesie: zapis `zmienna == x` bez niczego jest niepoprawny i nic nie robi, zapisuje go dla zobrazowania.
