<h1 id="12b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Both divergences vanish, so $\rho=0$. Faraday's and Ampere's curl equations respectively require

$$
kE_0=\omega B_0,
\qquad
kB_0=\omega E_0.
$$

For positive constants these imply

$$
\boxed{\omega=k,\qquad E_0=B_0,\qquad\rho=0}.
$$

The [Poynting vector](../../../../../../poynting-vector.md) is

$$
P=E_0^2\widehat x\cos^2(kx-\omega t).
$$

Only the two $x$-faces of the box contribute to its outward flux. With $a=\pi/(2k)$,

$$
\begin{aligned}
\int_SP\cdot dS
&=L^2E_0^2[
\cos^2(ka-\omega t)-\cos^2(\omega t)]\\
&=-L^2E_0^2\cos(2\omega t).
\end{aligned}
$$

The electromagnetic energy inside the box is

$$
U(t)=L^2E_0^2\int_0^a\cos^2(kx-\omega t)\,dx,
$$

and direct differentiation, using $\omega=k$, gives

$$
\frac{dU}{dt}=L^2E_0^2\cos(2\omega t).
$$

Thus

$$
\boxed{\int_SP\cdot dS=-\frac{dU}{dt}},
$$

confirming the integral identity when $J=0$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12B](../../12b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
