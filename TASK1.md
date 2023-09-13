# TASK 1

### Spis treści:
1. [Subtask 1 - wynik testu](#subtask1)
2. [Subtask 3 - Dlaczego zdecydował_ś się na udział w challenge portfolio?](#subtask2)
3. [Subtask 4 - Testy eksploracyjne: poznaj aplikację:](#subtask3)  
   - [Na czym polega ta aplikacja? Do czego służy?](#punkt1)
   - [Jakie funkcjonalności znajdują się w aplikacji? Do czego służą?Czy są intuicyjne, czy może byś coś zmienił_a?](#punkt2) 
   - [Oceń interfejs aplikacji (wygląd) – czy Ci się podoba, czy nie?](#punkt3)
   - [Czy aplikacja jest intuicyjna?](#punkt4)
   - [Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem?](#punkt5)     
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

   Na ten moment interfejs aplikacji nie wygląda na zaprojektowany. Rekomendowałabym przeprowadzić audyt interfejsu pod względem UX/UI, stworzyć od nowa makietę produktu oraz zaprojektować atrakcyjną pod względem graficznym stronę główną wraz z oknami z poszczególnymi 
   funkcjonalnościami.

Główne mankamenty interfejsu aplikacji:
 - strona główna aplikacji składa się z przypadkowo ułożonych kafelek, 
 - przypadkowe umiejscowienie logo w niepoprawnym formacie
 - projekt graficzny interfejsu w ogóle nie nawiązuje do przedstawionego logo -> brak headera
 - pod logiem znajduje się link do Dev Team kontakt, który jest odnośnikiem do Slacka -> strona powinna zawierać stopkę z podstawową nawigacją
 - przyciski w edytorach graczy i meczów nie mają zróżnicowanej hierarchii, 
 - brakuje odstępów i marginesów,
 - aplikacja nie jest responsywna (test na podstawie Toggle device toolbar); okna nie skalują się poprawnie, utrudniona nawigacja.

👉<a name='punkt4'> **Czy aplikacja jest intuicyjna?** </a>

Na podstawie dotychczasowej eksploracji aplikaji uważam, że jest ona stanowczo mało intuicyjna. Używanie podstawowych funkcjonalności z poziomów innych niż boczna nawiagcja było uciążliwe. Ze względu na brak dokumentacji trudno było zrozumieć konieczność niektórych pól do uzupełnienia w profilu gracza oraz przy edycji meczu. Najmniej intuicyjną funkcjonalnością okazała się akcja *Rozpocznij mecz* z poziomu zakładki *Mecze*. Dopiero przypadkowe kliknięcia uruchamiały akcje, których w ostateczności nie byłam w stanie zrozumiec i edytować. 

👉<a name='punkt5'> **Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem?** </a>

 - Brak możliwości sprawdzenia funkcjonalności zakładania nowego konta.
 - Brak możliwości usunięcia zawodnika z bazy.
 - Błędy językowe:
     - literówka w kafelku z listą ostatnich aktywności,
     - mimo wybranego języka PL teksty pod niektórymi polami nadal wyświetlają się po angielsku np. teksty walidacyjne, przyciski akcji nie są tłumaczone, oryginalna nazwa aplikacji, niektóra pola do wypełnienia, 
     - możliwe błędy w tłumaczeniu strony na angielski, nieumiejętne zastosowanie dosłownego tłumaczenia zamiast poprawnej terminologii w danym języku

![25](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/6070b44d-552a-4d73-b0cc-3c09c99811fa) ![26](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/fcfb2723-2c7c-4ca6-8c63-6a69ab9252b4)

![24](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/2c8b4f9c-8a2c-4008-be6f-3dea58cf01bd) 

![27](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/b3628ef1-ffc2-44d9-be2b-986ccafda920)

 - Okno Logowania: pozycjonowanie przycisków/zmiana ich położenia po kliknięciu: przy błędnym wpisaniu hasła lub adresu email przycisk SIGN IN wchodzi na ramkę okna. 
 - Błędy w funkcjonalności *Dodaj gracza/Edytuj gracza* (powtarzalne w funkcjonalności *Dodaj mecz/Edytuj mecz*):
   - brak komunikatów walidacyjnych, aby poinformować użytkownika o konieczności wprowadzenia poprawnego formatu danych takich jak email, numer telefonu,
   - brak indykacji, że należy wprowadzić poprawną wartość liczbową,
   - brak ustanowionych minimalnych i maksymalnych wartości liczbowych odpowiednich dla poszczególnych pól, gdzie wymagane jest wpisanie wartości liczbowej,
   - możliwość wpisywania licz w pola tekstowe i na odwrót,
   - możliwość wpisywania minusowych wartości,
   - brak ustanowionych zakresów w opcji dodawania data (date picker), brak poprawnego formatowania dat,
   - brak możliwości wpisania tekstu w polu *Recenzja* (funkcja *Dodaj mecz*),
   - w zakładce *EDYCJA MECZU*, sekcja *Lista zdarzeń* jest niemożliwa do edytowania; brak informacji skąd można edytować dane,
   - przycisk *CLEAR* w *EDYCJI MECZU*, *EDYCJI GRACZA* są nieaktywne,
   - linki wklejone w polach, gdzie możliwe jest ich dodanie zapisywane są jako nieaktywne,
   - *EDYCJA MECZU* brak konkretnych komunikatów o błędzie i co go wywołało podczas zapisywania danych,
   - funkcja *+DODAJ RAPORT* z poziomu zakładki *RAPORTY* nie otwiera okna edycji raportu, zostajemy przekierowaniu do zakładki *MECZE* i dopiero z listy *Akcji* po prawej stronie wybieramy opcję *Dodaj Raport*,
   - niemożliwe jest stworzenie raportu bez aktualizacji danych gracza - **dodania informacji *Województwo* w profilu gracza** - pole nie jest zaznaczone jako obowiązkowe; użytkownik kolejny raz musi wejść w profil gracza, aby dodać potrzebną informację w celu wygenerowania raportu,
   - brak możliwości edycji *DANYCH STATYSTYCZNYCH* w wygenerowanym raporcie (w przeciwieństwie do pozostałych punktów raportu oraz pola z komentarzami po lewej).
     


































