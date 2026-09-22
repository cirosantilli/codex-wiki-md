# Consistent heuristic

↑ **Parent:** [Search problem](search-problem.md)

A [heuristic function](heuristic-function.md) is consistent if $h(g)=0$ at every goal and

$$
h(s)\le c(s,a,s')+h(s')
$$

for every permitted transition $s\xrightarrow{a}s'$ with step cost $c(s,a,s')$. Summing these inequalities along a finite route to a goal gives $h(s)\le$ its total cost. Taking the minimum over such routes proves that every [consistent heuristic](consistent-heuristic.md) is an [admissible heuristic](admissible-heuristic.md).

## ↑ Ancestors (6)

1. [Search problem](search-problem.md)
2. [Computational problem](computational-problem.md)
3. [Computational complexity theory](computational-complexity-theory.md)
4. [Theoretical computer science](theoretical-computer-science-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (16)

- [A-star search](a-star-search.md)
- [Admissible heuristic combination](admissible-heuristic-combination.md)
- [Consistent heuristic](consistent-heuristic.md)
- [Heuristic function](heuristic-function.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/1/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/a/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/1/d/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/1/b/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/c/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/1/f/solution.md)
- [Perfect heuristic](perfect-heuristic.md)
- [Relaxation heuristic](relaxation-heuristic.md)
- [Simultaneous rendezvous distance](simultaneous-rendezvous-distance.md)
- [Word ladder](word-ladder.md)
