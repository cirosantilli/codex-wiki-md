<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

All [cohomology](../../../../../cohomology-split.md) below has rational coefficients. First describe the incidence space geometrically. The image of $g$ is $\mathbb P(W)\cong\mathbb {CP}^1$, inside $\operatorname{Gr}(1,4)\cong\mathbb {CP}^3$. For a line $U\subset W$, choosing a plane $V$ containing $U$ is equivalent to choosing the line $V/U$ in $\mathbb C^4/U$. If $\mathcal L$ is the tautological line bundle on $\mathbb P(W)$, then

$$
F_W\cong\mathbb P\big((\mathbb P(W)\times\mathbb C^4)/\mathcal L\big).
$$

This is the [projective bundle](../../../../../projective-bundle.md) of a rank-three quotient bundle, with fibre $\mathbb {CP}^2$. Local frames of the quotient bundle give local product charts. In particular $F_W$ is an oriented real six-dimensional [manifold](../../../../../topological-manifold.md).

For $V\in S_W\setminus\{W\}$, the intersection $V\cap W$ is exactly a line, so $f^{-1}(V)$ is a single point and the inverse map is $V\mapsto(V\cap W,V)$. The intersection line varies continuously, indeed holomorphically, wherever its dimension is constant: in local [Grassmannian](../../../../../grassmannian.md) charts it is the kernel of a matrix of constant rank, whose kernel bases can be chosen locally. Thus $f$ is an isomorphism over the open stratum. At the remaining point,

$$
\boxed{f^{-1}(W)=\mathbb P(W)\cong\mathbb {CP}^1.}
$$

Set $K=Rf_*\mathbb Q_{F_W}$, a [derived direct image of sheaves](../../../../../derived-direct-image-of-sheaves.md). The [proper base change for sheaves](../../../../../proper-base-change-for-sheaves.md) theorem identifies its derived stalks with the [cohomology](../../../../../cohomology-split.md) complexes of the fibres. Consequently $K$ is the constant rational [sheaf](../../../../../sheaf-mathematics.md) in degree zero on $S_W\setminus\{W\}$, and

$$
H^a(i_W^*K)=\begin{cases}\mathbb Q,&a=0,2,\\0,&a\ne0,2.\end{cases}
$$

The [cohomology sheaves](../../../../../cohomology-sheaf.md) are therefore finite-rank [local systems](../../../../../local-system.md) on the two strata, with no other nonzero degrees. This proves that $K$ is a [constructible complex of sheaves](../../../../../constructible-complex-of-sheaves.md) and verifies normalization. The open stratum has real dimension six, so the isolated point has codimension six. Its middle [perversity](../../../../../perversity.md) is $\bar m(6)=2$, and the [intersection-complex support and cosupport axioms](../../../../../intersection-complex-support-and-cosupport-axioms.md) require stalk vanishing in degrees above two. The fibre calculation verifies the support axiom, as well as vanishing in negative degrees.

For an oriented real six-dimensional [manifold](../../../../../topological-manifold.md), [Verdier duality](../../../../../verdier-duality.md) gives $D_{F_W}\mathbb Q_{F_W}\cong\mathbb Q_{F_W}[6]$. For a [proper map](../../../../../proper-map.md), [Verdier duality](../../../../../verdier-duality.md) commutes with derived direct image. Applying these statements here yields

$$
D_{S_W}K\cong Rf_*D_{F_W}\mathbb Q_{F_W}\cong Rf_*\mathbb Q_{F_W}[6]=K[6],\qquad
\boxed{\Sigma^{-6}D_{S_W}K\cong K.}
$$

The duality identity $i_W^!D_{S_W}K\cong D_{\{W\}}i_W^*K$ converts this into

$$
H^a(i_W^!K)\cong H^{6-a}(i_W^*K)^*.
$$

Here $i_W^!K$ is the [costalk](../../../../../costalk.md), and dualization of rational complexes reverses degrees. Thus its only nonzero groups are $\mathbb Q$ in degrees four and six. In particular they vanish for $a\le3$, which is precisely the cosupport axiom at this isolated six-dimensional singularity. The uniqueness characterization by constructibility, normalization, support and cosupport now identifies $K$ with the unshifted [intersection complex](../../../../../intersection-complex.md) of $S_W$. Taking [hypercohomology](../../../../../hypercohomology.md), and using the composition of derived global sections with $Rf_*$, gives

$$
\boxed{IH^*(S_W)\cong\mathbb H^*(S_W,K)\cong H^*(F_W).}
$$

Finally apply the fibration result allowed in the question to $g:F_W\to\mathbb P(W)$. Its base is the simply connected [complex projective line](../../../../../complex-projective-line.md), its fibre is the [Complex projective plane](../../../../../complex-projective-plane.md), and the projective-bundle charts above verify the fibration hypothesis. Hence, as graded rational [vector spaces](../../../../../vector-space-split.md),

$$
\boxed{IH^*(S_W)\cong H^*(\mathbb {CP}^1)\otimes H^*(\mathbb {CP}^2).}
$$

The resulting [Betti numbers](../../../../../betti-number.md) and [Poincaré polynomial](../../../../../poincare-polynomial.md) are

$$
\boxed{\dim IH^i(S_W)=\begin{cases}1,&i=0,6,\\2,&i=2,4,\\0,&\text{otherwise},\end{cases}\qquad P_{IH}(t)=1+2t^2+2t^4+t^6.}
$$

This uses $H^*(\mathbb {CP}^r)=\mathbb Q[h]/(h^{r+1})$ with $\deg h=2$. No assertion that an arbitrary projective fibration has the product [cohomology](../../../../../cohomology-split.md) ring is needed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
