Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.

film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?



--CEVAPLAR-
--1.SORU--
SELECT DISTINCT replacement_cost FROM film;


--2. SORU--
SELECT COUNT (DISTINCT replacement_cost) FROM film;


--3.SORU--
SELECT COUNT (*) FROM film 
WHERE title LIKE 'T%' AND rating = 'G';


--4.SORU--
SELECT COUNT (*) FROM country
WHERE country LIKE '-----';


--5.SORU--
SELECT COUNT (*) FROM city
WHERE city ILIKE '%R';
