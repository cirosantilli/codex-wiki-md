<h1 id="35c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a lattice of period $a$, wavevectors differing by the reciprocal-lattice vector $2\pi/a$ describe the same translation eigenvalue. The first [Brillouin zone](../../../../../../brillouin-zone.md) may therefore be chosen as

$$
-\frac{\pi}{a}\leq k<\frac{\pi}{a}.
$$

[Bloch theorem](../../../../../../bloch-s-theorem.md) states that every energy eigenstate in a [periodic potential](../../../../../../periodic-potential.md) may be chosen in the form

$$
\boxed{\psi_k(x)=e^{ikx}u_k(x),\qquad u_k(x+a)=u_k(x)}.
$$

To prove it, let $T_a$ be translation by one period:

$$
(T_a\psi)(x)=\psi(x+a).
$$

Periodicity gives $[T_a,H]=0$. The translation operator is unitary, so it can be diagonalized within each energy eigenspace. Choose a common eigenstate,

$$
T_a\psi=\lambda\psi.
$$

Unitarity gives $|\lambda|=1$, so $\lambda=e^{ika}$ for some real $k$. Thus $\psi(x+a)=e^{ika}\psi(x)$. Defining $u_k(x)=e^{-ikx}\psi(x)$ gives

$$
u_k(x+a)=e^{-ik(x+a)}e^{ika}\psi(x)=u_k(x),
$$

which proves the theorem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [35C](../../35c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
