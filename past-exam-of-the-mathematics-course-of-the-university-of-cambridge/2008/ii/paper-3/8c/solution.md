<h1 id="8c/solution">Solution</h1>

↑ **Parent:** [8C](../8c.md)

The [Möbius transformation](../../../../../mobius-transformation.md) $w=z/(z-1)$ sends $0\mapsto0$, $\infty\mapsto1$ and $1\mapsto\infty$. The [hypergeometric function](../../../../../hypergeometric-function.md) $F(a,c-b;c;w)$ has local exponent pairs $(0,1-c)$ at $w=0$, $(0,b-a)$ at $w=1$, and $(a,c-b)$ at $w=\infty$. Pulling back to $z$ and multiplying by $(z-1)^{-a}$ gives the pairs

$$
z=0:(0,1-c),\qquad z=\infty:(a,b),\qquad z=1:(0,c-a-b).
$$

At infinity the prefactor adds $a$ to both exponents, while at $z=1$ it subtracts $a$ from both pulled-back exponents. These are exactly the requested [Riemann P-symbol](../../../../../papperitz-symbol.md) exponents. Equivalently, the [Pfaff transformation](../../../../../pfaff-transformation.md) identifies this branch, up to a nonzero phase depending on the chosen branches, with $F(a,b;c;z)$.

When $c\notin\mathbb Z$, an independent [Frobenius solution](../../../../../frobenius-solution.md) is

$$
\boxed{z^{1-c}F(a-c+1,b-c+1;2-c;z).}
$$

Its exponent $1-c$ differs from the first branch's exponent zero, establishing [linear independence](../../../../../linear-independence.md). For resonant parameters, use a parameter limit giving the appropriate logarithmic branch. More directly, on a simply connected region avoiding the singularities and zeros of a nonzero first solution $y_1$, [reduction of order](../../../../../reduction-of-order.md) gives

$$
\boxed{y_2(z)=y_1(z)\int^z\frac{t^{-c}(1-t)^{c-a-b-1}}{y_1(t)^2}\,dt.}
$$

The [Wronskian](../../../../../wronskian.md) is a nonzero multiple of $z^{-c}(1-z)^{c-a-b-1}$, so this also produces an independent local solution in the resonant cases for which the first branch is defined.

## ↑ Ancestors (10)

1. [8C](../8c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
