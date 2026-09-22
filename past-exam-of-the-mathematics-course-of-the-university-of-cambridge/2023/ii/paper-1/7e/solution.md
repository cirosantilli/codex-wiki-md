<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Taking reciprocals in the finite product defining the [gamma function](../../../../../gamma-function.md) gives

$$
\frac1{\Gamma(z)}
=z\lim_{n\to\infty}n^{-z}
 \prod_{k=1}^n\left(1+\frac zk\right).
$$

Let $H_n=\sum_{k=1}^n k^{-1}$. Since

$$
n^{-z}
=e^{z(H_n-\log n)}e^{-zH_n}
=e^{z(H_n-\log n)}\prod_{k=1}^n e^{-z/k}
$$

and $H_n-\log n\to\gamma$, where $\gamma$ is the [Euler--Mascheroni constant](../../../../../euler-s-constant.md), passage to the limit gives the [Weierstrass product for the reciprocal gamma function](../../../../../weierstrass-product-for-the-reciprocal-gamma-function.md)

$$
\boxed{
\frac1{\Gamma(z)}
=ze^{\gamma z}\prod_{k=1}^{\infty}
 \left(1+\frac zk\right)e^{-z/k}
}.
$$

The logarithmic derivative of this identity is

$$
-\psi(z)
=\frac1z+\gamma
 +\sum_{k=1}^{\infty}
  \left(\frac1{z+k}-\frac1k\right).
$$

Since $k^{-1}-(z+k)^{-1}=z/[k(z+k)]$, the [digamma function](../../../../../digamma-function.md) therefore satisfies

$$
\boxed{
\psi(z)=-\gamma-\frac1z
 +z\sum_{k=1}^{\infty}\frac1{k(z+k)}
}.
$$

For real $z>0$, termwise differentiation gives the [trigamma function](../../../../../trigamma-function.md)

$$
\psi'(z)=\frac1{z^2}
 +\sum_{k=1}^{\infty}\frac1{(z+k)^2}>0.
$$

Thus $\psi$ is strictly increasing on the positive real axis. At the two positive integers needed here, telescoping gives

$$
\psi(1)=-\gamma<0,
\qquad
\psi(2)=1-\gamma>0.
$$

The [intermediate value theorem](../../../../../intermediate-value-theorem.md) supplies a zero in $(1,2)$, and strict increase makes it unique. This is the [positive zero of the digamma function](../../../../../positive-zero-of-the-digamma-function.md).

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
