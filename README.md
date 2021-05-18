# sqlChallenge

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
