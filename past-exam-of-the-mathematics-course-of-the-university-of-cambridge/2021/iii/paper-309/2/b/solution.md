<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the weak-field, slow-source approximation, the leading luminosity is the [quadrupole formula](../../../../../../quadrupole-formula.md)

$$
P(t)=\frac15\dddot Q_{ij}(t-R)\dddot Q_{ij}(t-R)
$$

in units $G=c=1$, where

$$
Q_{ij}=\int d^3x\,T_{00}
\left(x_ix_j-\frac13\delta_{ij}r^2\right).
$$

Only the $\ell=2$ symmetric trace-free coefficient contributes. Indeed,

$$
\int d\Omega\,\widehat x_i\widehat x_j
\widehat x_k\widehat x_l
=\frac{4\pi}{15}
(\delta_{ij}\delta_{kl}+\delta_{ik}\delta_{jl}+\delta_{il}\delta_{jk}),
$$

and contraction with traceless $a_{kl}$ removes the first term. Therefore

$$
\boxed{Q_{ij}(t)=\frac{8\pi}{15}
\int_0^\infty r^4a_{ij}(t,r)\,dr}.
$$

The power crossing the large sphere at time $t$ is consequently

$$
\boxed{
P(t)=\frac{64\pi^2}{1125}
\sum_{i,j}\left[
\int_0^\infty r^4
\frac{\partial^3a_{ij}}{\partial t^3}(t-R,r)\,dr
\right]^2}.
$$

The monopole is conserved total mass, the dipole is center-of-mass motion, and every $\ell\neq2$ term is orthogonal to the trace-free quadrupole at this leading order.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
