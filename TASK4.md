# TASK 4 📲 
    
### Spis treści:
1. [Subtask 2 - Subtask 2 - Testowanie eksploracyjne i raportowanie błędów.](#subtask2)
2. [Subtask 3 - Subtask 3 - Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?](#subtask3)   
   - [Kto ma być użytkownikiem końcowym aplikacji?](#punkt1) 
   - [Czy według Ciebie aplikacja jest user friendly?](#punkt2)
   - [Jak byś usprawnił aplikację? Czy masz jakiś pomysł na dodatkową funkcjonalność?](#punkt3)
   - [Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?](#punkt4)     
<hr>

### <a name='subtask2'>☑️ Subtask 2 - Testowanie eksploracyjne i raportowanie błędów </a>

Testowanie eksploracyjne aplikacji natywnej [OLX App](https://play.google.com/store/apps/details?id=pl.tablica&hl=pl&gl=US&pli=1)
  - **System operacyjny:** Android
  - **Urządzenie mobilne:** Sony Xperia XZ1 G8342
  - **Czas testowania:** 1h

👉 [Link to Google Drive Disk with Subtask 2](https://docs.google.com/spreadsheets/d/1AlL74ImZRhPj_lSBnfEWEH5jvBPH2WSPeiKsD2yLzCc/edit#gid=0)

### <a name='subtask3'>☑️ Subtask 3 - Do czego służy ta aplikacja? Jaki jest cel tej aplikacji? </a>

Głównym założeniem aplikacji OLX jest możliwość publikowania ogłoszeń dotyczących między innymi sprzedaży, wymiany, oddawania za darmo, wypożyczania, dystrybucji dóbr, jak i usług. Dzięki aplikacji użytkownik w wygodny sposób wyszukuje różnorodne produkty w bardzo rozbudowanej bazie danych (tworzonej przez samych użytkowników), ma możliwość korzystniejszych zakupów po cenie niższej niż w innych sklepach internetowych lub stacjonarnych. Dodatkowo aplikacja pośrednio wspiera zrównoważony rozwój i idee szeroko pojętej idei "less waste", ponieważ umożliwia sprzedaż, wymianę lub oddanie używanych dóbr, które mogą posłużyć kolejnym użytkownikom.

📋 **Główne funkcjonalności aplikacji to między innymi:**

- dodawanie ogłoszeń  w ponad 20 kategoriach, a przy tym edytowanie, usuwanie ogłoszeń,
- chat z innymi użytkownikami aplikacji,
- tworzenie list “ulubionych” *Ogłoszeń*, jak i *Wyszukiwań*,
- transakcje sprzedaży i kupna,
- śledzenie przesyłek, zgłoszeń i zwrotów,
- dodawanie ogłoszeń o pracę,
- tworzenie profilu kandydata dla osób szukających pracy, w tym edytowania profilu, zapisywanie aplikacji,         
 generowanie CV, preferencyjne filtrowanie ofert pracy,
-rozbudowana funkcja filtrowania ogłoszeń.

💰 <a name='punkt1'> **Kto ma być użytkownikiem końcowym aplikacji?** </a>

Końcowym użytkownikiem aplikacji są osoby prywatne oraz firmy (jednoosobowe lub o innym statusie). Danych użytkowników możemy podzielić na dwie główne kategorie: sprzedawców i kupujących (klientów).

👍🏻 <a name='punkt2'> **Czy według Ciebie aplikacja jest user friendly?** </a>

W mojej ocenie aplikacja (build v 5.94.3) jest przyjaźna dla użytkownika. Design aplikacji jest czytelny, hierarchia informacji jest przemyślana. Użytkownik ma łatwy dostęp do najważniejszych funkcjonalności z dolnego paska nawigacji - ergonomiczny układ dla kciuków obsługujących aplikację 😉

Projekt przycisków, ikon, typografia są spójne. Środowisko użytkownika jest czytelne.🔠

Aplikacja zawiera solidnie zaprojektowane opcje wyszukiwania oraz filtrowania ogłoszeń, co pozwala na szybkie znalezienie produktów lub usług biorąc pod uwagę takie czynniki jak lokalizacja, kategoria, cena. Wprowadzona jest funkcja przewidywania tekstu tym bardziej ułatwia cały proces.🔍

Aplikacja jest dobrze zintegrowana z innymi platformami odpowiedzialnymi za operacje takie jak: transakcje finansowe, logistyka i transport towarów. Tym samym użytkownik intuicyjnie może przejść przez proces zakupu/sprzedaży. 💳

📈 <a name='punkt3'> **Jak byś usprawnił aplikację? Czy masz jakiś pomysł na dodatkową funkcjonalność?** </a>

Na podstawie szybkich testów eksploracyjnych stwierdzam, że aplikacja jest dobrze zaprojektowana i spełnia swoją funkcję. Subiektywnie rzecz biorąc przy kolejnych aktualizacjach można byłyby wziąć pod uwagę kwestie takie jak:

- Chat, który dostępny jest w wersji webowej. Teoretycznie łączy nas z pomocą - niestety nie działa on w poprawny sposób, 
  ponieważ i tak tylko przekierowuje użytkownika do formularza kontaktowego - upierdliwy bug dla aplikacji webowej 😅 
  Działający chat z natychmiastowa pomocą byłby bardzo dużym upgradem.
- Sugestia wprowadzenia “onboardingu” ze wskazówkami jak szybko dostać się do funkcjonalności innych niż “dodawanie 
  ogłoszenia”.
- Możliwość zmiany języka dla osób nie posługujących się biegle językiem polskim, ale chcącym korzystać z możliwości 
  aplikacji na terenie kraju w którym mieszkają oraz wymianę dóbr i usług bez ograniczeń językowych.
- Podbijając poprzedni punkt: real-time chat translation.
- Możliwość zweryfikowania seryjnego sprzedawcy i jego walidacja przez wprowadzenie “Odznaki” uczciwego sprzedawcy.

 🖥️ vs. 📱 <a name='punkt4'> **Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?** </a>

- Główną różnicą w testowaniu aplikacji internetowych i natywnych to **platforma i środowisko**. Aplikacje natywne 
  tworzone są dla określonej platformy np. iOS lub Android, natomiast aplikacja webowa dostęna jest przez przeglądarkę 
  internetową, a więc testujemy na różnych przeglądarkach i platformach. 
- Aplikacje natywne szerzej korzystają z funkcji urządzenia np. aparat. kontakty, lokalizacja, więc weryfikujemy czy te 
  funkcje działaja poprawnie. Są instalowane na urządzeniu użytkownika, wieć potrzebujemy konkretne urządzenie (pomijam 
  celowo symulatory), by przetestowac proces instalacji i aktualizacji
- Na pewno testy wydajności dają inne wyniki, pnieważ aplikacjie natywne zazwyczaj mają lepsza reaktywność, jako że są 
  zoptymalizowane do pracy pod kątem konkretnej platformy.
- Aplikacje webowe są dostępne online, wymagane jest połączenie z internetem.
- Testowanie interfejsu użytkownika i doświadczenia różni się ze względu na wzorce interakcji i projekt graficzny.
- Podczas testowania webowego szerzej testuje się kompatybilność aplikacji, ponieważ ta musi działać na różnych 
  przeglądarkach internetowych i urządzeniach.
- Różnice w testowaniu aplikacji webowych i natywnych mogą być widoczne w doborze narzędzi testowcyh np. frameworków przy 
  automatyzacji testów, które będą stanowiły większy procent przy testowaniu aplikacji natwynych.





