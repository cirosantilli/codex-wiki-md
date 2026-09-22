<h1 id="16f/solution">Solution</h1>

↑ **Parent:** [16F](../16f.md)

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states: if $(X,d)$ is a nonempty complete [metric space](../../../../../metric-space.md) and $f:X\to X$ satisfies $d(fx,fy)\le qd(x,y)$ for a fixed $0\le q<1$, then it has exactly one [fixed point](../../../../../fixed-point.md) and the iteration from every starting point converges to it.

To prove existence, choose $x_0$ and let $x_{n+1}=f(x_n)$. Induction gives $d(x_{n+1},x_n)\le q^nd(x_1,x_0)$. The [triangle inequality](../../../../../triangle-inequality.md) and geometric sum then imply, for $m>n$,

$$
d(x_m,x_n)\le\frac{q^n}{1-q}d(x_1,x_0).
$$

The iterates are a [Cauchy sequence](../../../../../cauchy-sequence.md); completeness supplies their limit $x_*$. The contraction is continuous, so $f(x_*)=\lim f(x_n)=\lim x_{n+1}=x_*$. If $y_*$ is another [fixed point](../../../../../fixed-point.md), $d(x_*,y_*)\le qd(x_*,y_*)$ forces equality of the points. The same estimate gives geometric convergence from every initial point.

For the particular map, the original PDF gives $X=[\sqrt{a/2},\infty)$, which is a closed, complete subset of the real line. For positive $x$, the arithmetic-geometric mean inequality gives $f(x)=(x+a/x)/2\ge\sqrt a$, proving $f(X)\subset X$. Furthermore

$$
f'(x)=\frac12\left(1-\frac a{x^2}\right),\qquad -\frac12\le f'(x)<\frac12\quad(x\in X).
$$

The [mean value theorem](../../../../../mean-value-theorem.md) therefore gives $|f(x)-f(y)|\le|x-y|/2$, a genuine contraction. The fixed-point equation is $x^2=a$, and only the positive root belongs to $X$, so

$$
\boxed{x_*=\sqrt a.}
$$

The printed square-root endpoint is essential: the TeX transcription loses it.

## ↑ Ancestors (10)

1. [16F](../16f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
