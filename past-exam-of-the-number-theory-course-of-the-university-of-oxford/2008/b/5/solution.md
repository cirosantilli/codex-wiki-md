<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the [basis](../../../../basis.md) $w_1,\ldots,w_d$, its [discriminant](../../../../discriminant.md) is

$$
\operatorname{disc}(B)=\det\big(\operatorname{Tr}_{K/\mathbb Q}(w_iw_j)\big)_{i,j}.
$$

Equivalently it is the square of the [determinant](../../../../determinant.md) of the [matrix](../../../../matrix.md) of the $d$ embeddings applied to the [basis](../../../../basis.md) vectors. It is nonzero because [number fields](../../../../number-field.md) are separable. An [integral basis](../../../../integral-basis.md) is a [basis](../../../../basis.md) of the [ring of integers](../../../../ring-of-integers.md) as a [free abelian group](../../../../free-abelian-group.md); in particular it is a rational [basis](../../../../basis.md) of the [field](../../../../field.md) and expresses every [algebraic integer](../../../../algebraic-integer.md) uniquely with [integer](../../../../integer-split.md) coefficients.

To prove existence, start with any rational [basis](../../../../basis.md) and multiply each vector by a suitable nonzero [integer](../../../../integer-split.md) to make it integral. This is possible by clearing coefficients in its monic rational [minimal polynomial of an algebraic element](../../../../minimal-polynomial-of-an-algebraic-element.md) and rescaling the variable. Let $M$ be the [lattice](../../../../free-abelian-group.md) spanned over $\mathbb Z$ by these integral vectors, and let $D\ne0$ be its [discriminant](../../../../discriminant.md). For any [algebraic integer](../../../../algebraic-integer.md) $\alpha=\sum_jc_jw_j$, each trace $\operatorname{Tr}(\alpha w_i)$ is an [integer](../../../../integer-split.md). The resulting [linear system](../../../../system-of-linear-equations.md) has integral coefficient [matrix](../../../../matrix.md) with [determinant](../../../../determinant.md) $D$. Its [adjugate matrix](../../../../adjugate-matrix.md) shows $c_j\in D^{-1}\mathbb Z$. Thus

$$
M\subseteq\mathcal O_K\subseteq D^{-1}M.
$$

A [subgroup](../../../../subgroup.md) of a finitely generated [free abelian group](../../../../free-abelian-group.md) is free and finitely generated. Here its rank is $d$, since it contains $M$ and is contained in a rank-$d$ [lattice](../../../../free-abelian-group.md). Its free generators are the required [integral basis](../../../../integral-basis.md).

For squarefree $d\ne1$, the quadratic [integral basis](../../../../integral-basis.md) is

$$
\boxed{\{1,(1+\sqrt d)/2\}\quad(d\equiv1\pmod4),\qquad\{1,\sqrt d\}\quad(d\equiv2,3\pmod4).}
$$

The source allows squarefree nonzero [integers](../../../../integer-split.md), so the degenerate value $d=1$ gives $K=\mathbb Q$ and [basis](../../../../basis.md) $\{1\}$ instead of a two-element [basis](../../../../basis.md).

In the biquadratic [field](../../../../field.md) define the three [automorphisms](../../../../automorphism.md) by changing respectively the sign of $\sqrt r$, the sign of $\sqrt2$, and both signs. Their actions are

$$
\begin{aligned}
\sigma_1(\mu)&=a+b\sqrt2-c\sqrt r-d\sqrt{2r},\\
\sigma_2(\mu)&=a-b\sqrt2+c\sqrt r-d\sqrt{2r},\\
\sigma_3(\mu)&=a-b\sqrt2-c\sqrt r+d\sqrt{2r}.
\end{aligned}
$$

Hence the three sums are $2a+2b\sqrt2$, $2a+2c\sqrt r$ and $2a+2d\sqrt{2r}$. If $\mu$ is integral, each sum is integral and lies in its displayed quadratic subfield. Their radicands are squarefree and respectively congruent to two, three and two modulo four. The quadratic [basis](../../../../basis.md) formula therefore forces all their two coefficients to be [integers](../../../../integer-split.md), proving

$$
\boxed{2a,2b,2c,2d\in\mathbb Z.}
$$

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
