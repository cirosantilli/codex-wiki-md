<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathcal H$ be the family of [closed half-spaces](../../../../../../closed-half-space.md) containing $C$. Certainly $C\subseteq\bigcap_{H\in\mathcal H}H$. To prove the reverse inclusion, exclude an arbitrary $z\notin C$.

Suppose first that $C$ is nonempty. Its [Euclidean projection onto a convex set](../../../../../../euclidean-projection-onto-a-convex-set.md) $p$ exists: minimizing the continuous squared distance may be restricted to a sufficiently large closed ball, whose intersection with the closed set is compact. Put $d=z-p\ne0$. For every $x\in C$, [convexity](../../../../../../convex-function.md) puts $p+t(x-p)$ in $C$ for $0\leq t\leq1$. Minimality of $p$ gives

$$
0\leq\left.\frac d{dt}\|z-p-t(x-p)\|^2\right|_{t=0+}
=-2\langle d,x-p\rangle.
$$

Thus the [closed half-space](../../../../../../closed-half-space.md)

$$
H_z=\{x:\langle d,x\rangle\leq\langle d,p\rangle\}
$$

contains $C$, while $\langle d,z\rangle=\langle d,p\rangle+\|d\|^2$ excludes $z$. Since every point outside $C$ is excluded by some member of $\mathcal H$,

$$
\boxed{C=\bigcap_{\substack{H\text{ a closed half-space}\\C\subseteq H}}H.}
$$

This is the [half-space representation of a closed convex set](../../../../../../half-space-representation-of-a-closed-convex-set.md). If $C=\varnothing$, every point can again be excluded by a containing half-space, so the intersection is empty. If $C=\mathbb R^n$, no proper half-space contains it and the empty intersection is, by convention, $\mathbb R^n$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
