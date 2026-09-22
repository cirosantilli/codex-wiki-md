<h1 id="b3/solution">Solution</h1>

↑ **Parent:** [B3](../b3.md)

For noninteracting particles, a many-particle configuration has $E=\sum_jn_j\epsilon_j$ and $N=\sum_jn_j$. Summing independently over allowed occupations therefore factorizes the grand [partition function](../../../../canonical-partition-function.md):

$$
\Theta=\prod_j\Theta_j,\qquad
\boxed{\Phi=-k_BT\sum_j\ln\Theta_j.}
$$

At fixed $T,V$, differentiating the original state sum gives $\partial_\mu\ln\Theta=\beta\langle N\rangle$ and $\partial_\mu^2\ln\Theta=\beta^2\operatorname{Var}N$, so

$$
\boxed{\langle N\rangle=-\partial_\mu\Phi,\qquad
\operatorname{Var}N=-k_BT\partial_\mu^2\Phi
=k_BT\partial_\mu\langle N\rangle.}
$$

For one level, write $q=e^{-\beta(\epsilon-\mu)}$. [Fermions](../../../../fermion.md) allow $n=0,1$, giving $\Theta_F=1+q$ and $\bar n=q/(1+q)$. [Bosons](../../../../boson.md) allow all nonnegative integers, giving $\Theta_B=1/(1-q)$ and $\bar n=q/(1-q)$, with $q<1$. Thus

$$
\boxed{\bar n_F=\frac1{e^{\beta(\epsilon-\mu)}+1},\qquad
\bar n_B=\frac1{e^{\beta(\epsilon-\mu)}-1}.}
$$

The [grand-canonical single-level occupation variance](../../../../grand-canonical-single-level-occupation-variance.md) follows from the same derivative identity applied to one level:

$$
\boxed{\operatorname{Var}n=k_BT\partial_\mu\bar n
=\begin{cases}\bar n(1-\bar n),&\text{fermions},\\
\bar n(1+\bar n),&\text{bosons}.\end{cases}}
$$

In the high-temperature nondegenerate regime, $\bar n\ll1$ and both approach classical Poisson-like fluctuations, $\operatorname{Var}n\simeq\bar n$. At low [temperature](../../../../temperature-split.md), nearly filled or empty [fermion](../../../../fermion.md) levels have strongly suppressed fluctuations; only the Fermi-surface window changes occupation. Highly occupied low-energy [boson](../../../../boson.md) levels can instead have $\operatorname{Var}n\sim\bar n^2$, showing bosonic enhancement. This last statement depends on occupation and reservoir [chemical potential](../../../../chemical-potential-split.md), not [temperature](../../../../temperature-split.md) alone; grand-canonical condensate fluctuations must not be confused with a fixed-total-number ensemble.

## ↑ Ancestors (12)

1. [B3](../b3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2014](../../split.md)
4. [Past exam of the physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
