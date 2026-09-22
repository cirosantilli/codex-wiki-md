<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For each $t\in[0,1]$, evaluation $\delta_t:f\mapsto f(t)$ is a [bounded linear functional](../../../../../../../continuous-linear-functional.md) of [norm](../../../../../../../norm.md) one. Thus [weak convergence](../../../../../../../weak-convergence.md) to zero gives $f_n(t)\to0$ at every $t$. The set $\{f_n:n\ge1\}$ is a [weakly bounded set](../../../../../../../weakly-bounded-set.md), since every scalar sequence $\ell(f_n)$ converges, and part (a) supplies a uniform bound $\|f_n\|_\infty\le M$.

The constant $M$ is integrable for [Lebesgue measure](../../../../../../../lebesgue-measure.md) on $[0,1]$. Applying the [dominated convergence theorem](../../../../../../../dominated-convergence-theorem.md) to $|f_n|$ gives the [weakly null continuous functions converge in L1](../../../../../../../weakly-null-continuous-functions-converge-in-l1.md) conclusion

$$
\boxed{\|f_n\|_{L^1[0,1]}=\int_0^1|f_n(t)|\,dt\longrightarrow0.}
$$

Pointwise convergence alone would not provide the needed uniform dominating function; it is the weak boundedness argument that supplies it.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 106](../../../../paper-106-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
