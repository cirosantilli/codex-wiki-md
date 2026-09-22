<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For negative $x$, the [mean value theorem](../../../../../mean-value-theorem.md) gives $f'(x)=3+xf''(\xi_x)$. In particular,

$$
f'(-2)\leq-1<0,\qquad f'(-1)>0.
$$

Since $f'$ is [continuous](../../../../../continuous-function.md) and strictly increasing, it vanishes at exactly one point $x_m\in(-2,-1)$. The positive [second derivative](../../../../../second-derivative.md) makes $f$ a [strictly convex function](../../../../../strictly-convex-function.md) on the entire real line. Its [derivative](../../../../../derivative.md) changes from negative to positive at $x_m$, so **$x_m$ is the unique [global minimum](../../../../../global-minimum.md)**. One may also use $f(x)\geq x^2+3x-5\to\infty$ to verify [coercivity](../../../../../coercive-function.md).

In the endpoint-bracketing form of [golden-section search](../../../../../golden-section-search.md), begin with **$[-2,-1]$**, a width-one [interval](../../../../../interval-mathematics.md) known to contain this unique minimum, and place the two standard interior probes. The attainable position accuracy is different from that for a simple root. Around $x_m$, [Taylor's theorem](../../../../../taylor-s-theorem.md) gives

$$
f(x_m+h)-f(x_m)=\tfrac12f''(\xi)h^2.
$$

Here the minimum value is nonzero and of order one: the lower quadratic bound gives $f(x_m)\geq-29/4$, while $f(x_m)\leq f(-1)<-13/2$. Ordinary relative [round-off error](../../../../../round-off-error.md) in these [function](../../../../../function-split.md) values therefore hides changes of order $\epsilon$, once $h^2$ has that size. The [function-value resolution near a nondegenerate minimum](../../../../../function-value-resolution-near-a-nondegenerate-minimum.md) is consequently of order

$$
\boxed{|h|\sim\sqrt\epsilon=2^{-20}\approx9.54\times10^{-7}.}
$$

Each [golden-section search](../../../../../golden-section-search.md) contraction multiplies the bracket width by $\rho=(\sqrt5-1)/2$. Using $2^{-20}$ as the nominal target width gives

$$
N\geq\frac{20\log2}{-\log\rho}=28.81\ldots,
\qquad\boxed{N=29\text{ contractions}.}
$$

Unknown evaluation-error constants can change the actual stopping point; $29$ is the standard scale-based count. Requiring $2^{-40}$ position accuracy from these [function](../../../../../function-split.md)-value comparisons would disregard the quadratic flatness of the minimum. The same precision effect is documented for one-dimensional numerical minimization.[Caveats: Taylor expansion near the minimizer and the square-root precision limit; Minimization Algorithms: golden-section contraction](../../../../../one-dimensional-minimization-in-the-gnu-scientific-library-manual.md)

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
