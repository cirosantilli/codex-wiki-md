<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $\sigma=-1$, the reduced first-order outer equation is

$$
4x\log^2x\,z_0'+4z_0=0.
$$

The condition at $x=0$ selects

$$
\boxed{
z_0(x)=\exp\left(\frac1{\log x}\right)
}.
$$

Indeed $z_0\to1$ as $x\to0^+$, while $z_0\to0$ as $x\to1^-$. The boundary condition at $x=1$ must therefore be supplied by a [boundary layer](../../../../../../../boundary-layer.md).

Set

$$
X=\frac{1-x}{\varepsilon},
\qquad z(x;\varepsilon)=Z(X).
$$

Since $x\log^2x=O(\varepsilon^2X^2)$ in this layer, the convection term is lower order. The leading inner equation and matching conditions are

$$
Z_{XX}-4Z=0,\qquad Z(0)=1,\qquad Z\to0
\quad(X\to\infty).
$$

Thus

$$
\boxed{Z(X)=e^{-2X}}.
$$

The leading uniformly valid expression is

$$
\boxed{
z(x;\varepsilon)\sim
\exp\left(\frac1{\log x}\right)
+\exp\left[-\frac{2(1-x)}{\varepsilon}\right]
}.
$$

Near $x=0$ diffusion regularizes the divergent derivative of the outer approximation on the thinner scale $x|\log x|=O(\varepsilon)$, but the leading value there remains the already matched constant $1$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 336](../../../../paper-336-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
