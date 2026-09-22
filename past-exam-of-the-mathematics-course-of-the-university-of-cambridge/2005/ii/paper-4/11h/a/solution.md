<h1 id="11h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the continued-fraction assertion, take the standard [Pell equation](../../../../../../pell-equation.md) hypothesis $N>0$ nonsquare. If $(x,y)$ is a solution with $x,y>0$, then

$$
\left|\frac xy-\sqrt N\right|
=\frac1{y^2(x/y+\sqrt N)}<\frac1{2y^2}.
$$

The convergent criterion for [continued fractions](../../../../../../continued-fraction.md) therefore makes $x/y$ a convergent to $\sqrt N$. Write its periodic expansion as $[a_0;\overline{a_1,\ldots,a_\ell}]$, and index convergents by $p_j/q_j$ with $p_0/q_0=a_0$. The norm-one convergents occur at $j=k\ell-1$ with $k\ell$ even. In particular the fundamental positive solution comes at $\ell-1$ if $\ell$ is even, and at $2\ell-1$ if it is odd. If $\varepsilon=x_1+y_1\sqrt N>1$ is this least norm-one unit, all integer solutions are represented by $\pm\varepsilon^m$, $m\in\mathbb Z$.

The [abelian group](../../../../../../abelian-group.md) law comes from multiplication of the norm-one expressions:

$$
\boxed{(x_0,y_0)\circ(x_1,y_1)
=(x_0x_1+Ny_0y_1,\ x_0y_1+x_1y_0)}.
$$

Their [field norms](../../../../../../field-norm.md) multiply, so the result remains a solution. Multiplication also proves associativity and commutativity; the identity is $(1,0)$ and the inverse of $(x,y)$ is $(x,-y)$. Cubing gives

$$
\boxed{(x,y)^{\circ3}
=(x^3+3Nxy^2,\ 3x^2y+Ny^3)
=(4x^3-3x,\ (4x^2-1)y)}.
$$

The last form uses $Ny^2=x^2-1$.

For completeness, the assertion about all powers follows by dividing any positive unit by the largest power of $\varepsilon$ not exceeding it: the remainder is a norm-one unit in $[1,\varepsilon)$, and minimality forces it to be $1$. Sign changes and inverses give the remaining solutions. If the phrase “nonsquare integer” includes negative $N$, real [continued fractions](../../../../../../continued-fraction.md) do not apply: $x^2+|N|y^2=1$ has only $(\pm1,0)$ except for $N=-1$, when $(0,\pm1)$ also occur. The same multiplication law still works in those finite groups.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11H](../../11h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
