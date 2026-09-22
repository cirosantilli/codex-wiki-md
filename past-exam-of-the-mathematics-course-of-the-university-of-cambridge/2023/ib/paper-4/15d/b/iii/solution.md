<h1 id="15d/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take the spherical harmonic $Y_{00}$ to have unit angular norm. The radial normalization condition is then

$$
1=\int_0^\infty |R(r)|^2r^2\,dr
=C^2\int_0^\infty r^2e^{-2\gamma r}\,dr
=\frac{C^2}{4\gamma^3}.
$$

Therefore

$$
\boxed{C=2\gamma^{3/2}}.
$$

Equivalently, if $R$ denotes the entire spherically symmetric wavefunction rather than the radial factor multiplying normalized $Y_{00}$, then $C=(\gamma^3/\pi)^{1/2}$.

The expected radius is

$$
\begin{aligned}
\langle r\rangle_R
&=C^2\int_0^\infty r^3e^{-2\gamma r}\,dr\\
&=4\gamma^3\frac{3!}{(2\gamma)^4}
=\boxed{\frac{3}{2\gamma}}.
\end{aligned}
$$

For the ground state, $\gamma=mq^2/\hbar^2$. The [Bohr radius](../../../../../../../bohr-radius.md) is $a_0=\hbar^2/(mq^2)=1/\gamma$, so

$$
\boxed{\langle r\rangle_R=\frac32a_0}.
$$

The mean radius is therefore of the Bohr-radius scale and is one and a half times $a_0$. This is the [radial normalization of the hydrogen ground state](../../../../../../../radial-normalization-of-the-hydrogen-ground-state.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [15D](../../../15d.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
