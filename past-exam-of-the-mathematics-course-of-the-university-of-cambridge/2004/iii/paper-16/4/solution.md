<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an oriented real [vector bundle](../../../../../vector-bundle.md) $\pi:E\to X$ of rank $d$, the [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) gives a unique [Thom class](../../../../../thom-class.md) $u_E\in H^d(D(E),S(E);\mathbb Z)$ restricting to the chosen generator in each fibre, and isomorphisms

$$
H^q(X;\mathbb Z)\xrightarrow{\ a\mapsto\pi^*a\smile u_E\ }H^{q+d}(D(E),S(E);\mathbb Z).
$$

Equivalently use the pair $(E,E\setminus X)$, identifying $X$ with the [zero section](../../../../../zero-section-of-a-vector-bundle.md). After forgetting relative supports, pull the [Thom class](../../../../../thom-class.md) back along the [zero section](../../../../../zero-section-of-a-vector-bundle.md) $s$ to define the [Euler class](../../../../../euler-class-of-a-vector-bundle.md):

$$
\boxed{e(E)=s^*u_E\in H^d(X;\mathbb Z).}
$$

In this expression the relative class is first mapped to absolute [cohomology](../../../../../cohomology-split.md).

A compact embedded [submanifold](../../../../../submanifold.md) equipped with a [coorientation](../../../../../coorientation.md) $Y\subset X$ has an oriented [normal bundle](../../../../../normal-bundle.md) $\nu_Y$ of rank $d$. A [tubular neighborhood](../../../../../tubular-neighborhood.md) and [excision](../../../../../excision-theorem.md) identify its [Thom class](../../../../../thom-class.md) with a class $u_Y\in H^d(X,X\setminus Y)$. Its image in $H^d(X)$ is the [cohomology class of a cooriented submanifold](../../../../../cohomology-class-of-a-cooriented-submanifold.md) $\varepsilon_Y$. In particular it restricts to zero on $X\setminus Y$. If the ambient manifold is oriented, orient $Y$ by the normal-first convention. The class is its [Poincare dual](../../../../../poincare-dual.md), characterized by

$$
\langle\varepsilon_Y\smile\alpha,[X]\rangle=\langle\alpha|_Y,[Y]\rangle
$$

for the appropriate complementary degree. This is the stated integration identity in cohomological notation.

First prove the [Lefschetz fixed-point theorem](../../../../../lefschetz-fixed-point-theorem.md) for an oriented closed n-manifold $X$. Orient its diagonal by the identification $\Delta\cong X$, and choose the normal [orientation](../../../../../orientation-of-a-simplex.md) so this agrees with the normal-first convention in the product. This produces the integral class $\varepsilon_\Delta$. To compute the part that contributes to the [trace](../../../../../matrix-trace.md), tensor with $\mathbb Q$: the [trace](../../../../../matrix-trace.md) on a finitely generated integral [cohomology](../../../../../cohomology-split.md) group means its [trace](../../../../../matrix-trace.md) on the free quotient, equivalently on rational [cohomology](../../../../../cohomology-split.md); torsion contributes nothing.

Choose a basis $e_{p,j}$ of $H^p(X;\mathbb Q)$ and its [Poincare duality pairing](../../../../../poincare-duality-pairing.md) dual basis $e_{p,j}^{\vee}\in H^{n-p}(X;\mathbb Q)$, normalized by $\langle e_{p,i}\smile e_{p,j}^{\vee},[X]\rangle=\delta_{ij}$. The rational image of the [cohomology class of the diagonal](../../../../../cohomology-class-of-the-diagonal.md) is

$$
\boxed{\varepsilon_\Delta=\sum_{p,j}(-1)^{np}\,e_{p,j}^{\vee}\times e_{p,j}.}
$$

Indeed, pairing this expression against $\alpha\times\beta$ with degrees $p,n-p$ picks out the p-summands. The cross-product multiplication contributes $(-1)^{p^2}$ and moving $\alpha$ past $e_{p,j}^{\vee}$ contributes $(-1)^{p(n-p)}$. Together with $(-1)^{np}$ their product is $+1$. The result is $\langle\alpha\smile\beta,[X]\rangle$, exactly the diagonal's defining identity. The rational [Künneth theorem](../../../../../kunneth-theorem.md) and nondegeneracy of the duality pairing determine the class. An integral torsion component, if present, is not determined by this rational expression and does not affect any evaluation below.

For the graph map $\Gamma_f=(1,f):X\to X\times X$, write $f^*e_{p,j}=\sum_iA_{ij}e_{p,i}$. Pulling back the expression and evaluating gives the [graph-diagonal formula for the Lefschetz number](../../../../../graph-diagonal-formula-for-the-lefschetz-number.md):

$$
\begin{aligned}
\langle\Gamma_f^*\varepsilon_\Delta,[X]\rangle
&=\sum_{p,j}(-1)^{np}\langle e_{p,j}^{\vee}\smile f^*e_{p,j},[X]\rangle\\
&=\sum_p(-1)^{np+p(n-p)}\operatorname{tr}A_p
=\sum_p(-1)^p\operatorname{tr}(f^*:H^p(X;\mathbb Q)\to H^p(X;\mathbb Q))=L(f).
\end{aligned}
$$

If $f$ has no fixed point, its graph lies in $(X\times X)\setminus\Delta$. The relative [Thom class](../../../../../thom-class.md) restricts to zero there, so $\Gamma_f^*\varepsilon_\Delta=0$ and $L(f)=0$. The contrapositive proves the required fixed-point assertion, without requiring smoothness of $f$ or transversality of its graph.

The printed hypothesis does not require $X$ to be orientable. For a nonorientable $X$, the diagonal's [normal bundle](../../../../../normal-bundle.md) is $TX$, so an ordinary integral coorientation cannot be assumed. We extend the proved theorem as follows, rather than apply the untwisted diagonal computation incorrectly. We first construct a [smooth embedding](../../../../../smooth-embedding.md) in Euclidean space using finitely many charts $\chi_i:U_i\to\mathbb R^n$ and smooth functions $\rho_i$ supported in those charts, with at least one $\rho_i(x)>0$ at every point. The map $\Psi(x)=(\rho_i(x),\rho_i(x)\chi_i(x))_i$, with zero extensions, is injective: a positive first coordinate identifies a chart in which its remaining coordinates recover $x$. Its differential is injective as well, since $d\rho_i(v)=0$ and $d(\rho_i\chi_i)(v)=0$ force $d\chi_i(v)=0$ in a chart with $\rho_i>0$. Compactness makes this injective immersion a [homeomorphism](../../../../../homeomorphism.md) onto its image. This [finite-chart Euclidean embedding of a compact smooth manifold](../../../../../finite-chart-euclidean-embedding-of-a-compact-smooth-manifold.md), enlarged by zero coordinates if necessary, has positive codimension. A compact tubular disc neighbourhood $W$ is an oriented N-manifold with boundary, inheriting its [orientation](../../../../../orientation-of-a-simplex.md) from the ambient Euclidean space. Its [double of a manifold](../../../../../double-of-a-manifold.md) $M$ is closed and oriented. Projection of each copy of $W$ to $X$ agrees on their common boundary, giving $r:M\to X$; inclusion into the first copy gives $i:X\to M$ with $ri=1_X$.

Set $F=ifr$. A fixed point of $F$ must lie in $i(X)$, and then is exactly the image of a fixed point of $f$. Moreover $F^*=r^*f^*i^*$, and cyclicity of [trace](../../../../../matrix-trace.md) for maps between finite-dimensional rational [cohomology groups](../../../../../cohomology-group.md) gives

$$
\operatorname{tr}(r^*f^*i^*)=\operatorname{tr}(f^*i^*r^*)=\operatorname{tr}(f^*)
$$

in each degree, because $i^*r^*=1$. Thus $L(F)=L(f)$. The oriented theorem for $M$ now gives a fixed point of $F$, hence of $f$, whenever $L(f)\ne0$. This [oriented manifold retract for the Lefschetz theorem](../../../../../oriented-manifold-retract-for-the-lefschetz-theorem.md) proves the full printed result. The double construction also works componentwise if necessary.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
