<h1 id="36e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The kinetic [matrix](../../../../../../matrix.md) is diagonal:

$$
\langle\phi_n|T|\phi_m\rangle
=\delta_{nm}\frac{\hbar^2\pi^2n^2}{2ma^2}.
$$

For the linear potential,

$$
\langle\phi_n|V|\phi_n\rangle=\frac{V_0}{2}
=\frac{9\hbar^2}{2ma^2},
$$

and

$$
\left\langle\phi_1\left|\frac xa\right|\phi_2\right\rangle
=2\int_0^1y\sin(\pi y)\sin(2\pi y)\,dy
=-\frac{16}{9\pi^2}.
$$

Thus, in units $\hbar^2/(ma^2)$,

$$
\mathcal H=
\begin{pmatrix}
(\pi^2+9)/2&-16/\pi^2\\
-16/\pi^2&(4\pi^2+9)/2
\end{pmatrix}.
$$

The lower [eigenvalue](../../../../../../eigenvalue.md) gives the [two-mode variational bound for a linearly tilted square well](../../../../../../two-mode-variational-bound-for-a-linearly-tilted-square-well.md)

$$
\boxed{
E_0\leq\frac{\hbar^2}{ma^2}
\left[
\frac{5\pi^2+18}{4}
-\sqrt{\frac{9\pi^4}{16}+\frac{256}{\pi^4}}
\right]}
\approx9.25936\,\frac{\hbar^2}{ma^2}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [36E](../../36e.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
