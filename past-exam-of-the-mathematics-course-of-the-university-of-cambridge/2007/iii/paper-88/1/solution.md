<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume $A$ is finite and nonempty; the empty case is immediate. Here $2A=A+A$. Choose a nonempty [subset](../../../../../subset.md) $X\subseteq A$ minimizing

$$
K=\frac{|X+A|}{|X|}.
$$

Taking $X=A$ as a competitor gives $K\leq C$, and every [subset](../../../../../subset.md) $Y\subseteq X$ satisfies $|Y+A|\geq K|Y|$, including $Y=\varnothing$.

We first prove the [Petridis minimal-growth lemma](../../../../../petridis-minimal-growth-lemma.md) in the particular form needed: for every [finite set](../../../../../finite-set.md) $S$,

$$
|X+A+S|\leq K|X+S|.
$$

List $S=\{s_1,\ldots,s_t\}$ and let $X_j$ consist of those $x\in X$ for which $x+s_j$ does not belong to an earlier translate $X+s_h$, $h<j$. The [sets](../../../../../set-split.md) $X_j+s_j$ partition $X+S$, so $|X+S|=\sum_j|X_j|$.

If $x\in X\setminus X_j$, then $x+s_j=x'+s_h$ for some earlier $h$ and $x'\in X$. Hence every point of $x+A+s_j$ already belongs to $X+A+s_h$. Therefore the new points contributed by $(X+A)+s_j$ are contained in

$$
\bigl[(X+A)\setminus((X\setminus X_j)+A)\bigr]+s_j.
$$

Their number is at most

$$
|X+A|-|(X\setminus X_j)+A|\leq K|X|-K|X\setminus X_j|=K|X_j|.
$$

Summing over $j$ proves the lemma. With $S=A$, it gives

$$
|X+2A|\leq K|X+A|=K^2|X|.
$$

We also prove the [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md) directly. For each $d\in U-V$, choose one representation $d=u_d-v_d$. The map

$$
(d,x)\longmapsto(x+u_d,x+v_d)
$$

from $(U-V)\times X$ into $(X+U)\times(X+V)$ is [injective](../../../../../injective-function.md): subtracting the output coordinates recovers $d$, after which either coordinate recovers $x$. Thus $|U-V||X|\leq|X+U||X+V|$. Taking $U=V=2A$ now yields

$$
\boxed{|2A-2A|\leq\frac{|X+2A|^2}{|X|}\leq K^4|X|\leq C^4|A|.}
$$

This proves the required growth and [difference set](../../../../../difference-set.md) estimates directly.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 88](../../paper-88-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
