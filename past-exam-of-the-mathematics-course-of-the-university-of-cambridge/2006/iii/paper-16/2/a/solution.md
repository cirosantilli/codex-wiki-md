<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work first over $\mathbb F_2$. The [mod-two cohomology ring of real projective space](../../../../../../mod-two-cohomology-ring-of-real-projective-space.md) is $H^*(\mathbb{RP}^n;\mathbb F_2)=\mathbb F_2[a]/(a^{n+1})$, with $|a|=1$. A map missing a point has zero [mod-two degree of a map between closed manifolds](../../../../../../mod-two-degree-of-a-map-between-closed-manifolds.md), so $f^*(a^n)=0$. The group in degree one has only two elements, so $f^*a$ is either zero or $a$. The latter would imply $f^*(a^n)=(f^*a)^n=a^n\ne0$, a contradiction. Therefore $f^*a=0$, and multiplicativity makes $f^*$ zero in every positive cohomological degree. Duality of [homology](../../../../../../homology-split.md) and [cohomology](../../../../../../cohomology-split.md) over a field consequently makes $f_*$ zero in every positive degree with mod-two coefficients.

For integral coefficients, [cellular homology of real projective space](../../../../../../cellular-homology-of-real-projective-space.md) gives $H_k\cong\mathbb Z/2$ in odd degrees $0<k<n$, zero in even degrees $0<k<n$, and a top group $\mathbb Z$ if $n$ is odd and zero if $n$ is even. For each torsion group, the natural reduction map to mod-two [homology](../../../../../../homology-split.md) is injective by the [universal coefficient theorem for homology](../../../../../../universal-coefficient-theorem-for-homology.md); naturality and the preceding vanishing imply that its integral induced map is zero. When $n$ is odd, the integral top-degree map is also zero because the nonsurjective map has integer [degree of a map between oriented manifolds](../../../../../../degree-of-a-map-between-oriented-manifolds.md) zero. All groups above dimension $n$ vanish. Hence **$f_*$ is zero on all positive integral [homology](../../../../../../homology-split.md) groups** as well.

For $n\ge2$, $\pi_1(\mathbb{RP}^n)=\mathbb Z/2$, and its [abelianization](../../../../../../abelianization.md) is already $H_1(\mathbb{RP}^n;\mathbb Z)$. The vanishing just proved therefore implies $f_*\pi_1=0$. By the [lifting criterion for a covering space](../../../../../../lifting-criterion-for-a-covering-space.md), $f$ lifts through the double [covering space](../../../../../../covering-space.md) $q:S^n\to\mathbb{RP}^n$ to a map $\widetilde f:\mathbb{RP}^n\to S^n$ with $q\widetilde f=f$.

Choose a point $y$ missed by $f$. Both points of $q^{-1}(y)$ are missed by $\widetilde f$. In particular the lift has image in $S^n\setminus\{z\}\cong\mathbb R^n$, for either such point $z$. This punctured sphere is [contractible](../../../../../../contractible-space.md), so contraction there gives a [homotopy](../../../../../../homotopy.md) from $\widetilde f$ to a constant map into $S^n$. Composing with $q$ contracts $f$. Thus

$$
\boxed{f\simeq\text{constant}.}
$$

This proves the [nonsurjective self-map of real projective space is null-homotopic](../../../../../../nonsurjective-self-map-of-real-projective-space-is-null-homotopic.md) conclusion, and also shows that all positive-degree induced maps vanish with any coefficients.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
