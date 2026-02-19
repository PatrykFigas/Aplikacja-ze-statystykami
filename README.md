APLIKACJA ZE STATYSTYKAMI PIŁAKRSKIMI


Mobilna aplikacja wspomagająca dostęp do danych zawodników w klubach piłkarskich. Projekt został zrealizowany jako praca inżynierska na kierunku Informatyka (specjalność: Programowanie) na Uniwersytecie WSB Merito.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Cel projektu

Celem aplikacji jest umożliwienie zarządzania danymi zawodników, kontrolowania statusu składek członkowskich oraz prezentowania statystyk sportowych w zależności od roli użytkownika:

- Administrator,

- Trener,

- Rodzic.

Aplikacja została zaprojektowana jako rozwiązanie mobilne działające na systemie Android, z możliwością dalszej rozbudowy na inne platformy dzięki technologii .NET MAUI.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Technologie

Projekt został wykonany przy użyciu:

- .NET MAUI,

- C#,

- SQLite – lokalna baza danych,

- Architektura MVVM,

- PBKDF2 – bezpieczne hashowanie haseł z użyciem soli,

- Visual Studio,

- Git, GitHub.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Architektura

Aplikacja została zaprojektowana w oparciu o architekturę warstwową:

- Warstwa prezentacji (UI – MVVM),

- Warstwa logiki biznesowej (Services),

- Warstwa dostępu do danych (SQLite),


Model danych obejmuje trzy główne encje:

- UserAccount – użytkownicy i role,

- Player – dane i statystyki zawodników,

- ParentChildLink – powiązanie rodzica z dzieckiem.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Role użytkowników

Administrator

- Dodawanie, edycja i usuwanie zawodników bez ograniczeń,

- Zarządzanie statusem składek,

- Przegląd rankingów i statystyk,

- Pełny dostęp do systemu.

Trener

- Zarządzanie zawodnikami ograniczone do swojego klubu,

- Aktualizacja statystyk,

- Ustawianie statusu składek,

- Przegląd rankingów drużyny.

Rodzic

- Podgląd danych dziecka,

- Sprawdzanie statystyk,

- Sprawdzenie statusu składki.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Bezpieczeństwo

Hasła przechowywane są w postaci zahashowanej (PBKDF2 + sól).

Kontrola dostępu oparta o role użytkowników.

Ograniczenie dostępu do danych na poziomie logiki biznesowej.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Funkcjonalności

- Rejestracja i logowanie użytkowników,

- Routing do odpowiedniego dashboardu w zależności od roli,

- Dodawanie, edycja i usuwanie zawodników,

- Wyszukiwarka zawodników,

- Ranking zawodników,

- Status składek członkowskich,

- Przypisanie dziecka do konta rodzica,

- Migracje schematu bazy danych.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Testowanie

Aplikacja została przetestowana manualnie na urządzeniu z systemem Android.


Zrealizowano scenariusze testowe obejmujące:

- Zarządzanie zawodnikami przez trenera,

- Weryfikację statusu składki w panelu rodzica, 

- Proces rejestracji i logowania użytkowników.

Wszystkie testy zakończyły się pozytywnie.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Możliwości dalszego rozwoju:

- Synchronizacja danych z serwerem zewnętrznym,

- Rozszerzenie aplikacji na inne platformy,

- Rozbudowa systemu rankingów,

- Powiadomienia dla użytkowników,

- Obsługa multimediów (zdjęcia, wideo).
