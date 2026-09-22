<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x=\cos\theta$ with $0<\theta<\pi$, differentiation of the [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) gives

$$
T_n'(\cos\theta)=n\frac{\sin(n\theta)}{\sin\theta},\qquad \frac{1-x^2}{n^2}T_n'(x)^2=\sin^2(n\theta)=1-T_n(x)^2.
$$

Both sides are [polynomials](../../../../../../polynomial-split.md) in $x$, so the identity holds at the endpoints and, in fact, for every real $x$.

Order the [roots of a polynomial](../../../../../../root-of-a-polynomial.md) here as $x_j=\cos\theta_j$, $\theta_j=(2j-1)\pi/(2n)$, so $x_1>\cdots>x_n$. At these simple roots,

$$
T_n'(x_j)=\frac{n(-1)^{j-1}}{\sin\theta_j},\qquad |T_n'(x_j)|=\frac{n}{\sqrt{1-x_j^2}}.
$$

For a [polynomial](../../../../../../polynomial-split.md) $q$ of degree at most $n-1$, the [Lagrange interpolation polynomial](../../../../../../lagrange-polynomial.md) is

$$
q(x)=\sum_{j=1}^n q(x_j)\ell_j(x),\qquad \ell_j(x)=\frac{T_n(x)}{(x-x_j)T_n'(x_j)}.
$$

For $x>x_1$, the [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) is positive: all its roots are at most $x_1$ and its leading coefficient is positive. Hence $\ell_j(x)T_n'(x_j)=T_n(x)/(x-x_j)>0$. The assumed nodal bounds and interpolation of the degree-$n-1$ [polynomial](../../../../../../polynomial-split.md) $T_n'$ now give

$$
|q(x)|\le\sum_j|\ell_j(x)|\,|T_n'(x_j)|=\sum_j\ell_j(x)T_n'(x_j)=T_n'(x).
$$

Continuity includes $x=x_1$. Apply this argument to $q(-x)$ and use the parity of the [Chebyshev polynomial](../../../../../../chebyshev-polynomial.md) to obtain the negative side. Thus the [Chebyshev nodal derivative comparison](../../../../../../chebyshev-nodal-derivative-comparison.md) proves

$$
\boxed{|q(x)|\le|T_n'(x)|\quad\text{when }|x|\ge\cos(\pi/(2n)).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
