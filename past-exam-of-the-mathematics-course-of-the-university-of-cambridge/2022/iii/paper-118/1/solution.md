<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [almost complex structure](../../../../../almost-complex-manifold.md) on a [smooth manifold](../../../../../smooth-manifold.md) $M$ is a smooth bundle endomorphism $J:TM\to TM$ satisfying $J^2=-1$. On the complexified tangent bundle, $J$ has the eigenbundle decomposition

$$
TM\otimes\mathbb C=T^{1,0}M\oplus T^{0,1}M,
$$

with eigenvalues $i$ and $-i$. A [differential form of type (p, q)](../../../../../differential-form-of-type-p-q.md) is a section of $\bigwedge^p(T^{1,0}M)^*\otimes\bigwedge^q(T^{0,1}M)^*$. The operators $\partial$ and $\bar\partial$ are the type-$(1,0)$ and type-$(0,1)$ components of the [exterior derivative](../../../../../exterior-derivative.md).

We prove the three stated conditions are equivalent. If $X,Y$ have type $(1,0)$ and $\alpha$ has type $(0,1)$, the formula for the exterior derivative gives

$$
d\alpha(X,Y)=-\alpha([X,Y]).
$$

Thus closure of $T^{1,0}M$ under the [Lie bracket](../../../../../lie-bracket.md) is equivalent to the vanishing of the $(2,0)$ component of $d\alpha$ for every $(0,1)$-form. [Complex conjugation of differential-form type](../../../../../complex-conjugation-of-differential-form-type.md) gives the corresponding vanishing of the $(0,2)$ component on $(1,0)$-forms. Since every complex one-form is a sum of these two types, this is precisely

$$
d\alpha=\partial\alpha+\bar\partial\alpha.
$$

This proves (i)$\Longleftrightarrow$(ii).

Under (ii), the $(2,0)$ component of $d^2f=0$ is $\partial^2f$, proving (iii). Conversely, for $X,Y$ of type $(1,0)$,

$$
(\partial^2f)(X,Y)=df\bigl([X,Y]^{0,1}\bigr).
$$

If this vanishes for every smooth complex-valued $f$, then $[X,Y]^{0,1}=0$, so (iii) implies (i). These conditions define an [integrable almost complex structure](../../../../../integrable-almost-complex-structure.md).

For a [complex manifold](../../../../../complex-manifold.md), a holomorphic chart $z^j=x^j+iy^j$ defines $J_M(\partial_{x^j})=\partial_{y^j}$ and $J_M(\partial_{y^j})=-\partial_{x^j}$. The derivative of a holomorphic coordinate change is complex linear, hence commutes with multiplication by $i$; the definitions therefore glue and are independent of coordinates. Locally $T^{1,0}M$ is spanned by the commuting fields $\partial/\partial z^j$, so it is closed under brackets and $J_M$ is integrable. This is the [almost complex structure induced by a complex atlas](../../../../../almost-complex-structure-induced-by-a-complex-atlas.md).

We next prove the local [Dolbeault-Poincaré lemma](../../../../../dolbeault-poincare-lemma.md). Write a $\bar\partial$-closed $(0,q)$-form on a slightly larger polydisc as

$$
\varphi=\alpha+d\bar z_n\wedge\beta,
$$

where neither $\alpha$ nor $\beta$ contains $d\bar z_n$. Apply the supplied one-variable [Cauchy-Green operator](../../../../../cauchy-green-operator.md) coefficientwise to $\beta$, obtaining $\gamma$ with $\partial\gamma/\partial\bar z_n=\beta$. Then $\varphi-\bar\partial\gamma$ contains no $d\bar z_n$, and $\bar\partial\varphi=0$ says that its coefficients are holomorphic in $z_n$ and $\bar\partial$-closed in the first $n-1$ variables. Induction on $n$, with the one-variable formula as the base case, makes this remainder $\bar\partial$-exact. Hence every $\bar\partial$-closed $(0,q)$-form with $q>0$ is $\bar\partial$-exact on each bounded polydisc.

Finally, translation by $i$ leaves $d\bar z$ unchanged, so this form descends to $\mathbb C/(z\sim z+i)$. It is in fact exact on this noncompact [complex cylinder](../../../../../complex-cylinder.md), because the invariant function $z+\bar z=2\operatorname{Re}z$ descends and satisfies

$$
\boxed{\bar\partial(z+\bar z)=d\bar z.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 118](../../paper-118-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
