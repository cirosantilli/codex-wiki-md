<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First suppose the [convex set](../../../../../convex-set-split.md) $K$ is closed in the [norm topology](../../../../../norm-topology.md), and $x_n\in K$ satisfies $x_n\rightharpoonup x$. Apply the [weak Banach–Saks theorem in a Hilbert space](../../../../../weak-banach-saks-theorem-in-a-hilbert-space.md) to the [weakly null sequence](../../../../../weakly-null-sequence.md) $x_n-x$. Along the resulting subsequence,

$$
z_m=\frac1m\sum_{k=1}^m x_{n_k}\longrightarrow x
$$

in [norm](../../../../../norm.md). Each $z_m$ is a [convex combination](../../../../../convex-combination.md) of points in $K$, so $z_m\in K$. Since $K$ is a [closed set](../../../../../closed-set.md) in the [norm topology](../../../../../norm-topology.md), $x\in K$.

Conversely, suppose $K$ is a [sequentially weakly closed set](../../../../../sequentially-weakly-closed-set.md). If $x\in\overline K$ in the [norm topology](../../../../../norm-topology.md), choose $x_n\in K$ with $\|x_n-x\|<1/n$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $|\langle x_n-x,z\rangle|\leq\|x_n-x\|\|z\|\to0$ for every $z$, hence [weak convergence](../../../../../weak-convergence.md) to $x$. The assumed closure property gives $x\in K$. The empty [set](../../../../../set-split.md) satisfies both properties too. Thus

$$
\boxed{K\text{ convex}:\quad K\text{ norm-closed}\ \Longleftrightarrow\ K\text{ sequentially weakly closed}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
