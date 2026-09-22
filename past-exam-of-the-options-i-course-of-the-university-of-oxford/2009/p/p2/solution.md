<h1 id="p/p2/solution">Solution</h1>

↑ **Parent:** [P2](../p2.md)

For any $q\in\Pi_n$, write $f-q=(f-p)+(p-q)$. The stated [orthogonality](../../../../orthogonal-vectors.md) makes the two summands perpendicular in the given [inner product](../../../../inner-product-split.md), because $p-q\in\Pi_n$. The [Pythagorean theorem for inner product spaces](../../../../pythagorean-theorem-in-an-inner-product-space.md) therefore gives

$$
\|f-q\|^2=\|f-p\|^2+\|p-q\|^2\geq\|f-p\|^2.
$$

Equality is attained at $q=p$, and positive definiteness makes it unique. Thus $p$ is the [orthogonal projection](../../../../orthogonal-projection.md) of $f$ onto the [polynomial](../../../../polynomial-split.md) subspace.

For the weighted example set $p(x)=A+Bx$. [Orthogonality](../../../../orthogonal-vectors.md) against the [basis](../../../../basis.md) $1,x$ gives

$$
0=\int_{-1}^1x^2(x^2-A-Bx)\,dx=\frac25-\frac{2A}3,
$$



$$
0=\int_{-1}^1x^3(x^2-A-Bx)\,dx=-\frac{2B}5.
$$

Odd terms vanish on the symmetric [interval](../../../../interval-mathematics.md), so $A=3/5$ and $B=0$. Consequently

$$
\boxed{p(x)=\frac35}.
$$

The weight $x^2$ vanishes only at one point; its integral against $g^2$ is positive for every nonzero [continuous](../../../../continuous-function.md) $g$, so it really does define an [inner product](../../../../inner-product-split.md). For an optional error check, the squared minimum error is $2/7-12/25+6/25=8/175$.

## ↑ Ancestors (12)

1. [P2](../p2.md)
2. [P](../../p.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
