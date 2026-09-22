<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use uniform [expectations](../../../../../../expected-value.md) on the two nonempty parts, and equip their function spaces with the [inner product](../../../../../../inner-product.md) $\langle u,v\rangle=\mathbb E\overline u v$. Let $H=G-\gamma$ and

$$
(T_Hv)(x)=\mathbb E_yH(x,y)v(y).
$$

Since the [bipartite graph](../../../../../../bipartite-graph.md) is a [biregular graph](../../../../../../biregular-graph.md), both row and column averages of $H$ vanish. The [normalized adjacency operator of a bipartite graph](../../../../../../normalized-adjacency-operator-of-a-bipartite-graph.md) therefore splits into the map between constant functions, of [singular value](../../../../../../singular-value.md) $\gamma$, and $T_H$ between their [orthogonal complements](../../../../../../orthogonal-complement.md).

There is no [singular value](../../../../../../singular-value.md) larger than $\gamma$. Indeed, for $\gamma>0$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
|\mathbb E_yG(x,y)v(y)|^2
\leq\gamma\mathbb E_yG(x,y)|v(y)|^2.
$$

Averaging in $x$ uses the constant column degree and gives $\|\theta_Gv\|_2\leq\gamma\|v\|_2$. For $\gamma=0$ every operator is zero. Thus the second [singular value](../../../../../../singular-value.md) is

$$
s=\|T_H\|_{\mathrm{op}}.
$$

If one part has a single vertex, missing [singular values](../../../../../../singular-value.md) are interpreted as zero; the [biregular graph](../../../../../../biregular-graph.md) then has $H=0$.

The discrepancy in (i) is exactly $\mathbb E H1_A1_B$. Its supremum over $A,B$ is the [cut norm](../../../../../../cut-norm.md) $\delta=\|H\|_{\mathrm{cut}}$. To pass from this bound to arbitrary bounded [real-valued functions](../../../../../../real-valued-function.md), use the positive and negative parts and the identity $u_+(x)=\int_0^M1_{\{u(x)>t\}}\,dt$ for $|u|\leq M$. Applying this separately to both factors gives

$$
|\mathbb E_{x,y}H(x,y)u(x)v(y)|\leq4\delta MN
\quad\text{if }|u|\leq M,\ |v|\leq N.
$$

Here $N$ is a bound on $v$, unrelated to any [cardinality](../../../../../../cardinality.md).

If $s>0$, take real unit [left singular vector](../../../../../../left-singular-vector.md) $u$ and [right singular vector](../../../../../../right-singular-vector.md) $v$ with $T_Hv=su$ and $T_H^*u=sv$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and $|H|\leq1$ imply $\|u\|_\infty,\|v\|_\infty\leq1/s$. Hence

$$
s=\mathbb E Huv\leq\frac{4\delta}{s^2},
\qquad\boxed{s\leq(4c_1)^{1/3}}.
$$

This proves (i)$\Rightarrow$(iii), with a constant independent of both part sizes. The case $s=0$ satisfies the same conclusion immediately.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
