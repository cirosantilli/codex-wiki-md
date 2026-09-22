<h1 id="35b/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The condition $2m=\hbar^2$ makes

$$
H=-\frac{d^2}{dx^2}-V_0e^{-x^2}.
$$

For

$$
\psi_a(x)=e^{-ax^2/2},
\qquad a>0,
$$

the squared norm is the [Gaussian integral](../../../../../../../gaussian-integral.md)

$$
\langle\psi_a|\psi_a\rangle
=\int_{\mathbb R}e^{-ax^2}\,dx
=\sqrt{\frac\pi a}.
$$

Since $\psi_a'=-ax\psi_a$, integration by parts gives the kinetic quotient

$$
\frac{\int\psi_a(-\psi_a'')\,dx}
{\int\psi_a^2\,dx}
=\frac{\int|\psi_a'|^2\,dx}{\int\psi_a^2\,dx}
=a^2\frac{\int x^2e^{-ax^2}\,dx}
{\int e^{-ax^2}\,dx}
=\frac a2.
$$

The potential quotient is

$$
-V_0
\frac{\int e^{-(a+1)x^2}\,dx}
{\int e^{-ax^2}\,dx}
=-V_0\sqrt{\frac a{1+a}}.
$$

The variational principle therefore yields the [Gaussian variational bound for an attractive Gaussian well](../../../../../../../gaussian-variational-bound-for-an-attractive-gaussian-well.md)

$$
\boxed{
E_0\leq E(a)
=\frac a2-V_0\frac{\sqrt a}{\sqrt{1+a}}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [35B](../../../35b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
