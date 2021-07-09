

## Ödev 12

**film** tablosunda film uzunluğu **length** sütununda gösterilmektedir. Uzunluğu ortalama film uzunluğundan fazla kaç tane film vardır?

```sql
SELECT COUNT(*) FROM film
WHERE length > (SELECT AVG(length) FROM film);
```

**film** tablosunda en yüksek rental_rate değerine sahip kaç tane film vardır?

```sql
SELECT COUNT(*) FROM film
WHERE rental_rate = (SELECT MAX(rental_rate) FROM film);
```

**film** tablosunda en düşük rental_rate ve en düşün replacement_cost değerlerine sahip filmleri sıralayınız.

```sql
SELECT title,rental_rate,replacement_cost FROM film
WHERE (rental_rate = (SELECT MIN(rental_rate) FROM film)) AND (replacement_cost = (SELECT MIN(replacement_cost) FROM film));

```

**payment** tablosunda en fazla sayıda alışveriş yapan müşterileri(customer) sıralayınız.

```sql
SELECT customer_id, COUNT(customer_id) AS sayi from payment
GROUP BY customer_id
ORDER BY sayi desc;
```

