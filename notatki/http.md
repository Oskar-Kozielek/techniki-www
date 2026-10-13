Telehack komendy:

1. Rain - uruchamia animacje deszczy w terminalu
2. minesweeper - uruchamia gre w sapera 
3. morse "tekst" - koduje nam tekst napisany po komendzie mors na kod morsa i wyświetla wynik


------

przy rządaniu info.cern.ch dostajemy kod 200 czyli wszystko jest OK i poprawną odpowiedz natomiast przy rządaniu githuba z http dostajemy kod 301, czyli przeniesienie strony jest tak ponieważ github wymaga połaczenia przez https, jeśli zamienimy w zapytaniu http na https to dostaniemy kod 200 i oczekiwaną odpowiedź.
przy podaniu URL strony która nie istnieje dostajemy kod 404 not found.

-------

Polecenie w konsoli (na stronie info.cern.ch): document.querySelectorAll('*').length
wynik: 16

Pomiary z zakładki Network dla strony info.cern.ch:

liczba żądań :      2
przesłane dane:     2,05kB / 2,53 kB
czas ładowania:     899 ms
elementy DOM:       448 ms
