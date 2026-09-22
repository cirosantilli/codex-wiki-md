<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the [affine variety](../../../../../affine-algebraic-set.md) as $X=\operatorname{Spec}A$. Its coordinate ring is [Noetherian](../../../../../noetherian-ring.md), and a [coherent sheaf](../../../../../coherent-sheaf.md) is $\mathcal F=\widetilde M$ for a finitely generated $A$-module $M$. We first justify the acyclic resolution used to compute its [sheaf cohomology](../../../../../sheaf-cohomology.md).

If $I$ is an [injective module](../../../../../injective-module.md), then $\widetilde I$ is a [flasque sheaf](../../../../../flasque-sheaf.md). Indeed every open $U$ in this [Noetherian scheme](../../../../../noetherian-scheme.md) has the form $X\setminus V(\mathfrak a)$ for a finitely generated ideal. Clearing denominators gives

$$
\Gamma(U,\widetilde I)=\varinjlim_n\operatorname{Hom}_A(\mathfrak a^n,I).
$$

Here a homomorphism $h:\mathfrak a^n\to I$ gives, on a principal open $D(f)$ with $f\in\mathfrak a$, the fraction $h(f^n)/f^n$; the fractions agree on overlaps. Conversely choose fractions for a section on a finite principal-open cover. A common power clears their denominators and the finitely many compatibility relations. Multiplication by a further power of $\mathfrak a$ kills any elements supported on $V(\mathfrak a)$, producing a well-defined map on some $\mathfrak a^n$. Changing that power accounts for the direct limit. This is the [sheafification of an injective module is flasque](../../../../../sheafification-of-an-injective-module-is-flasque.md) construction. Since $I$ is injective, each map $\mathfrak a^n\to I$ extends to $A\to I$. Thus every section on every open extends to $X$. Extending globally and restricting again also proves surjectivity for restrictions between arbitrary opens.

Choose an [injective module](../../../../../injective-module.md) resolution $0\to M\to I^0\to I^1\to\cdots$. Localization is exact, so sheafifying gives a [flasque resolution](../../../../../flasque-resolution.md) of $\mathcal F$. Its global-section complex is exactly $I^\bullet$, since $\Gamma(\operatorname{Spec}A,\widetilde I)=I$. This complex is exact in positive degrees, and a [flasque resolution](../../../../../flasque-resolution.md) computes [sheaf cohomology](../../../../../sheaf-cohomology.md). Consequently

$$
\boxed{H^i(X,\mathcal F)=0\quad(i\ge1).}
$$

The argument actually proves [vanishing of quasi-coherent cohomology on an affine scheme](../../../../../vanishing-of-quasi-coherent-cohomology-on-an-affine-scheme.md), without finite generation of $M$.

For the intersection assertion, varieties are taken to be separated, as usual. The [diagonal morphism](../../../../../diagonal-morphism.md) $X\to X\times_kX$ is a [closed immersion](../../../../../closed-immersion.md). Its inverse image over $U\times_kV$ identifies $U\cap V$ with a closed subvariety of the [affine variety](../../../../../affine-algebraic-set.md) $U\times_kV$. A closed subvariety of an [affine variety](../../../../../affine-algebraic-set.md) is affine: its coordinate ring is the ambient coordinate ring modulo its defining ideal. **Thus $U\cap V$ is affine.** Repeated application gives affine finite intersections. Without [separatedness](../../../../../separated-morphism.md) this statement need not hold.

Choose a finite affine [open cover](../../../../../open-cover.md) $(U_\alpha)$ of the [projective variety](../../../../../projective-variety.md) $X$. For ordered indices write $U_{\alpha_0\cdots\alpha_p}=U_{\alpha_0}\cap\cdots\cap U_{\alpha_p}$. The answer is the cohomology of the [Čech cochain complex](../../../../../cech-cochain-complex.md)

$$
C^p=\prod_{\alpha_0<\cdots<\alpha_p}\Gamma(U_{\alpha_0\cdots\alpha_p},\mathcal F),\qquad
(dc)_{\alpha_0\cdots\alpha_{p+1}}=
\sum_{j=0}^{p+1}(-1)^j c_{\alpha_0\cdots\widehat{\alpha_j}\cdots\alpha_{p+1}}|_{U_{\alpha_0\cdots\alpha_{p+1}}}.
$$

In particular $H^0=\ker(C^0\to C^1)$ and, in positive degree,

$$
\boxed{H^i(X,\mathcal F)\cong\ker(d:C^i\to C^{i+1})/\operatorname{im}(d:C^{i-1}\to C^i).}
$$

The chart modules $\Gamma(U_\alpha,\mathcal F)$, together with their restriction and gluing maps, supply the modules on overlaps by localization. The gluing maps are essential; abstract chart modules alone do not specify a [sheaf](../../../../../sheaf-mathematics.md).

For completeness, take a [flasque resolution](../../../../../flasque-resolution.md) $\mathcal F\to\mathcal I^\bullet$ and its double complex of [Čech cochain complexes](../../../../../cech-cochain-complex.md) on this cover. In the resolution direction, its cohomology is $H^q(U_{\alpha_0\cdots\alpha_p},\mathcal F)$, which vanishes for $q>0$ by the affine result. In the cover direction, the augmented [Čech cochain complex](../../../../../cech-cochain-complex.md) of a [flasque sheaf](../../../../../flasque-sheaf.md) is exact: sections can be extended from overlaps, successively adjusting a cocycle to eliminate one cover member at a time. Equivalently the augmented sheaf complex is stalkwise contracted by inserting a cover index containing the point. Thus computing the total cohomology in the two directions identifies [Čech cohomology](../../../../../cech-cohomology.md) with [sheaf cohomology](../../../../../sheaf-cohomology.md), proving the displayed description.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 80](../../paper-80-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
