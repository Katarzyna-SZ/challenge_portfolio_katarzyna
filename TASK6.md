# TASK 6 🏁

### ☑️ Subtask 1 - kontyunacja zapytań SQL (level wyżej).

📌**Pakiet Xampp**

📌Narzędzie wykorzystane do zarządzania bazą danych: **phpMyAdmin** 

👉 **Zad. 11 Popraw bląd w nazwisku jednego z klientów. Zamień Muler na Miler. Znajdź i zastosuje funkcję, która poprawi błąd.**

```sql
UPDATE customers
SET surname = 'Miler'
WHERE customer_id = 3
```
![1](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/a73c2e27-f091-4948-b12a-0aa9983c4515)

👉 **Zad. 12 Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila. W celu napisania mu wiadomości o pomyłce fantastycznej szefowej.**

```sql
SELECT * FROM customers
JOIN sale ON customers.customer_id = sale.customer_id
WHERE movie_id = 4
```
![2](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/9519f93e-5d31-45e9-bad4-81d34c46876b)

👉 **Zad. 13 Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: pati@mail.com**

```sql
UPDATE customers
SET email = 'pati@gmail.com'
WHERE customer_id = 4
```
![3](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/991671ac-2bf0-4935-9447-cacfb77aecc7)

👉 **Zad. 14 Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).**

```sql
SELECT customers.name, customers.surname, sale.sale_date, movies.title 
FROM ((customers 
INNER JOIN sale ON customers.customer_id = sale.customer_id) 
INNER JOIN movies ON sale.movie_id = movies.movie_id)
ORDER BY sale_date DESC
```
![4](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/4bd3dc72-193c-4010-93bb-179478697670)

👉 **Zad. 15 W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag**

Dodanie kolumny | Wypełnienie kolumny 
--- | --- 
```ALTER TABLE customers ADD pseudonym varchar (3)``` | ```UPDATE customers SET pseudonym = CONCAT(SUBSTRING(name, 1, 2), RIGHT(surname, 1))```
![5a](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/f5dd7716-beea-4427-b5ad-76b4d202b5d8) | ![5](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/23372472-5d03-414a-a828-bfbb477e0e41)

👉 **Zad. 16 Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.**

```sql
SELECT DISTINCT title FROM movies 
JOIN sale ON movies.movie_id = sale.movie_id
```
![6](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/e15298f5-b3e2-412f-a61f-62c8b6d3e61f)

👉 **Zad. 17 Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie. (Wykorzystaj do tego funkcji UNION).**

```sql
SELECT name FROM actors 
UNION 
SELECT name FROM customers ORDER BY name ASC
```
![7](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/62b9c519-8a62-4c21-931b-21501727d08a)

👉 **Zad. 17 Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie).**

```sql
UPDATE movies SET price = CONCAT(price + 2.5) WHERE year_of_production > 2000
```
Cena wypożyczenia filmów przed podwyżką | Cena wypożyczenia filmów po podwyżce
--- | --- 
![8a](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/08c723f6-f029-4652-964d-89f7ddfdebd0) | ![8B](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/9b8a18ca-c94c-4368-9bee-13c288bafb37)
