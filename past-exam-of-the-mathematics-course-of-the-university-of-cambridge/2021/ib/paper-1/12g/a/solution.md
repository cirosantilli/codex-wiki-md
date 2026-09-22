<h1 id="12g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Laurent theorem](../../../../../../laurent-theorem.md) says that if $f$ is analytic on an annulus

$$
r<|z-a|<R,
$$

then it has a unique [Laurent series](../../../../../../laurent-series.md)

$$
f(z)=\sum_{n=-\infty}^{\infty}c_n(z-a)^n
$$

converging locally uniformly on that annulus, where

$$
c_n=\frac1{2\pi i}\oint_C\frac{f(\zeta)}{(\zeta-a)^{n+1}}\,d\zeta
$$

for any positively oriented circle $C$ in the annulus around $a$.

An [isolated singularity](../../../../../../isolated-singularity-split.md) at $a$ is a point at which $f$ is not analytic although it is analytic on some punctured neighbourhood. It is removable when every $c_n$ with $n<0$ vanishes; it is a pole of order $m$ when $c_{-m}\ne0$ and $c_n=0$ for $n<-m$; and it is essential when infinitely many negative-index coefficients are nonzero.

For $0<|z|<1$,

$$
\frac1{z(z-1)}
=-\frac1z\frac1{1-z}
=-\sum_{n=0}^{\infty}z^{n-1}.
$$

For $|z|>1$,

$$
\frac1{z(z-1)}
=\frac1{z^2}\frac1{1-z^{-1}}
=\sum_{n=0}^{\infty}z^{-n-2}.
$$

The coefficients are unique after the annulus is fixed; these expansions differ because they represent the function on different annuli. At zero the first expansion has principal part $-z^{-1}$, so zero is a simple pole with residue $-1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
