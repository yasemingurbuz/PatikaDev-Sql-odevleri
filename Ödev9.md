

## Ödev 9

**city** tablosu ile **country** tablosunda bulunan şehir (city) ve ülke (country) isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

```sql
 SELECT city,country FROM city
JOIN country ON city.country_id = country.country_id
```

**customer** tablosu ile **payment** tablosunda bulunan payment_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

```sql
SELECT payment_id,first_name,last_name FROM customer
JOIN payment ON customer.customer_id = payment.customer_id

```

**customer** tablosu ile **rental** tablosunda bulunan rental_id ile customer tablosundaki first_name ve last_name isimlerini birlikte görebileceğimiz INNER JOIN sorgusunu yazınız.

```sql
SELECT rental_id,first_name,last_name FROM customer
JOIN rental ON customer.customer_id = rental.customer_id

```

