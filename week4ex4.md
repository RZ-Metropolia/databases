# Week 4 Exercises 4

## Question 1 
```sql
select country.name as 'country name', airport.name as 'airport name'
from airport
inner join country
on airport.iso_country = country.iso_country
where airport.scheduled_service = 'yes' and
country.name = 'Finland';
```
![EX4Q1.png](pictures/EX4Q1.png)

## Question 2 
```sql
select game.screen_name, airport.name
from game
inner join airport
on game.location = airport.ident;
```
![EX4Q2.png](pictures/EX4Q2.png)

## Question 3 
```sql
select game.screen_name, country.name
from game
inner join airport
on game.location = airport.ident
inner join country
on airport.iso_country = country.iso_country;
```
![EX4Q3.png](pictures/EX4Q3.png)

## Question 4 
```sql
select airport.name, game.screen_name
from airport
left join game
on airport.ident = game.location
where airport.name like "%Hels%";
```
![EX4Q4.png](pictures/EX4Q4.png)

## Question 5
```sql
select goal.name, game.screen_name
from goal
left join goal_reached
on goal.id = goal_reached.goal_id
left join game
on goal_reached.game_id = game.id;
```
![EX4Q5.png](pictures/EX4Q5.png)