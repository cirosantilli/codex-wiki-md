<h1 id="16h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a set $x$ and define by recursion on $\omega$

$$
T_0=x,
\qquad
T_{n+1}=\bigcup T_n.
$$

The recursion theorem defines a function-class $F$ uniquely by $F(n)=T_n$: for each $n\in\omega$ there is exactly one finite sequence satisfying the displayed recursion through stage $n$. Thus $F$ is genuinely functional, and the [Axiom schema of replacement](../../../../../../axiom-schema-of-replacement.md) applied to the set $\omega$ gives the set $\{T_n:n\in\omega\}$.

Now define

$$
T=\bigcup_{n\in\omega}T_n.
$$

It contains every member of $x$. If $y\in T$, then $y\in T_n$ for some $n$; hence every $z\in y$ belongs to

$$
\bigcup T_n=T_{n+1}\subseteq T.
$$

Thus $T$ is transitive. If $U$ is any transitive set containing every member of $x$, induction gives $T_n\subseteq U$ for every $n$, so $T\subseteq U$. Therefore

$$
\boxed{T=\operatorname{TC}(x)}
$$

is the [transitive closure](../../../../../../transitive-closure.md) of $x$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16H](../../16h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
