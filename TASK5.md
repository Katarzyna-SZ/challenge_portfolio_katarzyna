# TASK 5 🗃️
    
### Spis treści:
1. [Subtask 1 - Krótki kurs podstaw SQL](#subtask1)
2. [Subtask 2 - Konfiguracja środowiska i wgranie bazy danych.](#subtask2)
3. [Subtask 3 - Kilka zadań na rozgrzewkę:](#subtask3)
    - [Zad. 1 Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.](#punkt1) 
    - [Zad. 2 Wyświetl film, który powstał w 2019 roku.](#punkt2)
    - [Zad. 3 Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.](#punkt3)
    - [Zad. 4 Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$.](#punkt4)
    - [Zad. 5 Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.](#punkt5)
    - [Zad. 6 Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.](#punkt6)
    - [Zad. 7 Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.](#punkt7)
    - [Zad. 8 Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.](#punkt8)
    - [Zad. 9 Wyświetl dane klienta, który nie ma podanego adresu email.](#punkt9)
    - [Zad. 10 Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.](#punkt10)
     
<hr>

### <a name='subtask1'>☑️ Subtask 1 - Krótki kurs podstaw SQL </a>

📌**Oprogramowanie użyte do wykonania ćwiczeń:** Microsoft SQL Server Management Studio

📌**Baza danych wykorzystana do wykonania ćwiczeń:** [AdventureWorks2014](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms)

👉 **Zad. 1** Wyświetl wszystkie produkty (tabela Production.Product) kolory czarnego, posortowane malejąco wg ceny (ListPrice).

```sql
SELECT * FROM Production.Product
WHERE Color = 'Black'
ORDER BY ListPrice DESC
```
👉 **Zad. 2** Wyświetl wszystkie produktu koloru czerwonego i niebieskiego, których nazwa zaczyna się na 'L', posortowane wg rozmiaru malejąco i ceny rosnąco.

```sql
SELECT * FROM Production.Product
WHERE Color IN ('Red', 'Blue') AND Name LIKE 'L%'
ORDER BY Size DESC, ListPrice ASC
```
👉 **Zad. 3** Wyświetl wiesze z tabeli Sales.SalesTerritory, przypisane do Europy, posortowane wg nazwy kraju.

```sql
SELECT * FROM Sales.SalesTerritory
WHERE [Group] = 'Europe'
ORDER BY Name
```
👉 **Zad. 4** Wyświetl wiersze z tabeli Sales.SalesTerritory, posortowane wg grupy regionów (kontynentów) i nazwy kraju rosnąco.

```sql
SELECT * FROM Sales.SalesTerritory
ORDER BY Name, [Group] DESC
```

👉 **Zad. 5** Wyświetl zamówienia przypisane do obszarów o identyfikatorach 7,8,9.

```sql
SELECT * FROM Sales.SalesOrderHeader
WHERE TerritoryID IN (7, 8, 9)
```

👉 **Zad. 6** Wyświetl 10 ostatnich zamówień, przypisanych do obszarów o identyfikatorach 7, 8, 9 o wartości (kolumna SubTotal) mniejszej niż 100, posortowane wg daty (OrderDate).

```sql
SELECT TOP 10 * FROM Sales.SalesOrderHeader
WHERE TerritoryID IN (7, 8, 9) AND SubTotal <100
ORDER BY OrderDate
```
👉 **Zad. 7** Wyświetl 10 zamówień na najwyższą kwotę, przypisanych do obszaru 7.

```sql
SELECT TOP 10 * FROM Sales.SalesOrderHeader
WHERE TerritoryID = 7
ORDER BY SubTotal DESC
```

👉 **Zad. 8** Wyświetl zamówienia przypisane do obszaru 7, bez przypisanego numeru karty kredytowej (kolumna CreditCardID).

```sql
SELECT * FROM Sales.SalesOrderHeader
WHERE TerritoryID = 7 AND CreditCardID IS NULL
```

👉 **Zad. 9** Wyświetl zamówienia przyposanych do obszaru 7, z przypisanym numerem karty kredytowej.

```sql
SELECT * FROM Sales.SalesOrderHeader
WHERE TerritoryID = 7 AND CreditCardID IS NOT NULL
```

👉 **Zad. 10** Wyświetl zamówienia z roku 2011, posortuj wg daty zamówienia.

```sql
SELECT * FROM Sales.SalesOrderHeader
WHERE OrderDate BETWEEN '20110101' AND '20111231'
ORDER BY OrderDate
```
### <a name='subtask2'>☑️ Subtask 2 - Konfiguracja środowiska i wgranie bazy danych. </a>

Instalacja pakietu XAMPP oraz pobranie bazy danych przygotowanej do ćwiczenia zapytań.

### <a name='subtask3'>☑️ Subtask 2 - Subtask 3 - Kilka zadań na rozgrzewkę: </a>

👉 <a name='punkt1'> **Zad. 1** Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.</a>

```sql
SELECT * FROM actors
ORDER BY surname ASC
```
![1](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/b95bb03c-f357-4263-a85a-411bc93f3874)

👉 <a name='punkt2'> **Zad. 2** Wyświetl film, który powstał w 2019 roku.</a>

```sql
SELECT * FROM movies
WHERE year_of_production = 2019
```
![2](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/e8a8e87d-c2b4-4786-be60-052c0027a280)

👉 <a name='punkt3'> **Zad. 3** Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.</a>

```sql
SELECT * FROM movies 
WHERE year_of_production BETWEEN 1900 AND 1999;
```
![3](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/14669eea-6f38-423f-bfbd-d49b996a25b7)

👉 <a name='punkt4'> **Zad. 4** Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$.</a>

```sql
SELECT title, price FROM movies 
WHERE price <7
```
![4](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/47bb2ca3-b8f4-4294-8a1a-6bc2ee76a9a9)

👉 <a name='punkt5'> **Zad. 5** Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.</a>

```sql
SELECT * FROM actors 
WHERE actor_id >=4 AND actor_id <= 7
```
![5](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/24143066-2bda-4037-8e04-5324adc7584b)

👉 <a name='punkt6'> **Zad. 6** Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.</a>

```sql
SELECT * FROM customers 
WHERE customer_id = 2 OR customer_id = 4 OR customer_id = 6
```
![6](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/0f2a7c4f-3e25-47c0-a8aa-0d21fb54f4eb)

👉 <a name='punkt7'> **Zad. 7** Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.</a>

```sql
SELECT * FROM customers 
WHERE customer_id IN (1, 3, 5)
```
![7](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/007c8fb4-ffa4-41b9-8fa6-d4986e4869b7)

👉 <a name='punkt8'> **Zad. 8** Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.</a>

```sql
SELECT * FROM actors 
WHERE name LIKE 'An%'
```
![8](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/086d3048-4ae4-4d6a-bea2-28bcda5a8593)

👉 <a name='punkt9'> **Zad. 9** Wyświetl dane klienta, który nie ma podanego adresu email.</a>

```sql
SELECT * FROM customers 
WHERE email IS NULL
```
![9](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/f9d2cfd7-0a00-4f54-8d0d-641fe30411a4)

👉 <a name='punkt10'> **Zad. 10** Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.</a>

```sql
SELECT * FROM movies 
WHERE price >9 AND (movie_id BETWEEN 2 AND 8)
```
![10](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/63ecaefd-0389-4130-9241-e5303af8d59d)
