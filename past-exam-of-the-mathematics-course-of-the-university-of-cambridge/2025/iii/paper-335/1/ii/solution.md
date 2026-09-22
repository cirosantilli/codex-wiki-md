<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let

$$
M(x;z_1,z_2)=\langle E(x,z_1)E(x,z_2)\rangle.
$$

Applying the [parabolic wave equation](../../../../../../parabolic-wave-equation.md) to each factor gives

$$
\boxed{2ikM_x+(\partial_{z_1}^2+\partial_{z_2}^2)M=0.}
$$

If $C(s)=\langle w(z)w(z+s)\rangle$, Gaussian averaging at the screen gives

$$
M(0;z_1,z_2)
=\boxed{\exp\{-k^2\xi^2[\sigma^2+C(z_1-z_2)]\}.}
$$

Stationarity makes this a function only of $s=z_1-z_2$. Since $\partial_{z_1}^2+\partial_{z_2}^2=2\partial_s^2$ on such functions,

$$
M_x=\frac{i}{k}M_{ss}.
$$

Writing $\widehat M_0(q)$ for the [Fourier transform](../../../../../../fourier-transform.md) of the screen value, the solution at arbitrary range is

$$
\boxed{
M(x;s)=\frac1{2\pi}\int_{\mathbb R}
\widehat M_0(q)e^{iqs-iq^2x/k}\,dq.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
