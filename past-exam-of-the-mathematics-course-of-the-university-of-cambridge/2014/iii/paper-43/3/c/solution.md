<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume $m\ne0$, since the trivial $m=0$ theory cannot fix $\beta$ or the [vacuum expectation value](../../../../../../vacuum-expectation-value.md). A zero-energy vacuum must satisfy both $V=0$ and stationarity in both real scalar directions. With the notation from the preceding solution, these become $H=H_x=H_y=0$, because the prefactor $|m|^4e^{x^2+y^2}$ is positive. The derivatives are

$$
H_x=2P(2x+\beta)-6(x+\beta),\qquad
H_y=2y(2P+\beta^2-3).
$$

These conditions also show that the zero-energy [stationary point](../../../../../../stationary-point.md) must be real. If $y\ne0$, the second equation gives $P=(3-\beta^2)/2$; the first then gives $x=-(\beta^2+3)/(2\beta)$. Substituting into the definition of $P$ gives $x^2+y^2=2$. But

$$
x^2=\frac{(\beta^2+3)^2}{4\beta^2}\geq3,
$$

which is impossible. Thus $y=0$, without assuming a real vacuum in advance.

Set $t=x+\beta$ and $F=1+xt$. Since $t=0$ would give $H=1$, it cannot occur. The zero-energy equation gives $F=s\sqrt3\,t$, $s\in\{1,-1\}$. Stationarity gives

$$
2F(2x+\beta)-6t=0\quad\Longrightarrow\quad 2x+\beta=s\sqrt3.
$$

Combining these equations gives $1=(s\sqrt3-x)t=t^2$. Writing $t=\varepsilon\in\{1,-1\}$ produces

$$
x=s\sqrt3-\varepsilon,\qquad \beta=2\varepsilon-s\sqrt3.
$$

The condition $\beta>0$ leaves exactly $(s,\varepsilon)=(1,1)$ and $(-1,1)$. The second branch is a [saddle point](../../../../../../saddle-point.md), as its real-direction curvature is negative; the stability calculation in the next solution verifies this explicitly. The [stable zero-energy Polonyi vacuum](../../../../../../stable-zero-energy-polonyi-vacuum.md) therefore selects

$$
\boxed{\beta=2-\sqrt3,\qquad A=3,\quad B=2.}
$$

Zero energy alone, without stationarity and stability, would not imply this parameter value. Even zero energy plus stationarity also admits $\beta=2+\sqrt3$ on the unstable branch.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
