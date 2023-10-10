# TASK 5 🗃️
    
### Spis treści:
1. [Subtask 1 - Krótki kurs podstaw SQL](#subtask1)
2. Subtask 2 - Konfiguracja środowiska i wgranie bazy danych.
3. [Subtask 3 - Kilka zadań na rozgrzewkę:](#subtask3)
    - [Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.](#punkt1) 
    - [Wyświetl film, który powstał w 2019 roku.](#punkt2)
    - [Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.](#punkt3)
    - [Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$.](#punkt4)
    - [Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.](#punkt5)
    - [Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.](#punkt6)
    - [Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.](#punkt7)
    - [Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.](#punkt8)
    - [Wyświetl dane klienta, który nie ma podanego adresu email.](#punkt9)
    - [Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.](#punkt10)
     
<hr>

### <a name='subtask1'>☑️ Subtask 1 - Krótki kurs podstaw SQL </a>

📌**Oprogramowanie użyte do wykonania ćwiczeń:** Microsoft SQL Server Management Studio

📌**Baza danych wykorzystana do wykonania ćwiczeń:** [AdventureWorks2014](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms)

👉 Zad. 1 Wyświetl wszystkie produkty (tabela Production.Product) kolory czarnego, posortowane malejąco wg ceny (ListPrice).

**SELECT * FROM Production.Product
WHERE Color = 'Black'
ORDER BY ListPrice DESC**

![1](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/8613df7f-599f-458d-923a-b837e54d3f45)

👉 Zad 2. Wyświetl wszystkie produktu koloru czerwonego i niebieskiego, których nazwa zaczyna się na 'L', posortowane wg rozmiaru malejąco i ceny rosnąco.

**SELECT * FROM Production.Product
WHERE Color IN ('Red', 'Blue') AND Name LIKE 'L%'
ORDER BY Size DESC, ListPrice ASC**



