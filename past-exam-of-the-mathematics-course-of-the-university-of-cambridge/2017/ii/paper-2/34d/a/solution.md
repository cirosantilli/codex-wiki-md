<h1 id="34d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here $p(n)$ is the [probability](../../../../../../probability.md) of microstate $n$, including all occupation data. In the [grand canonical ensemble](../../../../../../grand-canonical-ensemble.md), with energy $E_n$, particle number $N_n$, [chemical potential](../../../../../../chemical-potential.md) $\mu$ and $T>0$,

$$
p(n)=\mathcal Z^{-1}e^{-(E_n-\mu N_n)/(kT)},\qquad
\mathcal Z=\sum_ne^{-(E_n-\mu N_n)/(kT)}.
$$

Substitution in the [Gibbs entropy](../../../../../../gibbs-entropy.md) gives $S=k\log\mathcal Z+(U-\mu N)/T$, where $U=\langle E\rangle$ and $N=\langle N_n\rangle$. Differentiating at fixed $\mu,V$ gives $\partial_T\log\mathcal Z=(U-\mu N)/(kT^2)$. Therefore

$$
\boxed{S=k\left[\frac{\partial}{\partial T}(T\log\mathcal Z)\right]_{\mu,V}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [34D](../../34d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
