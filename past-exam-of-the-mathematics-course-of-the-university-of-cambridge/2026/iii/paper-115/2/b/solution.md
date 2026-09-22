<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For an arbitrary smooth variation $u_t=u+t\varphi$, differentiation under the integral gives

$$
\left.\frac d{dt}E(u_t)\right|_{t=0}
=\int_M\left(g^{ij}\partial_i u\,\partial_j\varphi-f\varphi\right)\sqrt{|g|}\,dx.
$$

Since $M$ is compact without boundary, integration by parts turns this into

$$
-\int_M\left[
\frac1{\sqrt{|g|}}\partial_j\left(\sqrt{|g|}g^{ij}\partial_i u\right)+f
\right]\varphi\,d\operatorname{vol}_g.
$$

The [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore gives the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md)

$$
-\frac1{\sqrt{|g|}}\partial_j\left(\sqrt{|g|}g^{ij}\partial_i u\right)=f,
$$

or equivalently $-\Delta_gu=f$ for the [Laplace-Beltrami operator](../../../../../../laplace-beltrami-operator.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 115](../../../paper-115-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
