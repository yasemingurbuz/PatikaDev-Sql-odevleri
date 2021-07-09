

## Ödev 5

**film** tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en uzun (length) 5 filmi sıralayınız.

```sql
SELECT title FROM film WHERE title LIKE '%n' LIMIT 5;
```

**film** tablosunda bulunan ve film ismi (title) 'n' karakteri ile biten en kısa (length) ikinci 5 filmi sıralayınız.

```sql
SELECT title FROM film WHERE title LIKE '%n' OFFSET 5 LIMIT 5;
```

**country** tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?

```sql
SELECT last_name FROM customer WHERE store_id = 1 ORDER BY last_name DESC LIMIT 4;
```

