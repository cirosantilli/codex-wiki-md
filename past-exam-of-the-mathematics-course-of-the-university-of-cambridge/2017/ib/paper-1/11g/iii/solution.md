<h1 id="11g/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**True.** Define $c_n(x)=\max(-n,\min(x,n))$ and $f_n=f\circ c_n$. The map $c_n$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md) with constant one. The restriction of $f$ to $[-n,n]$ is [uniformly continuous](../../../../../../uniform-continuity.md) by the [Heine-Cantor theorem](../../../../../../heine-cantor-theorem.md); its modulus of continuity combined with $|c_n(x)-c_n(y)|\le|x-y|$ proves [uniform continuity](../../../../../../uniform-continuity.md) of $f_n$ on all of $\mathbb R$. For each fixed $x$, once $n\ge|x|$ we have $f_n(x)=f(x)$. Hence

$$
\boxed{f_n\longrightarrow f\text{ pointwise on }\mathbb R}.
$$

This [pointwise approximation by uniformly continuous functions](../../../../../../pointwise-approximation-by-uniformly-continuous-functions.md) even gives eventual equality on every fixed bounded interval. It need not give [uniform convergence](../../../../../../uniform-convergence.md) on the whole line, as the bounded counterexample in part (i) already demonstrates.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [11G](../../11g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
