<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

The [inverse function theorem](../../../../../inverse-function-theorem.md) says: if $U\subseteq\mathbb R^2$ is open, $F:U\to\mathbb R^2$ is smooth, $a\in U$, and $DF(a)$ is invertible, then there are open neighbourhoods $V\subseteq U$ of $a$ and $W$ of $F(a)$ for which $F:V\to W$ is a bijection with a smooth inverse. Its derivative is $D(F^{-1})(F(x))=[DF(x)]^{-1}$ after shrinking $V$ if necessary. A smooth function here has derivatives of every order.

For the given map,

$$
DF(x,y)=\begin{pmatrix}3x^2-1&-2y\\0&1\end{pmatrix},\qquad
\det DF(x,y)=3x^2-1.
$$

Thus its local smooth-invertibility set is

$$
\boxed{\{(x,y):x\ne\pm1/\sqrt3\}.}
$$

A differentiable local inverse is impossible at either excluded line by the [chain rule](../../../../../chain-rule.md). Even a merely continuous local inverse is impossible there: at fixed $y$, the cubic first component has a strict local extremum at these $x$ values, giving equal values at two nearby $x$ coordinates and preventing local injectivity.

On the curve, $y^2=x^3-x=x(x-1)(x+1)\ge0$. Its sign intervals give exactly $x\in[-1,0]\cup[1,\infty)$, so the two prescribed subsets cover the curve and are disjoint. For fixed $y$, the function $x^3-x$ is strictly increasing on $[1,\infty)$, starts at zero and tends to infinity. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) therefore gives a unique $p(y)\ge1$ with $p(y)^3-p(y)=y^2$.

At every point of this second component, $3x^2-1\ge2$, so the [inverse function theorem](../../../../../inverse-function-theorem.md) applies. Locally its smooth inverse evaluated at $(0,y)$ has the form $(p(y),y)$, by the proved uniqueness. These local descriptions agree on overlaps, proving **$p$ is smooth on all of $\mathbb R$**. For example,

$$
p'(y)=\frac{2y}{3p(y)^2-1},
$$

whose nonzero denominator also makes the smoothness mechanism transparent.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
