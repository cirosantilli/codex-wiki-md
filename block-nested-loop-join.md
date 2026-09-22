# Block nested-loop join

↑ **Parent:** [Database query plan](database-query-plan.md)

A [relational join](relational-join.md) implementation that retains a block of outer records in memory while scanning the inner input. With $b$ outer pages per block, $p$ outer pages and $q$ inner pages, its data-read cost is $p+\lceil p/b\rceil q$, before temporary output costs.

## ↑ Ancestors (5)

1. [Database query plan](database-query-plan.md)
2. [Database query](database-query.md)
3. [Database](database.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/databases/2/b/solution.md)
