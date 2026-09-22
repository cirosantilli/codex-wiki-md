<h1 id="2/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Since $w=ru$,

$$
w_t+w_r=r\left(u_t+u_r+\frac ur\right),
$$

and radial integration satisfies $dx=4\pi r^2dr$. Multiplying the identity from part 6 by $4\pi$ therefore gives

$$
\frac d{dt}\int_{\mathbb R^3}\psi\left[
\frac12\left(u_t+u_r+\frac ur\right)^2
+\frac{|u|^{p+1}}{p+1}
\right]dx
$$



$$
=-\frac12\int_{\mathbb R^3}\psi'
\left(u_t+u_r+\frac ur\right)^2dx
+\frac1{p+1}\int_{\mathbb R^3}|u|^{p+1}
\left(\psi'-(p-1)\frac\psi r\right)dx,
$$

which is the modified Morawetz identity.

Choose the constant weight $\psi=1$. The first term on the right vanishes and the second is

$$
-\frac{p-1}{p+1}\int_{\mathbb R^3}\frac{|u|^{p+1}}r,dx.
$$

The functional on the left is bounded by the conserved energy using the [Hardy inequality in Euclidean space](../../../../../../hardy-inequality-in-euclidean-space.md). Integrating in time gives another proof of the [Morawetz estimate for the defocusing wave equation](../../../../../../morawetz-estimate-for-the-defocusing-wave-equation.md).

## ↑ Ancestors (11)

1. [7](../7.md)
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
