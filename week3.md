# Week 3 Exercises 2

## Question 1
```sql
select * from goal;
```
![Ex2Q1.png](pictures/Ex2Q1.png)

## Question 2
```sql
select name, type from airport where iso_country = "FI";
```
![Ex2Q2.png](pictures/Ex2Q2.png)

## Question 3
```sql
select name from airport where iso_country = "FI" order by name asc;
```
![Ex2Q3.png](pictures/Ex2Q3.png)

## Question 4
```sql
select name, type from airport where iso_country = "FI" order by type asc, name asc;
```
![Ex2Q4.png](pictures/Ex2Q4.png)

## Question 5
```sql
select name from country where name like "F%";
```
![Ex2Q5.png](pictures/Ex2Q5.png)

## Question 6
```sql
select name from country where name like "%f%" or "%F%" or "F%";
```
![Ex2Q6.png](pictures/Ex2Q6.png)

## Question 7
```sql
select location from game where screen_name = "Vesa";
```
![Ex2Q7.png](pictures/Ex2Q7.png)

## Question 8 
```sql
select game.co2_consumed from game where screen_name = "Ilkka";
```
![Ex2Q8.png](pictures/Ex2Q8.png)

## Question 9 
```sql
select distinct game.co2_budget from game;
```
![Ex2Q9.png](pictures/Ex2Q9.png)

## Question 10
```sql
select screen_name, co2_budget, co2_consumed, (co2_budget - co2_consumed) as co2_left 
from game 
where screen_name = "Ilkka";
```
![Ex2Q10..png](pictures/Ex2Q10.png)