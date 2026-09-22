<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Read $\operatorname{prop}_3(u,v)$ as the existence of a directed successor [path](../../../../../continuous-path.md) from $u$ to $v$. Then the property says **every reachable ordered pair of even-valued nodes admits a connecting route through an odd-valued node**. More exactly, for all even-valued $u,v$ with $u$ reaching $v$, there is an odd-valued $w$ such that $u$ reaches $w$ and $w$ reaches $v$.

The two reachability witnesses concatenate to a [directed walk](../../../../../directed-walk.md) through $w$. In an [acyclic graph](../../../../../forest.md) this yields an intervening node on a [path](../../../../../continuous-path.md). In a graph with [directed cycles](../../../../../directed-cycle.md), the concatenation may revisit vertices. The existential witness does not say that every connecting path contains an odd-valued node, or even that an even-to-even edge is forbidden. For example edges $u\to v$, $u\to w$, $w\to v$, with even endpoints and odd $w$, satisfy the property for this pair despite the direct even-to-even edge.

There are two source-notation qualifications. The displayed outer universal quantifier binds both symbols appearing as formal arguments to `prop`, so the whole formula is a global property of $T$, rather than a genuinely free two-node predicate. Also the indexed ellipsis defining `prop3` does not formalize path length zero. With positive-length reachability, even nodes on a cycle impose additional requirements; with reflexive reachability, choosing $u=v$ also imposes a requirement, and an isolated even-valued node would fail. The usual intended reading here is positive-length successor reachability. No uniqueness, acyclicity or specific path-length convention is proved by the displayed formula alone.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
