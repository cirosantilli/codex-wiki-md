<h1 id="2/iii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In free space $Q=0$, and the fourth moment obeys

$$
\partial_xm_4=\frac{i}{k}\partial_{r_1}\partial_{r_2}m_4.
$$

For the two-dimensional [Fourier transform](../../../../../../../fourier-transform.md)

$$
\widehat m_4(x,p_1,p_2)
=\int_{\mathbb R^2}m_4(x,r_1,r_2)
e^{-i(p_1r_1+p_2r_2)}\,dr_1dr_2,
$$

the [Fourier transform of a derivative](../../../../../../../fourier-transform-of-a-derivative.md) turns this equation into the [ordinary differential equation](../../../../../../../ordinary-differential-equation.md)

$$
\partial_x\widehat m_4
=-\frac{i}{k}p_1p_2\widehat m_4.
$$

Thus

$$
\boxed{
\widehat m_4(L,p_1,p_2)
=e^{-iLp_1p_2/k}
\widehat m_4(0,p_1,p_2)}.
$$

Using the screen-exit value from part (a), the inverse transform gives

$$
\boxed{
m_4(L,r_1,r_2)=\frac{1}{(2\pi)^2}
\int_{\mathbb R^2}e^{i(p_1r_1+p_2r_2)-iLp_1p_2/k}
\widehat{e^{-Q\Delta x}}(p_1,p_2)\,dp_1dp_2}
$$

through first order in $Δx$. Equivalently, the [free-space fourth-moment propagator](../../../../../../../free-space-fourth-moment-propagator.md) has kernel

$$
\boxed{
m_4(L,r_1,r_2)=\frac{k}{2\pi L}
\int_{\mathbb R^2}
\exp\left[\frac{ik}{L}(r_1-s_1)(r_2-s_2)\right]
m_4(0,s_1,s_2)\,ds_1ds_2}.
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iii](../../iii.md)
3. [2](../../../2.md)
4. [Paper 335](../../../../paper-335-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
