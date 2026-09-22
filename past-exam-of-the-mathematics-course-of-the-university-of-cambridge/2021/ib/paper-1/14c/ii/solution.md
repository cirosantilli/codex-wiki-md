<h1 id="14c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Before the change, the normalized [ground state](../../../../../../ground-state.md) of the infinite square well is

$$
\psi_0(x)=\sqrt{\frac2a}\sin\frac{\pi x}{a}.
$$

For an allowed post-quench energy $E\in(0,U_0)$ satisfying part (i), define the unnormalized eigenfunction

$$
\chi_E(x)=
\begin{cases}
\sin(kx),&0\leq x\leq a/2,\\[2pt]
\dfrac{\sin(ka/2)}{\sinh(la/2)}
\sinh(l(a-x)),&a/2\leq x\leq a.
\end{cases}
$$

Its normalization factor is

$$
N_E^{-2}=
\int_0^{a/2}\sin^2(kx)\,dx
+\frac{\sin^2(ka/2)}{\sinh^2(la/2)}
\int_{a/2}^{a}\sinh^2(l(a-x))\,dx.
$$

The [Born rule](../../../../../../born-rule.md) therefore gives

$$
\boxed{
\operatorname{prob}(E)
=\frac{2N_E^2}{a}
\left|
\int_0^{a/2}\sin\frac{\pi x}{a}\sin(kx)\,dx
+\frac{\sin(ka/2)}{\sinh(la/2)}
\int_{a/2}^{a}\sin\frac{\pi x}{a}\sinh(l(a-x))\,dx
\right|^2 }.
$$

For a value of $E$ that is not an eigenvalue, this probability is zero. The sudden change leaves the wavefunction fixed, while the energy eigenbasis changes.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14C](../../14c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
