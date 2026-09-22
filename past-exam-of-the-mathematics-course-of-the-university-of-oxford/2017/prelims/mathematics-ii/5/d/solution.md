<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Yes.** By [uniform convergence](../../../../../../uniform-convergence.md), choose $N$ so that $|p_n(x)-f(x)|<1$ for every $n\geq N$ and every $x\in\mathbb R$. Then

$$
|p_n(x)-p_N(x)|<2\qquad(n\geq N,\ x\in\mathbb R).
$$

The [polynomial](../../../../../../polynomial-split.md) $p_n-p_N$ is bounded on the whole [real line](../../../../../../real-line.md). The supplied growth property of nonconstant [polynomials](../../../../../../polynomial-split.md) implies that this difference must be constant; write $p_n=p_N+c_n$. Evaluating at zero gives $c_n=p_n(0)-p_N(0)\to c=f(0)-p_N(0)$. For each $x$, take the [limit of a sequence](../../../../../../limit-of-a-sequence.md) in $p_n(x)=p_N(x)+c_n$ to obtain

$$
\boxed{f(x)=p_N(x)+c\quad\text{for every }x\in\mathbb R.}
$$

This is a [polynomial](../../../../../../polynomial-split.md). The [uniform limits of polynomials on the real line](../../../../../../uniform-limits-of-polynomials-on-the-real-line.md) therefore have a tail in which all nonconstant coefficients have already stabilized; only the constant coefficients may continue to change.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
