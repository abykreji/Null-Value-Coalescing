## Exercise


> Question: 
##### Assuming a students minimum age for the class is 15, what is the average age of a student?


```python
SELECT avg(coalesce(age, 15)) FROM "Student";
```



> Question: 
##### Replace all empty first or last names with a default?

```python
SELECT id, coalesce(name, 'fallback'), coalesce(lastName, 'lastName'), age FROM "Student";
```