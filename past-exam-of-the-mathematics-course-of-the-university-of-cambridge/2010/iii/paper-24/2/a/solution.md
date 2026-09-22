<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An extending [absolute value on a field](../../../../../../absolute-value-algebra.md) is non-Archimedean by Question 1(a). We prove [finite-dimensional non-Archimedean norm equivalence over a complete field](../../../../../../finite-dimensional-non-archimedean-norm-equivalence-over-a-complete-field.md), using completeness rather than [local compactness](../../../../../../locally-compact-space.md).

Fix a [basis](../../../../../../basis.md) $e_1,\ldots,e_d$ of a finite-dimensional [vector space](../../../../../../vector-space-split.md) over $K$, and let $\|\cdot\|$ be a [norm](../../../../../../norm.md) homogeneous for the given [absolute value on a field](../../../../../../absolute-value-algebra.md) and satisfying the [ultrametric inequality](../../../../../../ultrametric-inequality.md). Write $\|\sum a_i e_i\|_0=\max_i|a_i|$. The upper bound

$$
\|v\|\leq C\|v\|_0,\qquad C=\max_i\|e_i\|,
$$

is immediate. For the lower bound use induction on $d$. The one-dimensional case is homogeneity. For the induction step, the span $W$ of $e_1,\ldots,e_{d-1}$ is complete for its restricted [norm](../../../../../../norm.md) by the induction comparison with the coordinate [norm](../../../../../../norm.md) and completeness of $K$. A complete [vector subspace](../../../../../../vector-subspace.md) of a [metric space](../../../../../../metric-space.md) is closed, so

$$
\delta=\inf_{w\in W}\|e_d-w\|>0.
$$

For $v=w+ae_d$ with $a\ne0$, scaling by $a$ gives $\|v\|\geq |a|\delta$; the same [coefficient](../../../../../../coefficient.md) bound is trivial when $a=0$. Also

$$
\|w\|\leq\max(\|v\|,|a|\|e_d\|)
\leq\max(1,\delta^{-1}\|e_d\|)\|v\|.
$$

The induction bound controls every coordinate of $w$ by a constant times $\|w\|$. Together with the bound on $a$, this proves $\|v\|_0\leq C'\|v\|$.

Two extending [absolute values on a field](../../../../../../absolute-value-algebra.md) on $L$ are [norms](../../../../../../norm.md) of this kind on its finite-dimensional [vector space](../../../../../../vector-space-split.md) over $K$. Hence there is $B>0$ with $|x|_2\leq B|x|_1$ for every $x\in L$. Apply this to $x^N$ and use multiplicativity:

$$
|x|_2\leq B^{1/N}|x|_1.
$$

Letting $N\to\infty$ gives $|x|_2\leq|x|_1$. Interchanging the two [norms](../../../../../../norm.md) gives equality. Thus

$$
\boxed{\text{There is at most one extending absolute value.}}
$$

The proof covers the trivial base [absolute value on a field](../../../../../../absolute-value-algebra.md) too. It proves uniqueness, without assuming an existence theorem or [compactness](../../../../../../compact-space.md) of the coordinate sphere $\{v:\|v\|_0=1\}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
