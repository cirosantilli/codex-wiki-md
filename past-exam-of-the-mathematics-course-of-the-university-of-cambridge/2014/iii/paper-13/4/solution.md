<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Order the index set of the [open cover](../../../../../open-cover.md) $\mathcal U=(U_a)$. The [Čech cochain groups](../../../../../cech-cochain-group.md) are

$$
\check C^p(\mathcal U,\mathcal F)=\prod_{a_0<\cdots<a_p}\mathcal F(U_{a_0}\cap\cdots\cap U_{a_p}),
$$

and their differential is the alternating sum of restrictions:

$$
(\delta c)_{a_0\ldots a_{p+1}}=\sum_{j=0}^{p+1}(-1)^j c_{a_0\ldots\widehat a_j\ldots a_{p+1}}|_{U_{a_0}\cap\cdots\cap U_{a_{p+1}}}.
$$

Terms obtained by deleting two indices cancel in pairs, so $\delta^2=0$. The [Čech cohomology](../../../../../cech-cohomology.md) is $\check H^p=\ker\delta/\operatorname{im}\delta$, with zero incoming differential in degree zero. Its zeroth group is the group of [global sections](../../../../../global-section.md) by [sheaf](../../../../../sheaf-mathematics.md) gluing.

The [acyclic cover theorem](../../../../../leray-s-theorem.md) applies if every nonempty finite intersection is acyclic for $\mathcal F$. For a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) on a variety it is sufficient that every such intersection is affine; on a separated variety, any affine [open cover](../../../../../open-cover.md) has this property. On $\mathbb P^n$, take the $n+1$ standard charts $U_i=D_+(X_i)$. Every intersection is a principal open in an affine chart, hence affine. The Čech complex has no terms above degree $n$, proving

$$
\boxed{H^i(\mathbb P^n,\mathcal F)=0\quad(i>n).}
$$

This is the [cohomological dimension bound from an affine cover](../../../../../cohomological-dimension-bound-from-an-affine-cover.md) and requires only quasi-coherence, not finite generation.

For the remaining projective calculations assume $n\ge1$. There is a necessary zero-dimensional exception to the negative-twist assertion: $\mathbb P^0$ is a point, every twist is trivial there, and $H^0(\mathbb P^0,\mathcal O(m))\cong k$ even for $m<0$.

Put $S=k[X_0,\ldots,X_n]$ with its usual grading. The [twisting sheaf on projective space](../../../../../twisting-sheaf-on-projective-space.md) is the [sheaf](../../../../../sheaf-mathematics.md) associated with the shifted graded [module](../../../../../module-mathematics.md) $S(m)$; on an intersection $U_I=\bigcap_{i\in I}U_i$ its sections are

$$
\mathcal O(m)(U_I)=(S_{\prod_{i\in I}X_i})_m.
$$

On $U_i$ a generator is $e_i=X_i^m$, with transition $e_j=(X_j/X_i)^m e_i$. These are regular units on overlaps and satisfy the cocycle relation, so they glue an [invertible sheaf](../../../../../line-bundle.md) for every integer $m$, including negative $m$.

A [global section](../../../../../global-section.md) is a compatible family of these homogeneous fractions, hence a single element of degree $m$ in $\bigcap_iS_{X_i}\subseteq\operatorname{Frac}S$. For $n\ge1$, $X_0$ and $X_1$ are relatively prime in the [unique factorization domain](../../../../../unique-factorization-domain.md) $S$, so $S_{X_0}\cap S_{X_1}=S$; therefore the full intersection is $S$. It follows that

$$
\boxed{H^0(\mathbb P^n,\mathcal O(m))\cong S_m=\begin{cases}
\text{homogeneous polynomials of degree }m,&m\ge0,\\
0,&m<0.
\end{cases}}
$$

For $m\ge0$ its dimension is $\binom{n+m}{n}$. The proof uses all-chart compatibility; regularity on one chart alone would permit poles on its complement.

If some $d_i=0$, the ideal $(X_i^{d_i})$ contains $1$, so the requested containment is immediate. Otherwise every $d_i\ge1$. A [monomial](../../../../../monomial.md) $X_0^{a_0}\cdots X_n^{a_n}$ of degree $\sum_id_i$ must have $a_i\ge d_i$ for some $i$: if not, its total degree would be at most $\sum_i(d_i-1)<\sum_id_i$. Thus every degree-$\sum_id_i$ [monomial](../../../../../monomial.md), and hence every [homogeneous polynomial](../../../../../homogeneous-polynomial.md) of that degree, belongs to $(X_0^{d_0},\ldots,X_n^{d_n})$. This is [monomial containment in an ideal of coordinate powers](../../../../../monomial-containment-in-an-ideal-of-coordinate-powers.md).

For $n>0$, a top-degree Čech cochain for $\mathcal O$ is a degree-zero Laurent [polynomial](../../../../../polynomial-split.md) on the full intersection. Write it with a common denominator as

$$
\frac{P}{X_0^{d_0}\cdots X_n^{d_n}},\qquad \deg P=\sum_i d_i.
$$

The containment just proved gives $P=\sum_iQ_iX_i^{d_i}$, with homogeneous $Q_i$ of degree $\sum_jd_j-d_i$. Consequently

$$
\frac P{\prod_jX_j^{d_j}}=\sum_i\frac{Q_i}{\prod_{j\ne i}X_j^{d_j}}.
$$

The $i$th term is regular on the intersection omitting $U_i$, and has degree zero. Give it the sign $(-1)^i$ in that component of the preceding Čech cochain. Its coboundary is the original fraction. Every top cochain is thus a coboundary, and

$$
\boxed{H^n(\mathbb P^n,\mathcal O)=0\quad(n>0).}
$$

This is [top Čech cohomology from missing-denominator monomials](../../../../../laurent-monomial-description-of-top-cohomology-on-projective-space.md).

To obtain the negative-twist bound by induction on dimension, let $H\cong\mathbb P^{n-1}$ be a hyperplane, with inclusion $j$. Its equation gives the [hyperplane exact sequence for twisting sheaves](../../../../../hyperplane-exact-sequence-for-twisting-sheaves.md)

$$
0\longrightarrow\mathcal O(m-1)\longrightarrow\mathcal O(m)\longrightarrow j_*\mathcal O_H(m)\longrightarrow0.
$$

The associated [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) and [sheaf cohomology under a closed inclusion](../../../../../sheaf-cohomology-under-a-closed-inclusion.md) give

$$
H^{n-1}(H,\mathcal O_H(m))\longrightarrow H^n(\mathbb P^n,\mathcal O(m-1))\longrightarrow H^n(\mathbb P^n,\mathcal O(m))\longrightarrow0.
$$

For $n=1$, restriction $H^0(\mathbb P^1,\mathcal O)\to H^0(H,\mathcal O_H)$ is the surjection $k\to k$. Exactness and the already proved $H^1(\mathbb P^1,\mathcal O)=0$ give $H^1(\mathbb P^1,\mathcal O(-1))=0$. The displayed surjections then give the same vanishing for every $m\ge0$. This handles the point hyperplane without making a false negative-twist claim on $\mathbb P^0$.

For $n\ge2$, the induction hypothesis in dimension $n-1$ gives $H^{n-1}(H,\mathcal O_H(m))=0$ whenever $m\ge-(n-1)$. Therefore consecutive top-degree groups are isomorphic for $m\ge1-n$. Starting with $H^n(\mathbb P^n,\mathcal O)=0$ and stepping down through $m=0,-1,\ldots,1-n$ reaches $H^n(\mathbb P^n,\mathcal O(-n))=0$. Stepping upward proves all positive twists too. We conclude

$$
\boxed{H^n(\mathbb P^n,\mathcal O(-r))=0\quad\text{for all integers }r\le n,\ n>0.}
$$

This is [top-twist vanishing by hyperplane induction](../../../../../top-twist-vanishing-by-hyperplane-induction.md).

Finally, on $U_0$ write $x_a=X_a/X_0$ and $\omega_0=dx_1\wedge\cdots\wedge dx_n$. On $U_i$, let $\omega_i$ be the wedge of $d(X_a/X_i)$ for $a\ne i$, taken in increasing index order. For $i>0$, differentiating $X_0/X_i=x_i^{-1}$ and $X_a/X_i=x_a/x_i$ gives

$$
\boxed{\omega_i=(-1)^i x_i^{-n-1}\omega_0.}
$$

In the wedge, all terms involving a second copy of $dx_i$ disappear; the surviving powers are $x_i^{-2}$ from $d(x_i^{-1})$ and $x_i^{-1}$ from the other $n-1$ differentials. Moving $dx_i$ into its original position produces the stated sign. Rescale each local generator by $\eta_i=(-1)^i\omega_i$. Then $\eta_j=(X_j/X_i)^{-n-1}\eta_i$ on every overlap, exactly the transition of the twist with $m=-n-1$. This [canonical-form transition on projective space](../../../../../canonical-form-transition-on-projective-space.md) proves the [canonical bundle of projective space](../../../../../canonical-bundle-of-projective-space.md):

$$
\boxed{\Omega^n_{\mathbb P^n}\cong\mathcal O_{\mathbb P^n}(-n-1).}
$$

For line bundles the [Serre duality](../../../../../serre-duality.md) pairing becomes

$$
H^i(\mathbb P^n,\mathcal O(m))^*\cong H^{n-i}(\mathbb P^n,\mathcal O(-m-n-1)).
$$

In particular $H^n(\mathcal O(-r))$ is dual to $H^0(\mathcal O(r-n-1))$, which is zero for $r\le n$, precisely the independently obtained bound. The case $r=0$ recovers $H^n(\mathcal O)=0$, and $H^n(\mathcal O(-n-1))\cong k$ matches $H^0(\mathcal O)\cong k$. Thus the calculated transition functions, [global sections](../../../../../global-section.md) and top-degree vanishing agree with [Serre duality](../../../../../serre-duality.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
