<h1 id="2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Set

$$
M_\psi(t)=\int_{\mathbb R^3}u_t
\left(\nabla\psi\cdot\nabla u+\frac{\Delta\psi}{2}u\right)dx.
$$

Differentiate, substitute $u_{tt}=\Delta u-u|u|^{p-1}$, and integrate every second derivative off $u$. The mixed first-derivative terms cancel because of the correction $(\Delta\psi)u/2$. For radial $u$ and radial $\psi$, the Hessian term is $\psi''|\nabla u|^2$. The potential term uses $u|u|^{p-1}\nabla u=\nabla(|u|^{p+1})/(p+1)$. One obtains the [Morawetz identity for the defocusing wave equation](../../../../../../morawetz-identity-for-the-defocusing-wave-equation.md)

$$
\boxed{-\frac{dM_\psi}{dt}
=\int_{\mathbb R^3}\left[
\psi''|\nabla u|^2-\frac14(\Delta^2\psi)u^2
+\frac{p-1}{2(p+1)}(\Delta\psi)|u|^{p+1}
\right]dx.}
$$

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2](../../2.md)
3. [Paper 154](../../../paper-154-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
