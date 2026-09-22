<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states that a [contraction mapping](../../../../../contraction-mapping.md) $f$ of a nonempty [complete metric space](../../../../../complete-metric-space.md) into itself has a unique [fixed point](../../../../../fixed-point.md). More explicitly, if $d(f(x),f(y))\leq qd(x,y)$ with $0\leq q<1$, iteration from any $x_0$ converges to that [fixed point](../../../../../fixed-point.md).

To prove this, put $x_{n+1}=f(x_n)$. Induction gives $d(x_{n+1},x_n)\leq q^nd(x_1,x_0)$, so for $m>n$ the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
d(x_m,x_n)\leq\sum_{j=n}^{m-1}q^jd(x_1,x_0)\leq\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus $(x_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md), and [completeness](../../../../../completeness.md) supplies a limit $x_*$. A [contraction mapping](../../../../../contraction-mapping.md) is [continuous](../../../../../continuous-function.md), so $f(x_*)=\lim f(x_n)=\lim x_{n+1}=x_*$. Two [fixed points](../../../../../fixed-point.md) satisfy $d(x_*,y_*)\leq qd(x_*,y_*)$, forcing equality of the points. Passing to the limit in the bound also gives the useful error estimate $d(x_n,x_*)\leq q^nd(x_1,x_0)/(1-q)$.

For the function space, take $X$ nonempty; otherwise the supremum in the printed definition is undefined without a convention. Boundedness of $X$ makes the [uniform metric](../../../../../uniform-metric.md) $\rho(f,g)$ finite. Nonnegativity and symmetry follow from $d$; $\rho(f,g)=0$ means $f(x)=g(x)$ at every $x$. Taking suprema in $d(f(x),h(x))\leq d(f(x),g(x))+d(g(x),h(x))$ proves the [triangle inequality](../../../../../triangle-inequality.md). Hence $\rho$ is a [metric](../../../../../metric.md).

Suppose $(f_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md) for this [uniform metric](../../../../../uniform-metric.md). At each $x$, $d(f_n(x),f_m(x))\leq\rho(f_n,f_m)$, so [completeness](../../../../../completeness.md) of $X$ supplies a value $f(x)=\lim_n f_n(x)$. Given $\varepsilon>0$, choose $N$ with $\rho(f_n,f_m)<\varepsilon/2$ for all $n,m\geq N$. Fix $n\geq N$ and let $m\to\infty$ pointwise; then $d(f_n(x),f(x))\leq\varepsilon/2$ for every $x$. Thus $\rho(f_n,f)\leq\varepsilon/2<\varepsilon$. The [uniform limit theorem](../../../../../uniform-limit-theorem.md) makes this limit continuous, so $f\in F$. This proves the [completeness of the continuous-map space in the uniform metric](../../../../../completeness-of-the-continuous-map-space-in-the-uniform-metric.md).

Finally fix $f\in C$ with contraction constant $q_f<1$, and write $x_f=\theta(f)$ and $x_g=\theta(g)$. Using the [fixed point](../../../../../fixed-point.md) equations,

$$
d(x_g,x_f)\leq d(g(x_g),f(x_g))+d(f(x_g),f(x_f))\leq\rho(f,g)+q_fd(x_g,x_f).
$$

Therefore the [fixed-point stability in the uniform metric](../../../../../fixed-point-stability-in-the-uniform-metric.md) estimate is

$$
\boxed{d(\theta(g),\theta(f))\leq\frac{\rho(f,g)}{1-q_f}.}
$$

Choosing $\rho(f,g)<(1-q_f)\varepsilon$ proves **continuity of $\theta$ at every $f$**. The estimate uses the constant of the fixed map $f$ only; it does not require a common contraction constant for all nearby $g$.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
