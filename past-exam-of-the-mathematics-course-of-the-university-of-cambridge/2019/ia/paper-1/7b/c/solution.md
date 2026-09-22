<h1 id="7b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Over $\mathbb C$, triangularize $B$ and denote its eigenvalues, with algebraic multiplicity, by $\beta_1,\ldots,\beta_n$. Then

$$
\chi_{B^m}(z^m)=\prod_{j=1}^n(\beta_j^m-z^m).
$$

The numbers $\omega_l=e^{2\pi il/m}$ are all the [root of unity](../../../../../../root-of-unity.md) solutions of $w^m=1$, so

$$
\prod_{l=1}^m(t-\omega_lz)=t^m-z^m.
$$

Consequently

$$
\begin{aligned}
\prod_{l=1}^m\chi_B(\omega_lz)
&=\prod_{j=1}^n\prod_{l=1}^m(\beta_j-\omega_lz)\\
&=\prod_{j=1}^n(\beta_j^m-z^m)
=\boxed{\chi_{B^m}(z^m)}.
\end{aligned}
$$

If $\lambda$ is an eigenvalue of $B^m$, choose $z$ with $z^m=\lambda$. The displayed identity makes at least one factor $\chi_B(\omega_lz)$ zero. Thus $\mu=\omega_lz$ is an eigenvalue of $B$ and

$$
\boxed{\mu^m=\lambda}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7B](../../7b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
