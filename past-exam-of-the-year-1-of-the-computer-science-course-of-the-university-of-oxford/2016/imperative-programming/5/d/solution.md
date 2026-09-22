<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a node tuple $u$, write $c(u)$ for its identifier. A [predicate](../../../../../predicate.md) that is true exactly when identifiers repeat is

$$
\boxed{\exists u,v\in T.\quad u\ne v\ \land\ c(u)=c(v).}
$$

The inequality excludes choosing the same tuple twice. The [set](../../../../../set-split.md) $T$ cannot contain two copies of an identical quadruple, but it can contain distinct quadruples with equal first component and different information or successors. The negation is the usual identifier-uniqueness [representation invariant](../../../../../representation-invariant.md), namely $\forall u,v\in T,\ c(u)=c(v)\Rightarrow u=v$.

## ↑ Ancestors (12)

1. [D](../d.md)
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
