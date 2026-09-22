<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The parameter relations give $\mu=\log(n/c)$ and

$$
p=\left(\frac{\log(n/c)}{\binom{n-1}{2}}\right)^{1/3}
=\Theta\bigl(n^{-2/3}(\log n)^{1/3}\bigr).
$$

For each fixed integer $r\ge1$, take an $r$-vertex set $S$ and let $X_S$ count triangles meeting $S$. The event that every [vertex](../../../../../vertex-graph-theory.md) of $S$ is counted by $T$ is exactly $X_S=0$.

The number of such triangles is

$$
N_S=r\binom{n-r}{2}+\binom r2(n-r)+\binom r3
=r\binom{n-1}{2}-\binom r2(n-r)-2\binom r3.
$$

Thus their total expected count is $\mu_S=N_Sp^3=r\mu+O_r(np^3)=r\mu+o(1)$.

Distinct triangles have dependent containment events only when they share an [edge](../../../../../edge-of-a-graph.md). If that common [edge](../../../../../edge-of-a-graph.md) meets $S$, there are $O_r(n)$ choices for it and $O(n^2)$ choices for the two other [vertices](../../../../../vertex-graph-theory.md). If the common [edge](../../../../../edge-of-a-graph.md) avoids $S$, both other [vertices](../../../../../vertex-graph-theory.md) must lie in $S$, giving only $O_r(n^2)$ pairs. Each pair needs five [edges](../../../../../edge-of-a-graph.md). Consequently its ordered [Janson dependency sum](../../../../../janson-dependency-sum.md) is

$$
\Delta_S=O_r(n^3p^5)
=O_r\bigl(n^{-1/3}(\log n)^{5/3}\bigr)=o(1).
$$

[Janson inequality](../../../../../janson-inequality.md) gives the upper bound $\Pr(X_S=0)\le\exp(-\mu_S+\Delta_S/2)$. For the lower bound, the avoidance of each triangle is a [decreasing event](../../../../../decreasing-event.md). Repeated application of [Harris' inequality](../../../../../harris-inequality.md) gives

$$
\Pr(X_S=0)\ge(1-p^3)^{N_S}
=\exp[-\mu_S+O_r(n^2p^6)].
$$

The error $n^2p^6=O((\log n)^2/n^2)$ also tends to zero. The bounds match multiplicatively:

$$
\boxed{\Pr(X_S=0)=e^{-r\mu+o(1)}=(c/n)^r(1+o(1)).}
$$

Summing over ordered distinct [vertices](../../../../../vertex-graph-theory.md) yields the [factorial moments](../../../../../factorial-moment.md)

$$
\mathbb E(T)_r=(n)_r\Pr(X_S=0)\longrightarrow c^r.
$$

Here is an explicit justification that these moments determine the limit. For every integer $t\ge0$, the finite alternating sums

$$
\frac1{t!}\sum_{j=0}^{L}\frac{(-1)^j}{j!}\mathbb E(T)_{t+j}
$$

are upper bounds for $\Pr(T=t)$ when $L$ is even and lower bounds when $L$ is odd. This follows by applying the [Bonferroni inequalities](../../../../../bonferroni-inequalities.md) to $\binom{T}{t}\sum_j(-1)^j\binom{T-t}{j}$; the full sum is precisely the indicator of $T=t$. First let $n\to\infty$ for a fixed truncation and use the factorial-moment limits. Then let the even and odd truncations grow. Both bounds tend to

$$
\frac{c^t}{t!}\sum_{j=0}^\infty\frac{(-c)^j}{j!}=e^{-c}\frac{c^t}{t!}.
$$

Hence every point [probability](../../../../../probability.md) has the [Poisson distribution](../../../../../poisson-distribution.md) limit, proving the [Poisson threshold for vertices lying in no triangle](../../../../../poisson-threshold-for-vertices-lying-in-no-triangle.md):

$$
\boxed{T\ \xrightarrow{\ d\ }\ \operatorname{Po}(c).}
$$

This is also the [factorial-moment criterion for Poisson convergence](../../../../../factorial-moment-criterion-for-poisson-convergence.md), here justified rather than left as an unproved implication.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
