<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [normal ordering identity for up and down operators](../../../../../../normal-ordering-identity-for-up-and-down-operators.md), placing every $U$ before every $D$. The [commutator](../../../../../../commutator.md) from part (a) implies

$$
DU^i=U^iD+iU^{i-1},
$$

by induction on $i$. Multiplying the normal-ordered expansion on the left by $D+U$ therefore gives

$$
a_{i,j}(\ell+1)
=a_{i-1,j}(\ell)+a_{i,j-1}(\ell)+(i+1)a_{i+1,j}(\ell),
$$

where negative indices have coefficient zero and $a_{0,0}(0)=1$.

We prove that $a_{i,j}(\ell)=0$ unless $i,j\geq0$ and $\ell-i-j=2m$ for some integer $m\geq0$, and otherwise

$$
\boxed{a_{i,j}(\ell)=\frac{\ell!}{2^m i!j!m!}}.
$$

The formula holds at $\ell=0$. For the next step with $\ell+1-i-j=2m$, the three contributions in the recurrence, after factoring out $\ell!/(2^m i!j!m!)$, are respectively $i$, $j$, and $2m$. Terms with a negative index or $m-1<0$ are simply absent. Their sum is $i+j+2m=\ell+1$, giving the required $(\ell+1)!$ numerator. Parity and nonnegativity exclude every remaining case. This proves the coefficient formula.

Apply the identity to the empty partition. Since $D(\emptyset)=0$, only terms with $j=0$ survive. To finish at $\lambda\vdash n$, only $U^n$ can contribute, and its coefficient of $\lambda$ is $f_\lambda$, by the [Young branching graph](../../../../../../young-branching-graph.md) correspondence with [standard Young tableaux](../../../../../../standard-young-tableau.md). For $\ell=n+2m$,

$$
N(\ell,\lambda)
=\frac{\ell!}{2^m n!m!}f_\lambda
=\boxed{\binom{\ell}{n}(2m-1)!!\,f_\lambda}.
$$

Here $(2m-1)!!=1\cdot3\cdots(2m-1)$ is the odd [double factorial](../../../../../../double-factorial.md), with $(-1)!!=1$. Thus

$$
\boxed{N(2m,\emptyset)=\frac{(2m)!}{2^m m!}=(2m-1)!!}.
$$

The operator $(D+U)^\ell$ counts [oscillating tableaux](../../../../../../oscillating-path-in-the-young-lattice.md), allowing both upward and downward steps. A strictly upward path to level $n$ would necessarily have length $n$; the printed operator specification is what determines $N$ when $\ell>n$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
