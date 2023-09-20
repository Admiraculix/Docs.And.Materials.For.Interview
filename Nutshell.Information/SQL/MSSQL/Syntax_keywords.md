JOIN		Joins tables
LEFT JOIN	Returns all rows from the left table, and the matching rows from the right table.
                Връща всички редове от лявата таблица и съответстващите редове от дясната таблицa.

OUTER JOIN	Returns all rows when there is a match in either left table or right table.
		Връща всички редове, когато има съвпадение в лявата или дясната таблица

RIGHT JOIN	Returns all rows from the right table, and the matching rows from the left table.
		Връща всички редове от дясната таблица и съответстващите редове от лявата таблица.
FULL OUTER JOIN	Returns all rows when there is a match in either left table or right table
		Връща всички редове, когато има съвпадение в лявата или дясната таблица

INNER JOIN	Returns rows that have matching values in both tables
		Връща редове, които имат съвпадащи стойности и в двете таблици

UNION		Combines the result set of two or more SELECT statements (only distinct values)
UNION ALL	Combines the result set of two or more SELECT statements (allows duplicate values)

CHECK		A constraint that limits the value that can be placed in a column

HAVING		Used instead of WHERE with aggregate functions ( into GROUP BY keyword)
aggregate function (Count() Sum() Avg() Min() Max())

MATCH  		??
-> https://neo4j.com/docs/cypher-manual/current/clauses/match/
