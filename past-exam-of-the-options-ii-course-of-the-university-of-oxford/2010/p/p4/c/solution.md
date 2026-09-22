<h1 id="p/p4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the intended degree ordering from part (b). Let $\ell_j$ be the degree-$n$ Lagrange cardinal [polynomial](../../../../../polynomial-split.md) at the distinct [roots](../../../../../root-of-a-root-system.md) $x_0,\ldots,x_n$ of $p_{n+1}$:

$$
\ell_j(x)=\prod_{i\neq j}\frac{x-x_i}{x_j-x_i},\qquad
w_j=\int_a^b\ell_j(x)w(x)\,dx.
$$

For any $f\in\Pi_{2n+1}$, [polynomial division](../../../../../polynomial-division.md) gives $f=sp_{n+1}+r$ with $\deg s\leq n$ and $\deg r\leq n$. [Orthogonality](../../../../../orthogonal-vectors.md) of $p_{n+1}$ to $\Pi_n$ makes the integral of $sp_{n+1}$ zero, and that product also vanishes at every quadrature node. Meanwhile $r=\sum_jr(x_j)\ell_j$ by interpolation. Consequently

$$
\boxed{\int_a^bf(x)w(x)\,dx=\int_a^br(x)w(x)\,dx
=\sum_{j=0}^nw_jf(x_j).}
$$

Thus the rule is exact up to degree $2n+1$. To determine the sign of a weight, apply exactness to $\ell_j^2$, of degree $2n$:

$$
\boxed{w_j=\sum_iw_i\ell_j(x_i)^2
=\int_a^b\ell_j(x)^2w(x)\,dx>0.}
$$

The inequality is strict because $\ell_j$ is a nonzero [polynomial](../../../../../polynomial-split.md) and the weight is positive. This is the [Gaussian quadrature](../../../../../gaussian-quadrature.md) construction; the source asks only for nonnegative weights, and the proof gives positivity.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
