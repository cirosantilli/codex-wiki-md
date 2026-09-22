<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A real [Lie group](../../../../../lie-group.md) is a finite-dimensional real [smooth manifold](../../../../../smooth-manifold.md) with a [group](../../../../../group-split.md) structure whose multiplication and inversion are smooth. Its [tangent space](../../../../../tangent-space.md) at the [identity element](../../../../../identity-element.md) $e$ is the vector space $\mathfrak g=T_eG$ of velocities of smooth curves through $e$. For the [general linear group](../../../../../general-linear-group.md) $\mathrm{GL}_n(\mathbb R)$ it identifies with $M_n(\mathbb R)$. The [matrix exponential](../../../../../matrix-exponential.md) and local [matrix logarithm](../../../../../matrix-logarithm.md) are

$$
\exp X=\sum_{r=0}^\infty\frac{X^r}{r!},\qquad\log(I+A)=\sum_{r=1}^\infty\frac{(-1)^{r+1}A^r}{r}\quad(\|A\|<1).
$$

The exponential is globally defined, and each matrix $\exp X$ is invertible with inverse $\exp(-X)$. The logarithm here is a local map near $I$; it is not a globally defined inverse on every real invertible matrix. The differential of $\exp$ at zero is the identity, and the two power series are inverse locally.

For a general $G$, the assumed [Exponential map of a Lie group](../../../../../exponential-map-of-a-lie-group.md) with $d\exp_0=I$ has a smooth local inverse by the [inverse function theorem](../../../../../inverse-function-theorem.md), giving a [local exponential chart](../../../../../local-exponential-chart.md). Define the [Lie bracket from local group commutators](../../../../../lie-bracket-from-local-group-commutators.md) by

$$
\boxed{[X,Y]=\left.\frac{\partial^2}{\partial s\,\partial t}\right|_{(0,0)}\log\!\left(\exp(sX)\exp(tY)\exp(-sX)\exp(-tY)\right).}
$$

For small $s,t$ the [group commutator](../../../../../group-commutator.md) lies in that chart. More explicitly, the map $F(u,v)=\log(\exp u\exp v\exp(-u)\exp(-v))$ is smooth and has $F(u,0)=F(0,v)=0$. Its mixed second differential at $(0,0)$ is a [bilinear map](../../../../../bilinear-map.md) of $X,Y$, proving bilinearity. Swapping the two group elements inverts the commutator, and $\log(g^{-1})=-\log g$ near $e$. Thus $F(v,u)=-F(u,v)$ and $[Y,X]=-[X,Y]$. In the matrix group, expansion to the mixed term $st$ gives the familiar [commutator](../../../../../commutator.md) $XY-YX$.

For $g\in G$, let $c_g(h)=ghg^{-1}$ and define the [Adjoint representation of a Lie group](../../../../../adjoint-representation-of-a-lie-group.md) by $\operatorname{Ad}_g=d(c_g)_e\in\mathrm{GL}(\mathfrak g)$. It is smooth and satisfies $\operatorname{Ad}_{gh}=\operatorname{Ad}_g\operatorname{Ad}_h$. Its [derived representation](../../../../../derived-representation.md) is $\operatorname{ad}=d(\operatorname{Ad})_e:\mathfrak g\to\operatorname{End}(\mathfrak g)$. Naturality of the [Exponential map of a Lie group](../../../../../exponential-map-of-a-lie-group.md) under conjugation gives

$$
\exp(sX)\exp(tY)\exp(-sX)=\exp\!\left(t\operatorname{Ad}_{\exp(sX)}Y\right).
$$

At $t=0$, the derivative of the logarithm of the commutator is $\operatorname{Ad}_{\exp(sX)}Y-Y$: the derivative of multiplication at $(e,e)$ adds tangent vectors, and $d\log_e=I$. Differentiate in $s$ to conclude

$$
\boxed{\operatorname{ad}(X)Y=[X,Y].}
$$

To prove the [Jacobi identity](../../../../../jacobi-identity.md) without assuming it in the bracket construction, first establish that the [differential of a Lie group homomorphism preserves Lie brackets](../../../../../differential-of-a-lie-group-homomorphism-preserves-lie-brackets.md). For a homomorphism $f:G\to H$, the allowed exponential identity gives $\log_H(f(\exp_Gu))=df_e(u)$ locally. Apply this identity to the group commutator and take the mixed derivative to obtain $df_e([X,Y])=[df_eX,df_eY]$. In particular $f=\operatorname{Ad}:G\to\mathrm{GL}(\mathfrak g)$ gives

$$
\operatorname{ad}[X,Y]=[\operatorname{ad}X,\operatorname{ad}Y].
$$

Applying both sides to $Z$ yields $[[X,Y],Z]=[X,[Y,Z]]-[Y,[X,Z]]$. Rearranging with antisymmetry proves

$$
\boxed{[X,[Y,Z]]+[Y,[Z,X]]+[Z,[X,Y]]=0.}
$$

Neither injectivity of $\operatorname{ad}$ nor the existence of a global logarithm was used.

Finally let $H$ be a normal [Lie subgroup](../../../../../lie-subgroup.md) of $G$, with its corresponding [Lie algebra](../../../../../lie-algebra-split.md) $\mathfrak h\subseteq\mathfrak g$. For each $g\in G$, conjugation restricts to $H$, so its differential preserves $\mathfrak h$: $\operatorname{Ad}_g\mathfrak h=\mathfrak h$. Differentiate along $g=\exp(tX)$ to get $[X,Y]=\operatorname{ad}(X)Y\in\mathfrak h$ for every $X\in\mathfrak g$ and $Y\in\mathfrak h$. Thus **the [Lie algebra of a normal Lie subgroup](../../../../../lie-algebra-of-a-normal-lie-subgroup.md) is an [ideal of a Lie algebra](../../../../../ideal-of-a-lie-algebra.md)**. The assertion concerns a subgroup carrying the corresponding Lie-subgroup structure, for example any closed subgroup; no arbitrary abstract subgroup is being assigned a tangent space.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
