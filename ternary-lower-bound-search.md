# Ternary lower-bound search

↑ **Parent:** [Search algorithm](search-algorithm.md)

A [lower-bound search](lower-bound-search.md) that probes two positions to retain one of three subintervals. For unresolved $[lo,hi)$ of positive length $d$, put $q=\lfloor d/3\rfloor$, $m_1=lo+q$ and $m_2=hi-1-q$. If $a(m_1)\geq x$, retain $[lo,m_1)$; if $a(m_2)<x$, retain $[m_2+1,hi)$; otherwise retain $[m_1+1,m_2)$. [Sortedness](sortedness.md) preserves the lower-bound partition. The new interval lengths are $q,q,d-2q-2$, and the feasible middle case has nonnegative length at most $q$. This proves strict progress and $O(\log(N+1))$ comparison cost. Equality must retain the first possible boundary rather than return an arbitrary matching occurrence.

## ↑ Ancestors (4)

1. [Search algorithm](search-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2023/imperative-programming/1/c/solution.md)
