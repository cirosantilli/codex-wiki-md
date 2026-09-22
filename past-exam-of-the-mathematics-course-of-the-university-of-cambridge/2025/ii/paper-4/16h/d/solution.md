<h1 id="16h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Consider the structure $(M,\in)$.

For extensionality, let $x,y\in M$ have the same members in $M$. Since $M$ is transitive, every actual member of $x$ or $y$ lies in $M$. Thus $x$ and $y$ have the same members in $V$, and ambient extensionality gives $x=y$.

By hypothesis $\varnothing\in M$, and it has no members in the induced structure, so the empty-set axiom holds. If $x,y\in M$, then $\{x,y\}\in M$ by closure, and its internal members are exactly $x$ and $y$, proving pairing.

Finally, if $x\in M$, then $\bigcup x\in M$. For $z\in M$,

$$
z\in\bigcup x
\quad\Longleftrightarrow\quad
\exists y\in x\ (z\in y).
$$

Every such $y$ lies in $M$ by transitivity, so the same equivalence holds internally. Hence union is satisfied. This is the [basic set-theoretic axioms inherited by a transitive class](../../../../../../basic-set-theoretic-axioms-inherited-by-a-transitive-class.md) argument.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [16H](../../16h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
