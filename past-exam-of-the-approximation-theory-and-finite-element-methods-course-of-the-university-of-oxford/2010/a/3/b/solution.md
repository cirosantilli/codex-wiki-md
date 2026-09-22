<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here the exchange point lies between adjacent reference points and has the same, positive error sign as the point it replaces. Hence the new set remains spatially ordered, and the old error at its points alternates in sign. Its magnitudes are $|h_0|$ everywhere except at $\eta$, where $M=u(\eta)-q(\eta)>|h_0|$.

Set $w_r=\prod_{j\ne r}(z_r-z_j)^{-1}$. Apply the order-$(n+1)$ [divided difference](../../../../../divided-difference.md) to $q$ and $v$; both vanish because their degrees are at most $n$. In the new alternation equations, all products $(-1)^rw_r$ have the same sign. Thus the [single-point exchange in polynomial minimax approximation](../../../../../single-point-exchange-in-polynomial-minimax-approximation.md) gives

$$
\boxed{|h_1|=|h_0|+\frac{|w_s|}{\sum_r|w_r|}(M-|h_0|)>|h_0|.}
$$

The [Remez algorithm](../../../../../remez-algorithm.md) repeatedly solves for the reference polynomial and common signed height, locates a larger error extreme, and performs an order-preserving exchange. The reference height bounds the optimum from below and the global error maximum bounds it from above. Their gap provides an optimality stopping certificate. A general implementation also needs the endpoint exchange rule when the new extreme lies outside the reference set.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
