<h1 id="1a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Collecting the shifted terms gives a [second-order difference equation](../../../../../../second-order-difference-equation.md) with coefficients $1-h/2$, $-(2+6h^2)$ and $1+h/2$. Substitute $y_n=r^n$ to obtain its [characteristic equation of a linear recurrence](../../../../../../characteristic-equation-of-a-linear-recurrence.md):

$$
(1-h/2)r^2-(2+6h^2)r+(1+h/2)=0.
$$

For real $h\ne0,2$, the roots and [general solution](../../../../../../general-solution.md) are

$$
r_\pm=\frac{1+3h^2\pm\frac h2\sqrt{25+36h^2}}{1-h/2},\qquad \boxed{y_n=Ar_+^n+Br_-^n.}
$$

In the small-step regime, indeed for $0<h<2$, the [polynomial](../../../../../../polynomial-split.md) is positive at $r=0$, negative at $r=1$ and positive for sufficiently large positive $r$. Thus $0<r_-<1<r_+$. The [bounded solution of a second-order constant-coefficient recurrence](../../../../../../bounded-solution-of-a-second-order-constant-coefficient-recurrence.md) discards the growing root, and $y_0=1$ fixes its remaining coefficient:

$$
\boxed{y_n=r_-^n,\qquad r_-=1-2h+2h^2+O(h^3),\qquad y_n\approx(1-2h)^n.}
$$

The [Taylor series](../../../../../../taylor-series.md) establishes the displayed approximation to the root. Raising that approximation to the $n$th power is a leading approximation, rather than a uniform relative approximation for arbitrarily large $n$: its relative error is controlled when $nh^2$ is small. For completeness, the degenerate values give $y_n=A+Bn$ when $h=0$, and $y_n=C13^{-n}$ when $h=2$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1A](../../1a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
