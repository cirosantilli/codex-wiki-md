<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md), the [Killing form](../../../../../killing-form.md) is defined using the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md) on the algebra itself, rather than the given [Lie algebra representation](../../../../../lie-algebra-representation.md) $d$:

$$
\kappa(X,Y)=\operatorname{Tr}_{\mathcal L}(\operatorname{ad}_X\operatorname{ad}_Y),\qquad \operatorname{ad}_X(Z)=[X,Z].
$$

The [Jacobi identity](../../../../../jacobi-identity.md) gives $\operatorname{ad}_{[X,Y]}=[\operatorname{ad}_X,\operatorname{ad}_Y]$. Using the [cyclic property of the trace](../../../../../cyclic-property-of-the-trace.md),

$$
\begin{aligned}
\kappa([X,Y],Z)&=\operatorname{Tr}(\operatorname{ad}_X\operatorname{ad}_Y\operatorname{ad}_Z-\operatorname{ad}_Y\operatorname{ad}_X\operatorname{ad}_Z)\\
&=\operatorname{Tr}(\operatorname{ad}_X[\operatorname{ad}_Y,\operatorname{ad}_Z])=\kappa(X,[Y,Z]).
\end{aligned}
$$

The same trace identity makes the [Killing form](../../../../../killing-form.md) symmetric. For a [basis](../../../../../basis.md) $(t_a)$, the lowered [structure constants of a Lie algebra](../../../../../structure-constant-of-a-lie-algebra.md) are $c_{abc}=\kappa([t_a,t_b],t_c)$. Antisymmetry of the [Lie bracket](../../../../../lie-bracket.md) gives $c_{abc}=-c_{bac}$, while invariance gives $c_{abc}=\kappa(t_a,[t_b,t_c])=-c_{acb}$. The two adjacent transpositions generate every permutation, proving the [antisymmetry of Killing-lowered structure constants](../../../../../antisymmetry-of-killing-lowered-structure-constants.md): **$c_{abc}$ is totally antisymmetric**, even if the [Killing form](../../../../../killing-form.md) is degenerate.

A [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) has no nonzero solvable ideal; equivalently, its [solvable radical](../../../../../radical-of-a-lie-algebra.md) is zero, or, in characteristic zero, its [Killing form](../../../../../killing-form.md) is nondegenerate. A real [compact Lie algebra](../../../../../compact-lie-algebra.md) is the algebra of some [compact Lie group](../../../../../compact-lie-group.md), equivalently an algebra admitting a positive-definite [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md). For a real [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md) the [compactness criterion from the Killing form](../../../../../compactness-criterion-from-the-killing-form.md) says precisely that $\kappa$ is negative-definite. A compact algebra with a nonzero abelian center has a degenerate [Killing form](../../../../../killing-form.md), so the semisimplicity qualification matters.

For a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), let $\kappa^{ab}$ denote the inverse matrix of $\kappa_{ab}=\kappa(t_a,t_b)$. Its [Casimir operator](../../../../../casimir-element.md) in $d$ is

$$
\boxed{C=\kappa^{ab}d(t_a)d(t_b).}
$$

This contraction is independent of the chosen [basis](../../../../../basis.md). To prove centrality directly, put $[X,t_b]=A^a{}_b t_a$. Invariance gives $A^{\mathsf T}\kappa+\kappa A=0$, hence $A\kappa^{-1}+\kappa^{-1}A^{\mathsf T}=0$. The [Lie algebra representation](../../../../../lie-algebra-representation.md) property and the product rule for a [commutator](../../../../../commutator.md) now give

$$
[d(X),C]=\kappa^{ab}\bigl(A^c{}_a d(t_c)d(t_b)+A^c{}_b d(t_a)d(t_c)\bigr)=0.
$$

Indeed, the coefficient of $d(t_c)d(t_b)$ in this expression is $(A\kappa^{-1}+\kappa^{-1}A^{\mathsf T})^{cb}$. Thus **$[d(X),C]=0$ for every $X$**. No irreducibility of $d$ is required.

The [matrix units](../../../../../matrix-unit.md) obey $E_{ij}E_{pq}=\delta_{jp}E_{iq}$. Consequently the [general linear Lie algebra](../../../../../general-linear-lie-algebra.md) $\mathcal M=\mathfrak{gl}_n(\mathbb R)$ has

$$
\boxed{[E_{ij},E_{pq}]=\delta_{jp}E_{iq}-\delta_{qi}E_{pj},\qquad c_{ij,pq}{}^{mn}=\delta_{jp}\delta_i^m\delta_q^n-\delta_{qi}\delta_p^m\delta_j^n.}
$$

For its [Killing form](../../../../../killing-form.md), write $L_X(Z)=XZ$ and $R_X(Z)=ZX$, so that $\operatorname{ad}_X=L_X-R_X$. Left multiplication acts identically on each of the $n$ columns, and right multiplication identically on each of the $n$ rows. Thus $\operatorname{Tr}(L_XL_Y)=\operatorname{Tr}(R_XR_Y)=n\operatorname{tr}(XY)$. The diagonal coefficient of $L_XR_Y$ on $E_{ij}$ is $X_{ii}Y_{jj}$, giving $\operatorname{Tr}(L_XR_Y)=\operatorname{tr}X\operatorname{tr}Y$; the other mixed trace is identical. This proves the [Killing form of the general linear Lie algebra](../../../../../killing-form-of-the-general-linear-lie-algebra.md):

$$
\kappa(X,Y)=2n\operatorname{tr}(XY)-2\operatorname{tr}X\operatorname{tr}Y,\qquad \boxed{\kappa_{ij,pq}=2n\delta_{jp}\delta_{iq}-2\delta_{ij}\delta_{pq}.}
$$

The scalar matrices form a nonzero central abelian ideal, so **$\mathcal M$ is not semisimple for any $n\ge1$**. More explicitly, the [radical of the Killing form](../../../../../radical-of-the-killing-form.md) is $\mathbb RI$, since vanishing against every $Y$ forces $nX-(\operatorname{tr}X)I=0$ by nondegeneracy of the trace pairing. For $n\ge2$, take $H=E_{11}-E_{22}$. Then $\kappa(H,H)=4n>0$, whereas a positive-definite invariant inner product would make every adjoint map skew and hence give $\kappa(X,X)\le0$. Therefore **$\mathcal M$ is not compact when $n\ge2$**. For the allowed exceptional value $n=1$, the abstract abelian algebra $\mathbb R$ is a [compact Lie algebra](../../../../../compact-lie-algebra.md), being isomorphic to the algebra of $U(1)$; the particular matrix group $GL_1(\mathbb R)$ is nevertheless noncompact. This distinguishes compactness of an algebra from that of a chosen group realizing it.

For the final algebra, the printed basis specifies [strictly upper triangular matrices](../../../../../strictly-upper-triangular-matrix.md). If $i<j$ and $p<q$, the first term in $[E_{ij},E_{pq}]$ can be nonzero only when $i<j=p<q$, and then $E_{iq}$ is strictly upper triangular; the second can be nonzero only when $p<q=i<j$, and then $E_{pj}$ is strictly upper triangular. Bilinearity proves closure under the [Lie bracket](../../../../../lie-bracket.md). To compute its own [Killing form](../../../../../killing-form.md), grade $E_{ij}$ by the positive integer $j-i$. Bracketing with any basis element increases that degree whenever the result is nonzero. In a basis ordered by degree, all adjoint maps are strictly triangular, as are their products. Every such product has zero trace, so the [Killing form of a nilpotent Lie algebra vanishes](../../../../../killing-form-of-a-nilpotent-lie-algebra-vanishes.md) here. Therefore the subspace denoted by a prime in the PDF is

$$
\boxed{\mathcal L'=\mathcal L,\qquad \dim\mathcal L'=\frac{n(n-1)}2.}
$$

This is the defined [radical of the Killing form](../../../../../radical-of-the-killing-form.md), not the derived algebra; for $n=1$ both $\mathcal L$ and this radical are zero.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 52](../../paper-52-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
