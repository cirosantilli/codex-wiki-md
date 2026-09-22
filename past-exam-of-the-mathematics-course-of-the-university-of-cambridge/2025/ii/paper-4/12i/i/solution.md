<h1 id="12i/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $C=C([0,1])$ with the uniform norm. For rational numbers $0\leq a<b\leq1$, let $M^+_{a,b}$ and $M^-_{a,b}$ be the sets of functions that are respectively nondecreasing and nonincreasing on $[a,b]$.

Both sets are closed. For example, if $f_j\in M^+_{a,b}$ and $f_j\to f$ uniformly, then for $x<y$ in $[a,b]$,

$$
f(x)=\lim_jf_j(x)\leq\lim_jf_j(y)=f(y).
$$

They also have empty interior. Given $f\in M^+_{a,b}$ and $\varepsilon>0$, continuity lets us choose $a<x<y<b$ sufficiently close that

$$
0\leq f(y)-f(x)<\frac{\varepsilon}{2}.
$$

Add a continuous triangular bump $h$ supported near $x$, with $h(x)=3\varepsilon/4$, $h(y)=0$, and $\lVert h\rVert_\infty<\varepsilon$. Then $(f+h)(x)>(f+h)(y)$, so the $\varepsilon$-ball about $f$ is not contained in $M^+_{a,b}$. The analogous upward bump at $y$ deals with $M^-_{a,b}$. Thus both sets are nowhere dense.

There are only countably many rational pairs $(a,b)$, so

$$
\bigcup_{a,b\in\mathbb Q,\ 0\leq a<b\leq1}
\left(M^+_{a,b}\cup M^-_{a,b}\right)
$$

is meagre. Completeness of $C$ and the [Baire category theorem](../../../../../../baire-category-theorem.md) show that its complement is nonempty. Choose $f$ in that complement. If $f$ were monotone on an interval of positive length, that interval would contain a closed interval with rational endpoints, putting $f$ in one of the displayed sets. Hence $f$ is monotone on no interval of positive length, as described by the [generic nowhere-monotone continuous function](../../../../../../generic-nowhere-monotone-continuous-function.md) result.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12I](../../12i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
