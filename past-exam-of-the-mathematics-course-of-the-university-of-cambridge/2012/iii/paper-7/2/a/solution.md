<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the conventional [Laplace operator](../../../../../../laplace-operator.md) $\Delta=\partial_{x_1}^2+\partial_{x_2}^2$. The [fundamental solution of the Laplace equation](../../../../../../fundamental-solution-of-the-laplace-equation.md) in two dimensions is $G(x)=(2\pi)^{-1}\log|x|$, with $\Delta G=\delta_0$. To check its sign, integrate the outward normal derivative around a circle: $\int_{\partial B_\varepsilon}\partial_n\log|x|\,ds=2\pi$. Applying [integration by parts](../../../../../../integration-by-parts.md) against a smooth compactly supported test function and shrinking the circle gives the distributional identity.

The printed [stream function](../../../../../../stream-function.md) has $\phi=-G*\omega$. For each [multi-index](../../../../../../multi-index-notation.md) $\beta$ with $|\beta|\leq2$, transfer derivatives to the compactly supported $C^2$ function:

$$
\partial^\beta\phi=-G*(\partial^\beta\omega).
$$

The logarithmic singularity is locally integrable. On a bounded region in $x$, the convolution uses one fixed bounded region in the integration variable; splitting off a small disk around the singularity proves [continuity](../../../../../../continuous-function.md) of these derivatives. Thus $\phi\in C^2$, and [convolution](../../../../../../convolution.md) of the distributional identity gives

$$
\boxed{\Delta\phi=-\omega.}
$$

**The asserted plus sign is false for the printed kernel and the conventional Laplacian.** Any nonzero smooth compactly supported $\omega$ is a counterexample. To obtain $\Delta\phi=\omega$, replace the kernel's minus sign by a plus sign, or explicitly adopt the negative [Laplace operator](../../../../../../laplace-operator.md). Below, retain the printed kernel and velocity convention. With that convention, $\operatorname{curl}u=\Delta\phi=-\omega$, so $\omega$ is the negative of conventional scalar [vorticity](../../../../../../vorticity.md). This sign does not change the transport or flow arguments.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
