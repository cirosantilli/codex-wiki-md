<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We use the standard characteristic-$p$ absolute Galois-group theorem, $\operatorname{cd}_p(K)\le1$, and the cohomological identification $\operatorname{Br}(K)=H^2(K,K_s^\times)$. Both are clearly stated inputs permitted for this question.

In characteristic $p$, the map $a\mapsto a^p$ on $K_s^\times$ is injective, although it need not be surjective: $p$th roots are purely inseparable. Thus it gives an exact sequence of discrete [Galois modules](../../../../../../galois-module.md)

$$
1\longrightarrow K_s^\times\xrightarrow{\ p\ }K_s^\times
\longrightarrow Q\longrightarrow1,\qquad Q=K_s^\times/(K_s^\times)^p.
$$

The quotient $Q$ is killed by $p$. Since $\operatorname{cd}_p(K)\le1$, $H^2(K,Q)=0$. The long exact cohomology sequence contains

$$
\operatorname{Br}(K)\xrightarrow{\ p\ }\operatorname{Br}(K)\longrightarrow H^2(K,Q)=0.
$$

Therefore **multiplication by $p$ on $\operatorname{Br}(K)$ is surjective**. This is [Brauer p-divisibility in characteristic p](../../../../../../brauer-p-divisibility-in-characteristic-p.md). The quotient-module sequence is the relevant one in characteristic $p$; the separable Kummer sequence with a nontrivial $\mu_p$ is not available there.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
