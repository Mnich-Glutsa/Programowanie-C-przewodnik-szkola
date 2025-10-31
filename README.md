# Wstęp
Proste (mam nadzieję) wytłumaczenie programowania w C dla ludzi z mojej klasy którzy mniej ogarniają. Docelowo chce tłumaczyć wszystko z lekcji, ale zobaczymy jak wyjdzie. Na razie opisze nowości które drugiej grupie spowodowały lekkie problemy. Niestety, czytanie tego dokumentu nie nauczy was programowania. <ins>**Do tego wymagane jest regulare ćwiczenie.**</ins> Polecam zacząć robić małymi kroczkami jakieś swoje projekty. Jakie tylko chcecie. Dwie/trzy godzinki tygodniowo powinny wystarczyć. Programowanie to przede wszystkim sztuka myślenia jak programista. A tego trzeba się nauczyć.

## [kliknij tutaj by otworzyć spis treści](spis_tresci.md)

# #include `<iostream>`
Musi się to znajdować na początku każdego waszego programu. Dlaczego? Dowiecie się później. Nie teraz.

# Główna funkcja programu `int main()`
Jest to główna funkcja programu. To w niej będzie znajdywał się cały główny kod. Jeśli kod, napiszemy poza funkcją, tak o, losowo, to o ile nie jest to inicjalizacja zmiennej - nie wykona się on, albo kompilator wyrzuci błąd. Funkcja musi kończyć się `return 0;`. Wtedy program zakończy swoje działanie kodem 0.

# Pierwszy program i `printf()`
`printf()` służy do prostego wyświetlania informacji w formie tekstu. Składnia tej funkcji wygląda tak: `printf("tutaj dowolny tekst")`. No, to napiszmy najprostszy program.

```C
#include <iostream>

int main() {
    printf("Hello World!");

    return 0;
}
```

Wynikiem działania programu będzie:

```
Hello World!
```

# Zmienne
Zmienna to po prostu miejsce do przechowania jakiejś informacji. Na razie interesują nas liczby. Mamy trzy typy liczb jaka może przechować zmienna, ale interesują nas na razie dwie

```C
int liczba_calkowita = 5;
float liczba_rzeczywista = 0.123456;
```

`int` przechowuje liczbę całkowitą. `float` liczbe z 6-7 cyframi po przecinku. Proste, nie? Wartość zmiennej można w programie zmienić. Prosty przykład:

```C
#include <iostream>

int main() {
    int calkowita = 1;
    float z_przecinkiem = 1.235;

    printf("x = %d", x);
    y = y + x;
    printf("y = %d, y");

    return 0;
}
```

# Tablice
A więc tablice. Ehh. Tablica tak właściwie, to zbiór z matmy (nie mylić z przedziałem). Jest jednak parę różnic. W tablicy elementy mogą się powtarzać i <ins>**mogą zawierać tylko jeden typ danych**</ins>. To ważne. Ale tablice mogą mieć różny typ danych.

```C
int tablica0[5];
float tablica1[5];
```

Kod powyżej tworzy dwie tablice. Każda może zmieścić 5 elementów. Każda składa się z danych o innych typach. Definuje się je jak zmienne, tylko po nazwie dodaje [], w którym zapisuje się maksymalną ilość elementów. I tu zaczynają się lekkie schody.

```C
int tablica[3] = {9, 18, 27};
tablica[0] == 9;
tablica[2] == 27;
```

Liczbę elementów zapisujemy licząc od 1. Jak zapiszemy `int tablica[1]`, to zapiszemy w tablicy jeden element. Jednak numer elementu liczymy od 0. Tak jak zapisałem wyżej. Tablica ma trzy elementy, z czego element numer 0 równy jest 9, a element numer 2 jest równy 27. Element numer 3 nie istnieje w tej tablicy, bo byłby to 4 element w tej tablicy. Kumamy? Mam nadzieję. Jeśli chcemy wywołać zmienną z tablicy, piszemy nazwę tablicy i po niej (bez spacji) piszemy numer elementu w `[]`. O tak: `tablica[0]`.<br>
Na marginesie: zapis `zmienna == x` sam, bez niczego wokół, jest niepoprawny i nic nie robi. Zapisuję go tylko i wyłącznie dla zobrazowania posiadanych wartości.
