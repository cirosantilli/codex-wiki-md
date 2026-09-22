<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We first prove the needed [Petridis minimal-growth lemma](../../../../../../petridis-minimal-growth-lemma.md). For finite nonempty [sets](../../../../../../set-split.md) $A,D$, choose a nonempty $X\subseteq A$ minimizing $K_0=|X+D|/|X|$. Thus $|Y+D|\geq K_0|Y|$ for every $Y\subseteq X$, including the empty [set](../../../../../../set-split.md). For any finite $T=\{t_1,\ldots,t_r\}$, define

$$
X_i=\{x\in X:x+t_i\notin\bigcup_{j<i}(X+t_j)\}.
$$

The [sets](../../../../../../set-split.md) $X_i+t_i$ partition $X+T$. If $x\notin X_i$, then $x+t_i\in X+t_j$ for some $j<i$, and therefore $x+D+t_i\subseteq X+D+t_j$. The newly contributed portion of $X+D+t_i$ consequently has size at most

$$
|X+D|-|(X\setminus X_i)+D|\leq K_0|X_i|.
$$

Sum over $i$ to obtain $|X+D+T|\leq K_0|X+T|$. Apply this successively with $T=(r-1)D$ to get $|X+rD|\leq K_0^r|X|$.

Use $D=-A$. The hypothesis implies $K_0\leq|A-A|/|A|\leq C$, so $|X-2A|\leq C^2|X|$. We also prove the [Ruzsa triangle inequality](../../../../../../ruzsa-triangle-inequality.md): for finite nonempty $U,V,W$,

$$
|U-W|\,|V|\leq|U-V|\,|V-W|.
$$

For each $s\in U-W$, fix $u_s,w_s$ with $s=u_s-w_s$. The map $(s,v)\mapsto(u_s-v,v-w_s)$ is injective: summing its coordinates recovers $s$, and then its first coordinate recovers $v$. This proves the inequality.

Apply it with $U=W=2A$ and $V=X$. Both right-hand factors have [cardinality](../../../../../../cardinality.md) $|X-2A|$, giving

$$
|2A-2A|\leq\frac{|X-2A|^2}{|X|}\leq C^4|X|\leq C^4n.
$$

Thus $\boxed{K=C^4\text{ suffices}}$. This is the required case of the [Plünnecke-Ruzsa inequality](../../../../../../plunnecke-ruzsa-inequality.md), proved here using the minimal-growth argument and the explicit injection. If $A$ is empty the conclusion holds directly.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
