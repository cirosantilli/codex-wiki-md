<h1 id="19d/solution">Solution</h1>

↑ **Parent:** [19D](../19d.md)

Start with [Taylor's theorem](../../../../../taylor-theorem.md) with integral remainder, written on the whole interval using truncated powers:

$$
f(x)=\sum_{j=0}^k\frac{f^{(j)}(a)}{j!}(x-a)^j+\frac1{k!}\int_a^b(x-\theta)_+^k f^{(k+1)}(\theta)d\theta.
$$

For the [Peano kernel theorem](../../../../../peano-kernel-theorem.md), require that $L$ be a linear error functional, annihilate all polynomials of degree at most $k$, and permit interchange with this integral. These conditions hold, in particular, for finite linear combinations of point evaluations of $f$ and its derivatives through order $k$, with the truncated-power derivatives interpreted almost everywhere in $\theta$; dominated integration justifies the interchange. Another sufficient setting is a bounded functional on a differentiability space where the truncated-power integral is convergent in its norm. Polynomial exactness alone, without linearity and an integration-interchange justification, is not sufficient.

Applying $L$ annihilates the Taylor polynomial and gives

$$
\boxed{L(f)=\frac1{k!}\int_a^bK(\theta)f^{(k+1)}(\theta)d\theta,\qquad K(\theta)=L_x[(x-\theta)_+^k].}
$$

This is the unnormalized [Peano kernel](../../../../../peano-kernel.md) convention used by the question; including $1/k!$ within the kernel instead removes the factor outside the integral.

For the stated derivative error, constants and linear and quadratic polynomials are annihilated, so $k=2$. Acting on $(x-\theta)_+^2$ gives

$$
K(\theta)=2(1-\theta)_+-\frac12(2-\theta)^2
=\begin{cases}-\theta^2/2,&0\le\theta\le1,\\-(2-\theta)^2/2,&1\le\theta\le2.\end{cases}
$$

Thus the [sharp central-secant derivative error](../../../../../sharp-central-secant-derivative-error.md) satisfies

$$
|L(f)|\le\frac12\int_0^2|K(\theta)|d\theta\,\|f'''\|_\infty
=\frac12\left(\frac16+\frac16\right)\|f'''\|_\infty.
$$

Hence $c=1/6$ works. It is the minimum: for $f(x)=x^3$, $L(f)=3-4=-1$ and $\|f'''\|_\infty=6$, so no smaller constant can satisfy the inequality. Therefore

$$
\boxed{c_{\min}=\frac16.}
$$

The sign-definite kernel explains why a constant third derivative attains the bound exactly.

## ↑ Ancestors (10)

1. [19D](../19d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
