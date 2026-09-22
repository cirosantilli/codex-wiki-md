<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

Choose the [vector potential](../../../../../vector-potential.md) $A=(-\int_0^yB(s)ds,0,0)$, whose curl is $(0,0,B(y))$, and a spin-down wavefunction $\Psi=e^{-ikx}\chi(y)(0,1)^{\mathsf T}$, independent of $z$. Define

$$
a(y)=\frac e\hbar\int_0^yB(s)ds,\qquad b(y)=\frac{eB(y)}\hbar,\qquad\epsilon=\frac{2mE}{\hbar^2}.
$$

The covariant $x$ derivative acts as $-i(k+a)$, and $\sigma_3$ acts as $-1$. The [Pauli equation](../../../../../pauli-equation.md) consequently reduces to

$$
-\chi''+(k+a)^2\chi-b\chi=\epsilon\chi,\qquad\boxed{a'=b>eB_0/\hbar>0}.
$$

The sign of the plane-wave phase was chosen to match the printed $k+a$ convention; choosing $e^{ikx}$ simply reverses the label $k$.

Set $W=k+a$ and $M=\partial_y+W$. On the square-integrable operator domain with vanishing boundary terms, $M^\dagger=-\partial_y+W$, and

$$
M^\dagger M=-\partial_y^2+W^2-W'=-\partial_y^2+(k+a)^2-b.
$$

Taking the inner product with $\chi$ gives $\epsilon\|\chi\|_2^2=\|M\chi\|_2^2\ge0$. Thus $\boxed{E\ge0}$.

A zero mode solves $M\chi=0$, so

$$
\boxed{\chi_k(y)=C_k\exp\!\left[-ky-\int_0^y a(s)ds\right].}
$$

Since $a(0)=0$ and $a'\ge b_0=eB_0/\hbar$, integration on either side of zero gives $\int_0^y a(s)ds\ge b_0y^2/2$. Therefore $|\chi_k(y)|\le|C_k|e^{-ky-b_0y^2/2}$, proving square integrability for every real $k$. Each can be normalized and supplies a distinct momentum label at zero energy. Hence **zero energy is infinitely degenerate**. In an infinite $x$ direction the individual plane waves are generalized momentum states; square-integrable superpositions of their normalized transverse zero modes give ordinary transverse states by the Fourier isometry. The stipulated zero $z$ momentum is understood per unit longitudinal length, or with periodic longitudinal normalization.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
