<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because $t^TM=n t^T$,

$$
t^TK^{-1}=t^T\left(I_n-\frac p{1+np}M\right)
=\frac1{1+np}t^T.
$$

Thus a fundamental quasiparticle has fractional constituent number

$$
\boxed{N(e_J)=t^TK^{-1}e_J=\frac1{1+np}.}
$$

Let $q$ be the gauge-charge vector of a local electron. Trivial full braiding with every integer quasiparticle $q'$ requires

$$
q'^TK^{-1}q\in\mathbb Z
\quad\text{for all }q'\in\mathbb Z^n.
$$

Equivalently $K^{-1}q=\ell$ for some $\ell\in\mathbb Z^n$, so the allowed local charges lie in the local-particle lattice

$$
q=K\ell.
$$

Unit constituent number requires

$$
1=t^TK^{-1}q=t^T\ell,
\qquad\text{that is,}\qquad \sum_I\ell_I=1.
$$

Finally its self-exchange angle is

$$
\theta_{qq}=\pi q^TK^{-1}q
=\pi\ell^TK\ell
=\pi\left(\sum_I\ell_I^2+p\left(\sum_I\ell_I\right)^2\right).
$$

For integer $\ell_I$, one has $\ell_I^2\equiv\ell_I\pmod2$, and hence

$$
\frac{\theta_{qq}}\pi\equiv1+p\pmod2.
$$

The exchange phase is fermionic precisely when this integer is odd. Therefore

$$
\boxed{q=K\ell,\quad\ell\in\mathbb Z^n,\quad\sum_I\ell_I=1,
\qquad p\text{ must be even}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
