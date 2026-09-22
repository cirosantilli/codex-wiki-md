<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $t=\lceil\sqrt n\rceil$ and consider the powers

$$
S^t,S^{5t},S^{5^2t},\ldots,S^{5^{L+1}t},
$$

where $L$ is maximal subject to $5^{L+1}t\leq n/20$. For $n$ sufficiently large in terms of $d$, one has $L+1\geq\frac13\log_5n$. Since the successive growth ratios telescope,

$$
\prod_{i=0}^L\frac{|S^{5^{i+1}t}|}{|S^{5^it}|}
\leq\frac{|S^n|}{|S|}
\leq n^d.
$$

Thus one ratio is at most $n^{d/(L+1)}\leq5^{3d}$. For the corresponding $m=5^it$,

$$
\sqrt n\leq m\leq\frac n{100},
\qquad
|S^{5m}|\leq O_d(1)|S^m|.
$$

Set $B=S^m$. Then $|B^3|\leq O_d(1)|B|$, so the small-tripling argument from Question 1(b) makes

$$
A=B^2=S^{2m}
$$

an $O_d(1)$-approximate group. Apply the [Breuillard-Green-Tao structure theorem for approximate groups](../../../../../../breuillard-green-tao-structure-theorem-for-approximate-groups.md). It gives subgroups

$$
H\trianglelefteq C<G
$$

such that

$$
H\subseteq A^4=S^{8m}\subseteq S^{\lfloor n/2\rfloor},
$$

$C/H$ is a [nilpotent group](../../../../../../nilpotent-group.md) of class $O_d(1)$, and $A$ is covered by $O_d(1)$ left cosets of $C$.

It remains to pass from a covering to an index bound. The ball $S^m\subseteq A$ meets only $O_d(1)$ vertices of the [Schreier graph](../../../../../../schreier-graph.md) of $G/C$. If $G/C$ had more vertices, a simple path from $C$ would give more than that many distinct cosets within distance $O_d(1)$. Since $m\geq\sqrt n$ and $n$ is sufficiently large, this is impossible. Therefore

$$
\boxed{H\trianglelefteq C<G,\quad H\subseteq S^{\lfloor n/2\rfloor},
\quad [G:C]=O_d(1),\quad C/H\text{ is }O_d(1)\text{-step nilpotent}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 149](../../../paper-149-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
