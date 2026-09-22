<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A vector in a [rational representation](../../../../../rational-representation.md) is an [unstable vector in a rational representation](../../../../../unstable-vector-in-a-rational-representation.md) when $0\in\overline{Gv}$, with Zariski closure. For $G=SL_n(\mathbb C)$, the [Hilbert-Mumford criterion for the affine null cone](../../../../../hilbert-mumford-criterion-for-the-affine-null-cone.md) is

$$
\boxed{v\text{ unstable}\iff\exists\lambda:\mathbb C^*\to SL_n(\mathbb C)\text{ algebraic},\quad\lim_{t\to0}\lambda(t)v=0.}
$$

Every [algebraic one-parameter subgroup](../../../../../algebraic-one-parameter-subgroup.md) is conjugate to $\operatorname{diag}(t^{a_1},\ldots,t^{a_n})$ with integer $a_j$ summing to zero. This follows by decomposing the standard representation into characters of the multiplicative group, then imposing [determinant](../../../../../determinant.md) one. In its weight decomposition, a limit of zero means that only strictly positive weights occur.

The reverse implication in the criterion is immediate: the subgroup lies in $G$ and supplies points of the orbit tending to zero. For the harder implication, the complex orbit is locally closed and Zariski open in its closure. A nonempty Zariski-open subset of a complex irreducible variety is dense also in the usual topology. Thus choose $g_jv\to0$ in the ordinary vector-space topology. [Singular value decomposition](../../../../../singular-value-decomposition.md), with [determinant](../../../../../determinant.md) phases adjusted, gives

$$
g_j=k_j\operatorname{diag}(e^{b_{j1}},\ldots,e^{b_{jn}})\ell_j,\qquad k_j,\ell_j\in SU_n,\quad\sum_rb_{jr}=0.
$$

Use an $SU_n$-invariant [Hermitian inner product](../../../../../hermitian-form.md) on $V$. By compactness, after a subsequence $\ell_j\to\ell$. Put $w=\ell v$, and decompose it into the weights of the diagonal torus, $w=\sum_\chi w_\chi$. These [weight spaces](../../../../../weight-space.md) are orthogonal because the unitary diagonal torus preserves the inner product. Hence

$$
\|g_jv\|^2=\sum_\chi e^{2\chi(b_j)}\|(\ell_jv)_\chi\|^2\longrightarrow0.
$$

For every $\chi$ with $w_\chi\ne0$, its final norm is bounded away from zero for large $j$, forcing $\chi(b_j)\to-\infty$. There are only finitely many such weights, so choose a single real vector $b$ with sum zero and $\chi(b)<0$ for all of them. The inequalities are strict with integer coefficients. A nearby rational vector still satisfies them; multiply its negative by a common denominator to obtain integers $a_r$ of sum zero with $\chi(a)>0$ throughout this support. Then $\mu(t)=\operatorname{diag}(t^{a_r})$ takes $w$ to zero. Conjugating gives $\lambda(t)=\ell^{-1}\mu(t)\ell$ taking $v$ to zero, completing the proof. The zero vector itself satisfies the criterion trivially.

For degree-six [binary forms](../../../../../binary-form.md), a nontrivial [algebraic one-parameter subgroup](../../../../../algebraic-one-parameter-subgroup.md) of $SL_2$ is, after conjugation and choosing its direction, $\operatorname{diag}(t^a,t^{-a})$ with $a>0$. On $x^{6-j}y^j$ the weight is $a(6-2j)$. Strictly positive weights permit only $j=0,1,2$, so the form is divisible by $x^4$. Conversely every such form tends to zero under that subgroup. Changing basis replaces $x$ by any linear factor. The [root-multiplicity criterion for unstable binary forms](../../../../../root-multiplicity-criterion-for-unstable-binary-forms.md) therefore gives

$$
\boxed{f\in\operatorname{Sym}^6W\text{ unstable}\iff f=0\text{ or }f\text{ has a projective root of multiplicity at least }4.}
$$

A triple root alone is insufficient: $x^3y^3$ has weight zero and is not unstable. Nor does merely having a repeated root suffice.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
