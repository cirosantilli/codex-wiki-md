<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use negative-exponential spatial [Fourier transforms](../../../../../../fourier-transform.md) and [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md):

$$
\begin{aligned}
Q_0(k)&=\int_0^Le^{-ikx}q_0(x)dx,&Q(k,t)&=\int_0^Le^{-ikx}q(x,t)dx,\\
F_j(k,t)&=\int_0^te^{\omega(k)s}\partial_x^jq(0,s)ds,&G_j(k,t)&=\int_0^te^{\omega(k)s}\partial_x^jq(L,s)ds\quad(j=0,1,2).
\end{aligned}
$$

Write $\mathcal F=k^2F_0-ikF_1-F_2$ and $\mathcal G=k^2G_0-ikG_1-G_2$. Integrate the [local relation](../../../../../../local-relation.md) first over $0<x<L$ and then over time. The left and right endpoint fluxes have opposite signs, giving the [finite-interval Airy global relation](../../../../../../finite-interval-airy-global-relation.md)

$$
\boxed{Q_0(k)-e^{\omega(k)t}Q(k,t)=\mathcal F(k,t)-e^{-ikL}\mathcal G(k,t).}
$$

All these spatial and temporal [integral transforms](../../../../../../integral-transform.md) are [entire functions](../../../../../../entire-function.md) of $k$ for sufficiently smooth data on the finite intervals. Put $\alpha=e^{2\pi i/3}$ and $k_j=\alpha^jk$, $j=0,1,2$. The [dispersion relation](../../../../../../dispersion-relation.md) obeys $\omega(k_j)=\omega(k)$; hence the same [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) holds at all three $k_j$. In particular, the missing traces satisfy the concrete [linear system](../../../../../../system-of-linear-equations.md)

$$
\begin{pmatrix}
-ik&-1&e^{-ikL}\\
-i\alpha k&-1&e^{-i\alpha kL}\\
-i\alpha^2k&-1&e^{-i\alpha^2kL}
\end{pmatrix}
\begin{pmatrix}F_1\\F_2\\G_2\end{pmatrix}
=\begin{pmatrix}R_0\\R_1\\R_2\end{pmatrix},
$$

where, with a common upper time limit $t$,

$$
R_j=Q_0(k_j)-e^{\omega(k)t}Q(k_j,t)-k_j^2F_0+e^{-ik_jL}(k_j^2G_0-ik_jG_1).
$$

The [finite-time spectral boundary transforms](../../../../../../finite-time-spectral-boundary-transform.md) $F_j,G_j$ are invariant under these rotations because their time kernel depends only on $k^3$. The coefficients multiplying them are not invariant; these differences make the three equations useful for eliminating the missing boundary traces.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
