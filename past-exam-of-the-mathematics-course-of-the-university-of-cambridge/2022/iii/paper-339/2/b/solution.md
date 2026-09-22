<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use multiplier $-z$ for $Ax-b-s=0$. The Lagrangian is

$$
L(x,s,z)=\frac12x^TQx+I_{\mathbb R_+^m}(s)-z^T(Ax-b-s).
$$

The infimum over $s$ is finite exactly when $z\geq0$. The infimum over $x$ occurs at $x=Q^{-1}A^Tz$, and hence

$$
\boxed{h(z)=b^Tz-\frac12z^TAQ^{-1}A^Tz.}
$$

The dual is $\max_{z\geq0}h(z)$. Since the primal objective is coercive, the explicit [Slater condition](../../../../../../slater-s-condition.md)

$$
\boxed{\text{there exists }\bar x\text{ such that }A\bar x>b}
$$

is sufficient for feasibility, attainment, and equality of primal and dual values.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
