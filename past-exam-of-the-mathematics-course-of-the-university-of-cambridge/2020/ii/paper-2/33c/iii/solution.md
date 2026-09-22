<h1 id="33c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The first [Born approximation for a one-dimensional reflection coefficient](../../../../../../born-approximation-for-a-one-dimensional-reflection-coefficient.md) follows by replacing the Jost solution inside its Volterra scattering equation by the free wave $e^{ikx}$:

$$
\boxed{
R(k)
=\frac{\epsilon}{2ik}
\int_{-\infty}^{\infty}e^{-2ikz}q(z)\,dz
+O(\epsilon^2)
}.
$$

To check the inverse problem, any shallow discrete state contributes only at $O(\epsilon^2)$ pointwise, so to first order the Marchenko input is

$$
F(s)
=\frac1{2\pi}\int_{-\infty}^{\infty}R(k)e^{iks}\,dk.
$$

Differentiating and inserting the Born approximation gives

$$
\begin{aligned}
F'(s)
&=\frac{\epsilon}{4\pi}
\int_{\mathbb R}\int_{\mathbb R}
e^{ik(s-2z)}q(z)\,dz\,dk+O(\epsilon^2)\\
&=\frac{\epsilon}{4}q(s/2)+O(\epsilon^2),
\end{aligned}
$$

where the second line is the [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md). At first order the quadratic integral term in the Marchenko equation may be dropped, so

$$
K(x,y)=-F(x+y)+O(\epsilon^2).
$$

The reconstruction formula therefore returns

$$
u(x)
=-2\frac d{dx}K(x,x)
=4F'(2x)+O(\epsilon^2)
=\boxed{\epsilon q(x)+O(\epsilon^2)}.
$$

**Thus direct and inverse scattering agree to first order.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [33C](../../33c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
