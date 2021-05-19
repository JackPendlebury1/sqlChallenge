# sqlChallenge

## world

1) select count(*) from city where CountryCode='USA';
2) select LifeExpectancy, Population from country where Name='Argentina';
3) select * from country where lifeExpectancy is not null order by lifeExpectancy desc limit 5;
4) select country.*, city.* from city join country on city.ID=country.Capital where country.Name='Spain';
5) select countrylanguage.*, country.Name from countrylanguage join country on countrylanguage.CountryCode=country.Code where region="Southeast Asia";
6) select * from city where Name like 'F%' limit 25;
7) select country.name, COUNT(city.Name) from city join country on country.Code=city.CountryCode where country.Name='China';
8) select * from country where Population > 0 order by Population asc limit 20;
9) select COUNT(*) from country;
10) select * from country order by SurfaceArea desc limit 10;
11) select country.name, city.* from city join country on country.Code=city.CountryCode where country.Name='Japan' order by country.Population desc limit 5;

## sakila
1) select * from actor;
2) select last_name from actor where first_name='John';
3) select * from actor where last_name='Neeson';
4) select * from actor where (actor_id % 10)=0;
5) select description  from film where film_id=100;
6) select * from film where rating='R';
7) select * from film where rating!='R';
8) select * from film order by length asc limit 10;
9) select max(length) from film;
10) select * from film where special_features='Deleted Scenes';
11) select last_name from actor group by last_name having count(last_name) = 1 order by last_name desc;
12) select count(last_name) from actor group by last_name having count(last_name) > 1 order by count(last_name) desc;
13) select count(actor.actor_id),actor.first_name, film_actor.actor_id from film_actor join actor on actor.actor_id=film_actor.actor_id group by film_actor.actor_id order by count(actor.actor_id) desc limit 1;
14) 
15) select avg(length) from film;
16) 
17) select count(film_id) from film where description like '%robot%'
18) select count(film_id) from film where release_year=2010;
19) select category.category_id, category.name, film_category.film_id, film.film_id, film.length, film.title from film join film_category on film_category.film_id=film.film_id join category on category.category_id=film_category.category_id where category.name='Horror'
20) select * from staff_list where ID=2;
21) 
22) select count(distinct country_id) from country;
23) select * from language order by name desc
24) select * from actor where last_name like '%son' order by first_name;
25)
