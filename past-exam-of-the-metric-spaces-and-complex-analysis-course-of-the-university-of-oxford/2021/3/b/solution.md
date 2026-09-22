<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

The [identity theorem](../../../../identity-theorem.md) states that if two [holomorphic functions](../../../../holomorphic-function-split.md) on a [connected](../../../../connected-space.md) [open set](../../../../open-set.md) agree at a [sequence](../../../../sequence.md) of distinct points with an [accumulation point](../../../../limit-point.md) inside that set, then they agree everywhere on it. Equivalently, the zeros of a [holomorphic function](../../../../holomorphic-function-split.md) which is not identically zero cannot accumulate inside its [domain](../../../../domain-mathematical-analysis.md).

Because $f,g$ never vanish, their [logarithmic derivatives](../../../../logarithmic-derivative.md) are [holomorphic](../../../../holomorphic-function-split.md). The [holomorphic function](../../../../holomorphic-function-split.md)

$$
H=\frac{f'}f-\frac{g'}g
$$

vanishes at every $a_n$. Since the distinct $a_n$ converge to $a\in U$, the [identity theorem](../../../../identity-theorem.md) gives $H\equiv0$. Applying the [quotient rule](../../../../quotient-rule.md) now gives

$$
\left(\frac fg\right)'=\frac{f'g-fg'}{g^2}=\frac fg\left(\frac{f'}f-\frac{g'}g\right)=0.
$$

A [holomorphic function](../../../../holomorphic-function-split.md) with zero [derivative](../../../../derivative.md) on a [domain](../../../../domain-mathematical-analysis.md) is constant. One can see this locally from its [Taylor series](../../../../taylor-series.md), then propagate the constant using [connectedness](../../../../connected-space.md). Hence $f/g=c$ on $U$, with $c\ne0$, and

$$
\boxed{f=cg\text{ on }U.}
$$

The conclusion can fail if the accumulation occurs outside $U$. Take the [punctured complex plane](../../../../punctured-complex-plane.md) $U=\mathbb C\setminus\{0\}$ and

$$
f(z)=\exp(\cos(1/z)),\qquad g(z)=1,\qquad a_n=\frac1{n\pi}\quad(n\geq1).
$$

Both [functions](../../../../function-split.md) are nowhere vanishing and [holomorphic](../../../../holomorphic-function-split.md) on $U$, and $a_n\to0\notin U$. The [chain rule](../../../../chain-rule.md) gives

$$
\frac{f'(z)}{f(z)}=\frac{\sin(1/z)}{z^2},\qquad \frac{g'(z)}{g(z)}=0,
$$

so these [logarithmic derivatives](../../../../logarithmic-derivative.md) agree at every $a_n$. However, $f$ is not constant: for example $f(1/\pi)=e^{-1}$ and $f(1/(2\pi))=e$. Therefore no constant $c$ gives $f=cg$.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
