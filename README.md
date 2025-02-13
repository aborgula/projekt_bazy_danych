Ten projekt zawiera strukturę i dane bazy PostgreSQL dla systemu zarządzania usługami sprzątania.
Baza danych przechowuje informacje o klientach, pracownikach, usługach oraz zamówieniach. Dodatkowo zawiera widoki, funkcje i wyzwalacze ułatwiające analizę danych.

 Struktura bazy danych

Baza danych składa się z kilku tabel, widoków i funkcji:

 Tabele:

klienci – przechowuje informacje o klientach (id, imię, nazwisko, adres, telefon).

pracownicy – lista pracowników (id, imię, nazwisko, stanowisko).

uslugisprzatania – dostępne usługi sprzątania (id, nazwa usługi, cena).

zleceniasprzatania – zamówienia usług (data, klient, pracownik, usługa).

modyfikacje – przechowuje datę ostatniej modyfikacji danych.

�️ Widoki:

task_1 – wyszukuje klientów, którzy zamówili „Czyszczenie dywanów”.

task_2 – zlicza liczbę zamówień na „Czyszczenie dywanów” i sumuje przychody.

 Funkcje:

task_3 – oblicza łączny koszt zamówień danego klienta w podanym zakresie dat.

task_4 – wyzwalacz aktualizujący modyfikacje po zmianie danych.

 Wyzwalacze:

Aktualizują modyfikacje po edycji uslugisprzatania i zleceniasprzatania.
