<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Interpretation of the removed locus.** Over $\mathbb Z$, the notation $[1:0:0]$ specifies a section $\operatorname{Spec}\mathbb Z\to\mathbb P^2_{\mathbb Z}$, with image $V_+(x_1,x_2)\cong\operatorname{Spec}\mathbb Z$. We remove this entire [closed subscheme](../../../../closed-subscheme.md). This is the interpretation forced by the asserted [open cover](../../../../open-cover.md) $X=U_1\cup U_2$. Removing one closed point in a particular fiber would not give that [open cover](../../../../open-cover.md). The native PDF uses the same notation as the transcription.

Put $a=x_0/x_1$, $b=x_2/x_1$ on $U_1$. On $U_2$ put $c=x_0/x_2$, $d=x_1/x_2$. On their intersection $c=a/b$ and $d=b^{-1}$, giving [coordinate rings](../../../../coordinate-ring.md)

$$
\Gamma(U_1,\mathcal O_X)=\mathbb Z[a,b],\qquad
\Gamma(U_2,\mathcal O_X)=\mathbb Z[a/b,b^{-1}],\qquad
\Gamma(U_1\cap U_2,\mathcal O_X)=L:=\mathbb Z[a,b,b^{-1}].
$$

The [Čech cochain complex](../../../../cech-cochain-complex.md) for the [structure sheaf](../../../../structure-sheaf-of-a-scheme.md), using increasing distinct indices, is

$$
0\longrightarrow\mathbb Z[a,b]\oplus\mathbb Z[a/b,b^{-1}]
\xrightarrow{\delta}L\longrightarrow0,\qquad
\delta(f,g)=g-f.
$$

Thus $\check H^0$ is the intersection of the two subrings of $L$, while $\check H^1$ is the [quotient module](../../../../quotient-module.md) of $L$ by their additive sum.

The [Laurent polynomial ring](../../../../laurent-polynomial-ring.md) $L$ is a free [abelian group](../../../../abelian-group.md) on the [monomials](../../../../monomial.md) $a^ib^j$ with $i\geq0$, $j\in\mathbb Z$. The first subring has the [basis](../../../../basis.md) $j\geq0$. The second has the [basis](../../../../basis.md)

$$
c^id^k=a^ib^{-i-k},\qquad i,k\geq0,
$$

so its allowed exponents satisfy $j\leq-i$. A [monomial](../../../../monomial.md) belongs to both precisely when $i=j=0$. The [monomials](../../../../monomial.md) belonging to neither satisfy $i\geq2$ and $-i<j<0$. Since the subgroups are spanned by subsets of the same [basis](../../../../basis.md), their sum introduces no other relations. Therefore

$$
\boxed{\begin{aligned}
\check H^0(\{U_1,U_2\},\mathcal O_X)&=\mathbb Z,\\
\check H^1(\{U_1,U_2\},\mathcal O_X)&=\bigoplus_{i\geq2}\ \bigoplus_{k=1}^{i-1}\mathbb Z\,[a^ib^{-k}]\\
&=\bigoplus_{m,n\geq1}\mathbb Z\!\left[\frac{x_0^{m+n}}{x_1^mx_2^n}\right],\\
\check H^q(\{U_1,U_2\},\mathcal O_X)&=0\qquad(q\geq2).
\end{aligned}}
$$

Here the square brackets denote [cohomology classes](../../../../cohomology-class.md), and the [direct sums](../../../../direct-sum.md) are as [abelian groups](../../../../abelian-group.md). In particular, $[a^2b^{-1}]=[x_0^2/(x_1x_2)]$ is a nonzero [cohomology class](../../../../cohomology-class.md). This [scheme](../../../../scheme.md) is a [separated scheme](../../../../separated-scheme.md), being an [open subscheme](../../../../open-subscheme.md) of [projective space](../../../../projective-space-split.md) over $\mathbb Z$, and is a [quasi-compact scheme](../../../../quasi-compact-scheme.md) by (d). Both charts and their intersection are [affine schemes](../../../../affine-scheme.md), so this [Čech cohomology](../../../../cech-cohomology.md) equals [sheaf cohomology](../../../../sheaf-cohomology.md). The nonzero first [sheaf cohomology](../../../../sheaf-cohomology.md) of the [quasi-coherent](../../../../quasi-coherent-sheaf.md) [structure sheaf](../../../../structure-sheaf-of-a-scheme.md) rules out an [affine scheme](../../../../affine-scheme.md):

$$
\boxed{X\text{ is not affine}.}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
