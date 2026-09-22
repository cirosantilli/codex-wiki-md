<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Fix $z_0\notin\Gamma$ and put $\delta=\operatorname{dist}(z_0,\Gamma)>0$. If $|z-z_0|<\delta/2$, then

$$
\left|\frac1{w-z}-\frac1{w-z_0}\right|
\leq \frac{2|z-z_0|}{\delta^2}
$$

uniformly for $w\in\Gamma$. Multiplication by the bounded [continuous function](../../../../../continuous-function.md) $f$ and integration therefore prove continuity of $F$ at $z_0$.

Take $\Gamma$ to be the positively oriented unit circle and $f\equiv1$. By the [Cauchy integral formula](../../../../../cauchy-integral-formula.md), $F(z)=1$ inside the circle and $F(z)=0$ outside it, so no continuous extension across $\Gamma$ exists.

For the final assertion, cover $K$ by finitely many sufficiently small closed axis-parallel squares whose slightly enlarged squares lie in $\Omega$, choosing the grid so that no boundary meets $K$. Apply the square Cauchy formula to $f$ on every selected square and add the results. [Integrals](../../../../../integral.md) over shared edges cancel with opposite orientations. The remaining finitely many oriented boundary polygons can be split into contours $\Gamma_j\subset\Omega\setminus K$, and their sum is

$$
f(z)=\sum_j\frac1{2\pi i}\oint_{\Gamma_j}\frac{f(w)}{w-z}\,dw
$$

for every $z\in K$.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
