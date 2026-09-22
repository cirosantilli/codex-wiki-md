<h1 id="4/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

We prove convergence of the actual sequential updates above, not just concentration of ideal equilibrium distributions. Write $M_m=\mathbb E v_m$ and $N_m=\mathbb E v_m^2$. Given $v_{m-1}$, the centered normal draw satisfies

$$
\mathbb E[(\mu_m-\bar x)^2\mid v_{m-1}]=\frac{T_m v_{m-1}}n,\qquad
\mathbb E[(\mu_m-\bar x)^4\mid v_{m-1}]=3\left(\frac{T_m v_{m-1}}n\right)^2.
$$

The conditional [inverse-gamma distribution](../../../../../../../inverse-gamma-distribution.md) moments therefore give

$$
M_m=\frac{S+T_mM_{m-1}}{n-4T_m},\qquad
N_m=\frac{S^2+2ST_mM_{m-1}+3T_m^2N_{m-1}}{(n-4T_m)(n-6T_m)}.
$$

For $T_m\leq n/10$, the coefficient multiplying $M_{m-1}$ is at most $1/6$, so $M_m$ stays bounded by a geometric-recursion argument. The coefficient multiplying $N_{m-1}$ is at most $1/8$, and the other terms are bounded using the first-moment bound, so $N_m$ also stays bounded. These bounds start from the finite deterministic $v_0$.

Since $T_m\to0$, the boundedness makes every term containing $T_mM_{m-1}$ or $T_m^2N_{m-1}$ vanish. Hence $M_m\to S/n$ and $N_m\to S^2/n^2$. Consequently

$$
\mathbb E\left(v_m-\frac Sn\right)^2\to0,\qquad
\mathbb E(\mu_m-\bar x)^2=\frac{T_mM_{m-1}}n\to0.
$$

Thus

$$
\boxed{(\mu_m,v_m)\longrightarrow(\bar x,S/n)\quad\text{in mean square and therefore in probability}.}
$$

This establishes [mean-square convergence](../../../../../../../convergence-in-l2.md) for the specified Gaussian annealer. It does not assert that every implementation or cooling rule for every objective has the same guarantee, nor that mean-square convergence alone is almost-sure convergence.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 40](../../../../paper-40-split.md)
5. [Iii](../../../../split.md)
6. [2002](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
