<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An additive form of the [Plünnecke inequality](../../../../../plunnecke-inequality.md) is the following. If $A,B$ are nonempty finite subsets of an [abelian group](../../../../../abelian-group.md) and $|A+B|\leq K|A|$, then there is one nonempty $X\subseteq A$ such that, simultaneously for every integer $m\geq0$,

$$
\boxed{|X+mB|\leq K^m|X|.}
$$

Here $mB$ is an [iterated sumset](../../../../../iterated-sumset.md) and $0B=\{0\}$. In particular, its [Plünnecke-Ruzsa inequality](../../../../../plunnecke-ruzsa-inequality.md) consequence is

$$
\boxed{|kB-\ell B|\leq K^{k+\ell}|A|\qquad(k,\ell\geq0).}
$$

We prove both statements, so that the [sumset](../../../../../sumset.md) and [difference set](../../../../../difference-set.md) formulations are covered.

Choose a nonempty $X\subseteq A$ minimizing the ratio $|X+B|/|X|$, and denote this minimum by $\kappa$. Such a minimizer exists because $A$ is finite, and $\kappa\leq K$. Every $Z\subseteq X$ satisfies $|Z+B|\geq\kappa|Z|$, with the empty case also valid. We first prove the [Petridis minimal-growth lemma](../../../../../petridis-minimal-growth-lemma.md)

$$
|X+B+C|\leq\kappa|X+C|
$$

for every finite nonempty $C$.

List $C=\{c_1,\ldots,c_t\}$. Let $U_i=X+\{c_1,\ldots,c_i\}$ and $U_0=\varnothing$. Define

$$
X_i=\{x\in X:x+c_i\notin U_{i-1}\},\qquad Z_i=X\setminus X_i.
$$

The new points of $U_i$ are exactly $X_i+c_i$, so $|X+C|=\sum_i|X_i|$. Since $Z_i+c_i\subseteq U_{i-1}$, the [sumset](../../../../../sumset.md) $Z_i+B+c_i$ is already contained in $U_{i-1}+B$. It follows that the new points introduced into $U_i+B$ are contained in

$$
\bigl((X+B)\setminus(Z_i+B)\bigr)+c_i.
$$

As $Z_i+B\subseteq X+B$, their number is at most

$$
|X+B|-|Z_i+B|\leq\kappa|X|-\kappa|Z_i|=\kappa|X_i|.
$$

Summing these increments proves the [Petridis minimal-growth lemma](../../../../../petridis-minimal-growth-lemma.md). Taking $C=(m-1)B$ for $m\geq1$ and iterating now gives

$$
|X+mB|\leq\kappa|X+(m-1)B|\leq\kappa^m|X|\leq K^m|X|.
$$

This proves the [Plünnecke inequality](../../../../../plunnecke-inequality.md) with the same minimizing set $X$ for every $m$.

To obtain the [difference set](../../../../../difference-set.md) bound, we also prove the required [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md). For finite $U,V,Z$ with $Z\ne\varnothing$, choose one representation $d=u_d-v_d$ of each $d\in U-V$. The map

$$
(U-V)\times Z\longrightarrow(U-Z)\times(Z-V),\qquad
(d,z)\longmapsto(u_d-z,z-v_d)
$$

is an [injection](../../../../../injective-function.md): the sum of the output coordinates recovers $d$, and the first coordinate then recovers $z$ because $u_d$ was fixed. Thus

$$
|U-V|\,|Z|\leq|U-Z|\,|Z-V|.
$$

Use $U=kB$, $V=\ell B$, and $Z=-X$. The already proved [Plünnecke inequality](../../../../../plunnecke-inequality.md) yields

$$
|kB-\ell B|\leq\frac{|X+kB|\,|X+\ell B|}{|X|}
\leq\kappa^{k+\ell}|X|\leq K^{k+\ell}|A|.
$$

This finishes the proof of the stated [Plünnecke-Ruzsa inequality](../../../../../plunnecke-ruzsa-inequality.md). The use of an [abelian group](../../../../../abelian-group.md) is essential in commuting the translates and [sumsets](../../../../../sumset.md) in the minimal-growth argument.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
