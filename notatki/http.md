Ćwiczenie 1

1. Rain - uruchamia animacje deszczu w terminalu
2. minesweeper - uruchamia gre w sapera 
3. morse "tekst" - koduje podany tekst na kod morsa i wyświetla wynik

Współczesny Web oferuje podobne funkcje, np. gry przeglądarkowe, animacje i konwertery tekstu. Różnica polega na tym, że dawniej wiele takich funkcji uruchamiało się w terminalu, a dziś korzystamy z graficznych interfejsów stron internetowych.

------
Ćwiczenie 2

| Strona | Metoda | Ścieżka | Kod HTTP |
|:-------|:------:|:-------:|---------:|
| info.cern.ch | GET | / | 200 OK |
| github.com | HEAD | / | 301 Moved Permanently |
| Nieistniejąca strona | HEAD | /nie-ma-takiej | 404 Not Found |

przy rządaniu info.cern.ch dostajemy kod 200 czyli wszystko jest OK i poprawną odpowiedz natomiast przy rządaniu githuba z http dostajemy kod 301, czyli przeniesienie strony jest tak ponieważ github wymaga połaczenia przez https, jeśli zamienimy w zapytaniu http na https to dostaniemy kod 200 i oczekiwaną odpowiedź.
przy podaniu URL strony która nie istnieje dostajemy kod 404 not found.

-------

Ćwiczenie 3

| Pomiar | info.cern.ch | spacejam.com/1996 | onet.pl |
|:-------|---------------:|-------------------:|----------:|
| Liczba żądań | 2 | 18 | 356 |
| Przesłane dane (kB) | 2,05 | 64,36 | 26030|
| Czas ładowania (ms) | 899 | 2006 | 3006 |
| Elementy DOM | 16 | 119 | 1397 |
| Najcięższy plik (typ) | vnd.microsoft.icon | gif | script js |

Różnice wynikają prawdopodobnie ze złożoności stron oraz liczby wykorzystywanych zasobów, takich jak obrazy i skrypty JavaScript.
 W przypadku Onetu rejestrowanie zatrzymałem po około minucie, ponieważ strona nieustannie wysyłała kolejne żądania w tle i ich liczba
 rosła ciągle co pare sekund, dlatego jego wyniki należy traktować jako pomiar wykonany w określonym czasie.
Na serwisie onet zaobserwowałem również że część żadań została zablokowana przez mój adblock.
