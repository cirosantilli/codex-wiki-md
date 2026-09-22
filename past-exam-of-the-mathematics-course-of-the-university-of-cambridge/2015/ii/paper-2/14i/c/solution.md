<h1 id="14i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [binomial upper bound for a Ramsey number](../../../../../../binomial-upper-bound-for-a-ramsey-number.md) gives $R(3,t)\leq\binom{t+1}{2}=O(t^2)$. For the [triangle-free Ramsey lower bound by alteration](../../../../../../triangle-free-ramsey-lower-bound-by-alteration.md), a [binomial random graph](../../../../../../binomial-random-graph.md) $G(n,p)$ has expected triangle count $\binom n3p^3$ and expected independent $t$-set count $\binom nt(1-p)^{\binom t2}$. Choose a realization whose sum of these counts is at most its expectation. Delete one vertex from each surviving forbidden set, iterating through the originally listed sets. The remaining [graph](../../../../../../graph-split.md) has neither a triangle nor an independent $t$-set. This [random alteration method](../../../../../../random-alteration-method.md) proves

$$
R(3,t)>n-\binom n3p^3-\binom nt(1-p)^{\binom t2}.
$$

For large $t$, set $n=\lfloor(t/(4\log t))^{3/2}\rfloor$ and $p=n^{-2/3}$. The triangle term is at most $n/6$. Using $\binom nt\leq(en/t)^t$ and $1-p\leq e^{-p}$, the logarithm of the independent-set term divided by $t$ is at most

$$
\log(en/t)-\frac{p(t-1)}2\leq\frac12\log t-\frac32\log\log t+O(1)-2\log t+o(1),
$$

which tends to $-\infty$. That term is eventually below $1$. Thus $R(3,t)>5n/6-1$ and

$$
\boxed{R(3,t)=\Omega\!\left((t/\log t)^{3/2}\right).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14I](../../14i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
