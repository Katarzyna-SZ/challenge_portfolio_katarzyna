# TASK 1

### Spis treści:
1. [Subtask 1 - wynik testu](#subtask1)
2. [Subtask 3 - Dlaczego zdecydował_ś się na udział w challenge portfolio?](#subtask2)
3. [Subtask 4 - Testy eksploracyjne: poznaj aplikację:](#subtask3)  
   - [Na czym polega ta aplikacja? Do czego służy?](#punkt1)
   - [Jakie funkcjonalności znajdują się w aplikacji? Do czego służą?Czy są intuicyjne, czy może byś coś zmienił_a?](#punkt2) 
   - [Oceń interfejs aplikacji (wygląd) – czy Ci się podoba, czy nie?](#punkt3)
   - Czy aplikacja jest intuicyjna?
   - Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem?     
<hr>

## <a name='subtask1'>  Subtask 1 - wynik testu </a>

Wynik testu: 8/10

## <a name='subtask2'>  Subtask 3 - Dlaczego zdecydował_ś się na udział w challenge portfolio? </a>

Zdecydowałam się wziąć udział w projekcie, ponieważ 7- tygodniowy program przedstawiony przez [DARE IT](https://www.dareit.io/challenges) jako jeden z nielicznych stawia przede wszystkim na **praktykę**. 
Mam nadzieję, że wraz z postępem prac **rozbuduję portfolio**, **usystematyzuję** samodzielnie zdobytą **wiedzę** oraz uzyskam **feedback od mentorów**, który wesprze mój rozwój zawodowy na nowej ścieżce kariery.💪🏻

## <a name='subtask3'>  Subtask 4 - Testy eksploracyjne: poznaj aplikację </a>

**Przedmiot testów:** Aplikacja webowa ⚽[Scouts Test](https://scouts-test.futbolkolektyw.pl/pl) **Dane wejściowe** 🔓login: user01@getnada.com hasło: Test-1234

👉<a name='punkt1'> **Na czym polega ta aplikacja? Do czego służy?** </a>

Aplikacja Scout Test przeznaczona jest dla łówców talentów piłki nożnej. Głównymi założeniami aplikacji jest stworzenie edytowalnej bazy danych graczy, prowadzenie statystyk oraz raportów z meczów w których uczestniczą.

👉<a name='punkt2'> **Jakie funkcjonalności znajdują się w aplikacji? Do czego służą? Czy są intuicyjne, czy może byś coś zmienił_a?** </a>

Podstawowe funkcjonalności aplikacji:

  - funkcja logowania do aplikacji za pomocą adresu e-mail i hasła,
  - funkcja przypomnienia hasła,
  - funkcja zmiany języka w oknie logowania na język angielski,
  - funkcja zakładania konta nowego użytkownika - poza zakresem testów,
  - funkcja dodania nowego gracza z okna znajdującego się na stronie głównej,
  - możliwość stworzenia rozbudowanego profilu gracza:
     * obowiązkowe pola do wypełnienia: imię, nazwisko, data urodzenia, główna pozycja.
     * dodatkowe pola do wypełnienia: email, telefon, waga, wzrost, dominująca waga, pozycja alternatywna, poziom rozgrywek, województwo, osiągniecia, dodatkowa opcja dodania języka, możliwość dodania linka z youtube, 
     pola zatytułowane *Łączy nas piłka*, *90 minut*, *profil facebook*.
  - funkcja edycji gracza, czyli edytowanie wczesniej zapisanych danych,
  - funkcja *dodaj mecz* - otwarcie nowego okna z formularzem - pola do wypełnienia opisują rozgrywkę w której uczestniczył dany zawodnik:
     * obowiązkowe pola do wypełnienia: drużyna zawodnika, drużyna przeciwna, zdobyte gole, utracone gole, data rozgrywki
     * dodatkowe pola do wypełnienia: meczy domowy, mecz wyjazdowy do zaznaczenia, kolor koszulki, liga, czas gry, numer, web match, general, recenzja
  - funkcja edytowania meczu, czyli informacji wcześniej zapisanych, dodatkowo poniżej pół do wypełnienia widnieje sekcja z *Lista zdarzeń*; brak informacji o możliwości edytowania
  - funkcja dodatnia i edytowania raportu z rozgrywek,
  - funkcja *Rozpocznij mecz*, czyli stworzenie symulacji najważniejszych akcji mających miejsce podczas rozgrywki.

📍Przykłady nieintuicyjnych funkcjonalności aplikacji + komentarz:
  - funkcja *DODAJ GRACZA* dostępna jest z przypadkowego kafelka o nazwie *LINKI POMOCNICZE* znajdującego się na stronie głównej; *Opcja dodaj gracza w obecnym układzie strony powinna być dostępna z panelu bocznego 
    znajdującego się po lewej stronie*;
  - funkcja dodawania i edytowania gracza powinna zostać uproszczona, tak aby użytkownik mógł wybrać konkretny wariant z rozwijanej listy np: wybrać poziomy rozgrywek czy główna pozycja zawodnika; wszystko w celu 
    ujednolicenia terminologii;
  - dopiero po dodaniu gracza mamy dostęp do głównych funkcjonalności w panelu bocznym takich jak *Mecz (Dodaj mecz)* i *Raport (Dodaj raport)*; jednakże funkcja *Dodaj raport* nie działa z zakładki Raport -> po wybraniu 
    kliknięciu w tekst *+ DODAJ RAPORT* użytkownik jest przekierowany do zakładki *Mecz* i dopiero z tego poziomu możemy dodać raport wybierając jedną z trzech *Akcji*;
    
    ![22](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/13d6d4be-1b9a-4de0-83aa-60b589cf90c6)

  - funkcja *Rozpocznij mecz*, czyli edytowanie/symulowanie akcji zawodnika totalnie nieintuicyjna -> brak dokumentacji, brak legendy na stronie; *Użytkownik powinien mieć dostęp do klarownej instrukcji obsługi edytora 
    wraz z objaśnieniem graficznym poszczególnych pół.*

👉<a name='punkt3'> **Oceń interfejs aplikacji (wygląd) – czy Ci się podoba, czy nie??** </a>













