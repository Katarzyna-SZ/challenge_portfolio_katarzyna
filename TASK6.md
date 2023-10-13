# TASK 6 🏁

### ☑️ Subtask 1 - kontunacja zapytań SQL (level wyżej).

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

👉 **Zad. 14. Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).**

```sql
SELECT customers.name, customers.surname, sale.sale_date, movies.title 
FROM ((customers 
INNER JOIN sale ON customers.customer_id = sale.customer_id) 
INNER JOIN movies ON sale.movie_id = movies.movie_id)
ORDER BY sale_date DESC
```
![4](https://github.com/Katarzyna-SZ/challenge_portfolio_katarzyna/assets/140599598/4bd3dc72-193c-4010-93bb-179478697670)
