<h1 id="14b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Seek $z=v e^{i\Omega t}$ and put $\mu=m/M$. The generalized characteristic equation is

$$
\det(\mathsf K-\Omega^2\mathsf M)=0,
$$

or

$$
(1+\mu)(\omega_0^2-\Omega^2)^2-\mu\Omega^4=0.
$$

As a quadratic in $X=\Omega^2$, this is

$$
X^2-2(1+\mu)\omega_0^2X+(1+\mu)\omega_0^4=0,
$$

so

$$
\boxed{
\Omega_\pm^2=\omega_0^2\left(1+\mu\pm\sqrt{\mu(1+\mu)}\right).}
$$

A corresponding displacement vector is

$$
v_\pm=\begin{pmatrix}\omega_0^2-\Omega_\pm^2\\\Omega_\pm^2\end{pmatrix}.
$$

Thus the four normal modes are $v_+e^{\pm i\Omega_+t}$ and $v_-e^{\pm i\Omega_-t}$. Both squared frequencies are positive for every $\mu>0$, proving linear stability.

For $\mu\ll1$,

$$
\Omega_\pm
=\omega_0\left(1\pm\frac12\sqrt\mu+O(\mu)\right).
$$

Therefore, labeling the larger and smaller positive frequencies by $\omega$ and $\omega'$,

$$
\boxed{\omega-\omega'=\omega_0\sqrt\mu+O(\mu),}
$$

so $\alpha=\omega_0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14B](../../14b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
