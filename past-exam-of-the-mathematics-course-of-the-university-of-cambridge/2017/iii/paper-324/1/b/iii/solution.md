<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply the same positive-exponent [quantum Fourier transform](../../../../../../../quantum-fourier-transform.md) to each of the two [quantum registers](../../../../../../../quantum-register.md). The amplitude at $(c_1,c_2)$ of the [coset state](../../../../../../../coset-state.md) is

$$
\frac{e^{2\pi i k_0c_1/M}}{M\sqrt M}\sum_{b=0}^{M-1}e^{2\pi ib(yc_1+c_2)/M}.
$$

The [finite geometric series](../../../../../../../finite-geometric-series.md) is $M$ when $yc_1+c_2\equiv0\pmod M$ and zero otherwise. Therefore

$$
\boxed{c_2\equiv-yc_1\pmod M,\qquad P(c_1,c_2)=\frac1M\text{ on this support}.}
$$

There are $M$ allowed pairs, with $c_1$ following the [uniform distribution on a finite set](../../../../../../../discrete-uniform-distribution.md). The factor $e^{2\pi i k_0c_1/M}$ changes the [probability amplitudes](../../../../../../../probability-amplitude.md) by phases depending on the output label $c_1$, but has no effect on their [probabilities](../../../../../../../probability.md). Using an inverse rather than forward [quantum Fourier transform](../../../../../../../quantum-fourier-transform.md) on both [quantum registers](../../../../../../../quantum-register.md) gives the same support relation.

A [modular inverse](../../../../../../../modular-multiplicative-inverse.md) of $c_1$ exists precisely when $\gcd(c_1,M)=1$. In that case the [discrete logarithm](../../../../../../../discrete-logarithm-problem.md) is

$$
\boxed{y\equiv-c_2c_1^{-1}\pmod M.}
$$

It cannot generally be determined from every allowed pair. Put $d=\gcd(c_1,M)$. The supported [linear congruence](../../../../../../../linear-congruence.md) has $d$ solutions modulo $M$, and determines only $y$ modulo $M/d$; $(0,0)$ gives no information when $M>1$. For instance $p=5$ and $(c_1,c_2)=(2,2)$ are compatible with both $y=1$ and $y=3$. One may verify a candidate by [modular exponentiation](../../../../../../../modular-exponentiation.md), checking $g^y=x$. Repeated [discrete-logarithm Fourier sampling](../../../../../../../discrete-logarithm-fourier-sampling.md) finds an invertible $c_1$ with per-trial probability $\varphi(M)/M$, which has the same [totient lower bound from the Mertens product](../../../../../../../totient-lower-bound-from-the-mertens-product.md) as before. When $p=2$, the group is trivial and $x=1,y=0$ are determined without Fourier samples.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
