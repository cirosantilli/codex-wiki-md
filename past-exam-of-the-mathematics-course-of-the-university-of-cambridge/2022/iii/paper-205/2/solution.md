<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [false discovery rate](../../../../../false-discovery-rate.md) is

$$
\operatorname{FDR}
=\mathbb E\left[\frac{V}{R\vee1}\right],
$$

where $R$ is the total number of rejections and $V$ is the number of rejected true nulls. The [Benjamini-Hochberg procedure](../../../../../benjamini-hochberg-procedure.md) orders the p-values and takes

$$
R=\max\{r:p_{(r)}\leq\alpha r/m\},
$$

with $R=0$ when the set is empty, then rejects the $R$ smallest p-values.

For $i\in I_0$, apply the modified procedure to $p_{-i}$ with critical values

$$
\frac{2\alpha}{m},\frac{3\alpha}{m},\ldots,\frac{m\alpha}{m},
$$

and let $R_i$ be its number of rejections. If the full procedure rejects $i$ and makes $r$ rejections, then $R_i=r-1$, and conversely

$$
\{i\text{ rejected},R=r\}
=\{p_i\leq\alpha r/m,\ R_i=r-1\}.
$$

Under Assumption A and the super-uniformity of a true-null p-value,

$$
\begin{aligned}
\mathbb E\frac{\mathbf1_{\{i\text{ rejected}\}}}{R}
&=\sum_{r=1}^m\frac1r
\mathbb P(p_i\leq\alpha r/m,R_i=r-1)\\
&\leq\sum_{r=1}^m\frac{\alpha}{m}
\mathbb P(R_i=r-1)=\frac\alpha m.
\end{aligned}
$$

Summing over $i\in I_0$ gives $\operatorname{FDR}\leq\alpha m_0/m\leq\alpha$.

Increasing any coordinates of $p_{-i}$ cannot increase the number of modified BH rejections. Hence

$$
D_r=\{p_{-i}:R_i\leq r-1\}
$$

is an increasing set.

Under Assumption B, put $t_r=\alpha r/m$ and $D_0=\varnothing$. The contribution of true null $i$ is bounded by

$$
\frac\alpha m\sum_{r=1}^m
\mathbb P(R_i=r-1\mid p_i\leq t_r).
$$

Now

$$
\mathbb P(R_i=r-1\mid p_i\leq t_r)
=\mathbb P(D_r\mid p_i\leq t_r)
-\mathbb P(D_{r-1}\mid p_i\leq t_r).
$$

Positive regression dependence and $t_{r-1}\leq t_r$ imply

$$
\mathbb P(D_{r-1}\mid p_i\leq t_r)
\geq\mathbb P(D_{r-1}\mid p_i\leq t_{r-1}).
$$

The resulting sum telescopes to at most one. Thus each true null again contributes at most $\alpha/m$, proving FDR control under Assumption B.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
