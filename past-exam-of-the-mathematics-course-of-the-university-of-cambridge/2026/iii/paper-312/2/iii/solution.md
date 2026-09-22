<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $\mathbf q=\mathbf k_1$, $\mathbf k-\mathbf q=\mathbf k_2$, $q=|\mathbf q|$, and $\mu=\widehat{\mathbf k}\cdot\widehat{\mathbf q}$. Substitution into $F_2=5\alpha_s/7+2\beta/7$ gives

$$
F_2(\mathbf q,\mathbf k-\mathbf q)
=\frac{k^2[7k\mu+q(3-10\mu^2)]}
{14q(k^2-2kq\mu+q^2)}.
$$

The azimuthal integral in $d^3q=q^2dq\,d\mu\,d\phi$ and the factor two in $P_{22}$ then give

$$
P_{22}(k)=\int_0^\infty\frac{dq}{4\pi^2}
\int_{-1}^1d\mu\,
\frac{k^4[7k\mu+q(3-10\mu^2)]^2}
{98(k^2-2kq\mu+q^2)^2}
P(q)P(\sqrt{k^2-2kq\mu+q^2}).
$$

For the [scale-free matter power spectrum](../../../../../../scale-free-matter-power-spectrum.md) $P(k)=Ak^n$, put $r=q/k$ and

$$
s(r,\mu)=\sqrt{1-2r\mu+r^2}.
$$

All dimensional factors separate:

$$
\boxed{P_{22}(k)=A^2k^{2n+3}
\int_0^\infty dr\int_{-1}^1d\mu\,K_{22}(r,\mu;n)},
$$

where

$$
\boxed{K_{22}(r,\mu;n)=
\frac{r^n[7\mu+r(3-10\mu^2)]^2}
{392\pi^2[1-2r\mu+r^2]^{,2-n/2}}}.
$$

As $r\to0$, $K_{22}\sim r^n\mu^2/(8\pi^2)$, so the soft-$q$ integral converges exactly when $n>-1$. For $r\to\infty$, $K_{22}\sim r^{2n-2}$ times an angular function, requiring $n<1/2$. At fixed $\mu<1$, $r\to1$ is regular. The corner $(r,\mu)=(1,1)$ makes $|\mathbf k-\mathbf q|$ soft; after resolving that corner in the local soft momentum, its radial behavior is again $p^n dp$, requiring $n>-1$. Therefore

$$
\boxed{-1<n<\frac12}
$$

is the infrared- and ultraviolet-convergence window for $P_{22}$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
