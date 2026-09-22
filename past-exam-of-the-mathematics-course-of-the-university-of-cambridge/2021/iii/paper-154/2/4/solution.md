<h1 id="2/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let

$$
I(t)=\int_{\mathbb R^4}|x|^2|u(t,x)|^2\,dx.
$$

The first [virial identity](../../../../../../virial-identity.md), obtained from the equation by integration by parts, is

$$
I'(t)=4\operatorname{Im}\int_{\mathbb R^4}\overline u\,x\mathbin{\cdot}\nabla u\,dx.
$$

Differentiating once more gives

$$
I''(t)=8\int|\nabla u|^2-4\int x\mathbin{\cdot}\nabla\phi\,|u|^2.
$$

Write $\phi=W*|u|^2$, where $W(x)=-1/(C_4|x|^2)$ is homogeneous of degree $-2$. Symmetrizing the double integral and applying Euler's identity $z\cdot\nabla W(z)=-2W(z)$ yields

$$
\int x\mathbin{\cdot}\nabla\phi(x)|u(x)|^2\,dx
=-\int\phi|u|^2
=\int|\nabla\phi|^2.
$$

Therefore

$$
\boxed{I''(t)
=8\int|\nabla u|^2-4\int|\nabla\phi|^2
=16E(u)}.
$$

Not all solutions are global. Choose smooth finite-variance data of negative energy, which is possible by multiplying any nonzero test function by a sufficiently large constant: the kinetic term is quadratic in the amplitude and the attractive potential term is quartic. If such a solution were global, the [Virial identity for the four-dimensional gravitational Hartree equation](../../../../../../virial-identity-for-the-four-dimensional-gravitational-hartree-equation.md) would make the nonnegative function $I(t)$ strictly concave with constant negative second derivative, forcing it below zero in finite time. The solution must therefore blow up in finite time.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2](../../2.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
