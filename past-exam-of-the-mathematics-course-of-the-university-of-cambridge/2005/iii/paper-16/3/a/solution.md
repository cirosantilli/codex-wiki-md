<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the separated-set definition of [topological entropy](../../../../../../topological-entropy.md). For a [compatible metric](../../../../../../compatible-metric.md) $d$ and $n\geq1$, define the [Bowen metric](../../../../../../bowen-metric.md) and separated-set count by

$$
d_n(x,y)=\max_{0\leq k<n}d(f^kx,f^ky),\qquad
s_n(d,\epsilon)=\max\{|E|:d_n(x,y)\geq\epsilon\text{ for distinct }x,y\in E\}.
$$

For fixed $n$, the [metric](../../../../../../metric.md) $d_n$ generates the original [topology](../../../../../../topology-split.md): it includes the $k=0$ term and all finitely many [iterations of a map](../../../../../../iterated-function.md) are [continuous](../../../../../../continuous-function.md). Thus its space is compact and $s_n(d,\epsilon)$ is finite. With natural logarithms, set

$$
h_d(f,\epsilon)=\limsup_{n\to\infty}\frac{\log s_n(d,\epsilon)}n,qquad
h_d(f)=\lim_{\epsilon\downarrow0}h_d(f,\epsilon).
$$

The last limit exists, possibly with value infinity, because decreasing $\epsilon$ can only increase separated-set counts.

Let $d'$ be another [compatible metric](../../../../../../compatible-metric.md). The identity $(X,d)\to(X,d')$ is a [continuous function](../../../../../../continuous-function.md) on a compact domain, hence [uniformly continuous](../../../../../../uniform-continuity.md). For every $\epsilon>0$, choose $\delta>0$ such that $d(x,y)<\delta$ implies $d'(x,y)<\epsilon$. The same implication at every iterate gives

$$
d_n(x,y)<\delta\ \Longrightarrow\ d'_n(x,y)<\epsilon.
$$

By its contrapositive, every $\epsilon$-[separated set](../../../../../../separated-subset-of-a-metric-space.md) for $d'_n$ is $\delta$-separated for $d_n$. Consequently $s_n(d',\epsilon)\leq s_n(d,\delta)$ for every $n$, and

$$
h_{d'}(f,\epsilon)\leq h_d(f,\delta)\leq h_d(f).
$$

Taking $\epsilon\downarrow0$ gives $h_{d'}(f)\leq h_d(f)$. Interchanging the two [compatible metrics](../../../../../../compatible-metric.md) gives the reverse inequality. Therefore

$$
\boxed{h_{d'}(f)=h_d(f)=h_{\mathrm{top}}(f).}
$$

[Compactness](../../../../../../compact-space.md) is used for [uniform continuity](../../../../../../uniform-continuity.md), not merely for pointwise equivalence of the two [metrics](../../../../../../metric.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
