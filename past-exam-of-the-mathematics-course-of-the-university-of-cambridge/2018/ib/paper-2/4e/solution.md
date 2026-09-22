<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

A [metric space](../../../../../metric-space.md) metric $d:X\times X\to[0,\infty)$ satisfies positivity, $d(x,y)=0$ exactly when $x=y$, symmetry, and the [triangle inequality](../../../../../triangle-inequality.md). A subset $U\subseteq X$ is an [open set](../../../../../open-set.md) when every $x\in U$ has some $\varepsilon>0$ with the open ball $B_d(x,\varepsilon)\subseteq U$.

Both $\varnothing$ and $X$ are open. An arbitrary union of open sets is open because a point lies in one member supplying a ball. A finite intersection is open because the minimum of the finitely many available radii supplies a ball. Thus the metric-open sets satisfy the [topology axioms](../../../../../topology-axiom.md).

For $C[0,1]$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $d_1(f,g)\leq d_2(f,g)$, so the $d_2$ topology is at least as fine as the $d_1$ topology. To see strictness, define the continuous triangular spikes

$$
f_n(x)=\sqrt n\max\{1-nx,0\}.
$$

Then

$$
d_1(f_n,0)=\frac1{2\sqrt n}\longrightarrow0,
\qquad
d_2(f_n,0)^2=\int_0^{1/n}n(1-nx)^2\,dx=\frac13.
$$

Thus $f_n$ converges to zero in the [L1 norm](../../../../../l1-norm.md) but not in the [L2 norm](../../../../../l2-norm.md). **The two metrics induce different topologies.**

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
