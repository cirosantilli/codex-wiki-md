<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [global Schauder estimate](../../../../../../global-schauder-estimate.md) on a bounded $C^{2,\alpha}$ domain is

$$
\boxed{\|u\|_{C^{2,\alpha}(\overline\Omega)}
\leq C\left(\|u\|_{C^0(\overline\Omega)}+\|f\|_{C^{0,\alpha}(\overline\Omega)}
+\|\psi\|_{C^{2,\alpha}(\overline\Omega)}\right).}
$$

Here $C$ depends on $n,\alpha$, the domain's boundary regularity and $\|c\|_{C^{0,\alpha}}$, but not on the particular solution or data. The $C^0$ term is needed before uniqueness has been established. The given $\psi$ is an extension of the boundary data to the closure.

For $c\leq0$, choose $d$ with $\Omega\subset\{|x_1|<d\}$ and set $M=\sup_{\partial\Omega}|\psi|$, $F=\sup_\Omega|f|$. The hinted function

$$
b(x)=M+(e^{2d}-e^{x_1+d})F
$$

is nonnegative, dominates $|\psi|$ on the boundary, and satisfies

$$
(\Delta+c)b=-e^{x_1+d}F+cb\leq-F,
$$

since $x_1+d>0$. Therefore $(\Delta+c)(u-b)=f-(\Delta+c)b\geq0$ and $(\Delta+c)(-u-b)=-f-(\Delta+c)b\geq0$. Both functions are nonpositive on the boundary. The [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) gives $|u|\leq b$, hence the [supremum norm barrier for an elliptic Dirichlet problem](../../../../../../supremum-norm-barrier-for-an-elliptic-dirichlet-problem.md):

$$
\boxed{\|u\|_\infty\leq M+e^{2d}F.}
$$

Unlike the full [Schauder estimate](../../../../../../schauder-estimates.md), this last constant depends only on a slab containing $\Omega$, and is independent of how negative $c$ is.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
