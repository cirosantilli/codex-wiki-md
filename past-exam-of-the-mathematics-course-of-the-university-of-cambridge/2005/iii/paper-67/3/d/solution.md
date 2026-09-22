<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\Phi$ denote the common trace transform of the unique solution, or of the rotational average at an exceptional parameter. Because $q$ and $f$ are real and $\lambda$ is real, $\overline{\Phi(\bar k)}=\Phi(k)$ and $\overline{\Psi(\bar k)}=\Psi(k)$. Taking the Schwarz conjugate of the [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) means replacing $k$ by $\bar k$ and conjugating the whole equation. It yields the second of the [conjugate global relations for the modified Helmholtz equation](../../../../../../conjugate-global-relations-for-the-modified-helmholtz-equation.md):

$$
E(ik)\Phi(k)+E(i\bar ak)\Phi(\bar ak)+E(iak)\Phi(ak)
=\frac i2[E(ik)\Psi(k)+E(i\bar ak)\Psi(\bar ak)+E(iak)\Psi(ak)].
$$

In this conjugation the rotated arguments interchange; after putting terms in the order $k,\bar ak,ak$, the coefficients have the displayed signs and arguments. Define

$$
\chi(k)=\frac l2\left(k+\frac\lambda k\right),\qquad e(k)=e^{\chi(k)}.
$$

The elementary cube-root identities give

$$
\begin{aligned}
E(iak)E(-ik)&=e(\bar ak),& E(iak)E(-i\bar ak)&=e(-k),\\
E(-iak)E(ik)&=e(-\bar ak),& E(-iak)E(i\bar ak)&=e(k).
\end{aligned}
$$

Multiply the first [global relation](../../../../../../global-relation-for-a-linear-boundary-value-problem.md) by $E(iak)$ and the conjugate one by $E(-iak)$. Then the coefficient of $\Phi(ak)$ is one in both equations:

$$
\begin{aligned}
e(\bar ak)\Phi(k)+e(-k)\Phi(\bar ak)+\Phi(ak)&=A(k),\\
e(-\bar ak)\Phi(k)+e(k)\Phi(\bar ak)+\Phi(ak)&=B(k),
\end{aligned}
$$

where all the quantities on the right are known,

$$
\begin{aligned}
A(k)&=-\frac i2[e(\bar ak)\Psi(k)+e(-k)\Psi(\bar ak)+\Psi(ak)],\\
B(k)&=\frac i2[e(-\bar ak)\Psi(k)+e(k)\Psi(\bar ak)+\Psi(ak)].
\end{aligned}
$$

Subtracting eliminates $\Phi(ak)$. If

$$
C(k)=\cosh\chi(\bar ak)\Psi(k)+\cosh\chi(k)\Psi(\bar ak)+\Psi(ak),
$$

the resulting **solution for the requested transform** is

$$
\boxed{\Phi(\bar ak)=\frac{2\sinh\chi(\bar ak)\Phi(k)+iC(k)}{2\sinh\chi(k)}.}
$$

At a zero of the denominator this identity is interpreted in its undivided form. The transforms themselves remain finite for $k\ne0$; consequently the numerator must vanish. That cancellation, rather than evaluation of a singular quotient, determines the Fourier coefficients below.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
