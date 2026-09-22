<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [irreducible scheme](../../../../../irreducible-scheme.md) is a nonempty [scheme](../../../../../scheme.md) whose underlying [topological space](../../../../../topological-space.md) cannot be expressed as the union of two proper closed subsets. Equivalently, any two nonempty [open subsets](../../../../../open-set.md) meet. A [reduced scheme](../../../../../reduced-scheme.md) is one whose [local rings](../../../../../local-ring.md) have no nonzero [nilpotent elements](../../../../../nilpotent.md). Equivalently, every [affine open subscheme](../../../../../affine-open-subscheme.md) has a [reduced ring](../../../../../reduced-ring.md) of [regular functions](../../../../../regular-function.md). We may define an [integral scheme](../../../../../integral-scheme.md) as a nonempty [scheme](../../../../../scheme.md) for which the [coordinate ring](../../../../../coordinate-ring.md) of every nonempty [affine open subscheme](../../../../../affine-open-subscheme.md) is an [integral domain](../../../../../integral-domain.md). We shall show that this is equivalent to being reduced and irreducible. The nonempty convention matters: the empty [scheme](../../../../../scheme.md) is reduced but is not irreducible or integral.

For a [commutative ring](../../../../../commutative-ring.md) $A$, the [spectrum of a ring](../../../../../spectrum-of-a-commutative-ring.md) is reduced exactly when $A$ is a [reduced ring](../../../../../reduced-ring.md). One direction follows since [localization](../../../../../localization-of-a-ring.md) preserves reducedness. Conversely, if $a$ is a nonzero [nilpotent element](../../../../../nilpotent.md), choose a [prime ideal](../../../../../prime-ideal.md) containing its proper annihilator. Then $a/1$ cannot vanish at that [localization](../../../../../localization-of-a-ring.md), contradicting reducedness of its [local ring](../../../../../local-ring.md).

The [spectrum of a ring](../../../../../spectrum-of-a-commutative-ring.md) is irreducible exactly when its [nilradical](../../../../../nilradical.md) $N=\sqrt{(0)}$ is a [prime ideal](../../../../../prime-ideal.md). To see the essential implication directly, if $ab\in N$, then $D(a)\cap D(b)=D(ab)$ is empty. Irreducibility forces $D(a)$ or $D(b)$ to be empty, hence $a\in N$ or $b\in N$. Also $N$ is proper because the spectrum is nonempty. Conversely, if $N$ is a [prime ideal](../../../../../prime-ideal.md), the point $N$ has closure $V(N)=\operatorname{Spec}A$, so the spectrum is irreducible. Combining the two criteria gives

$$
\boxed{A\text{ is an integral domain}
\iff\operatorname{Spec}A\text{ is reduced and irreducible}.}
$$

Now suppose $X$ is reduced and irreducible. Every nonempty [affine open subscheme](../../../../../affine-open-subscheme.md) is also reduced and irreducible: irreducibility passes to nonempty [open subsets](../../../../../open-set.md), because their nonempty open subsets are nonempty opens of $X$. The affine criterion makes each [coordinate ring](../../../../../coordinate-ring.md) an [integral domain](../../../../../integral-domain.md), so $X$ is integral. Conversely, suppose all its nonempty affine [coordinate rings](../../../../../coordinate-ring.md) are [integral domains](../../../../../integral-domain.md). Their [localizations](../../../../../localization-of-a-ring.md) show that $X$ is reduced. If $X$ were reducible, there would be disjoint nonempty [open subsets](../../../../../open-set.md); choose nonempty [affine open subschemes](../../../../../affine-open-subscheme.md) $U=\operatorname{Spec}A$ and $V=\operatorname{Spec}B$ inside them. Their disjoint union is itself an [affine open subscheme](../../../../../affine-open-subscheme.md) $\operatorname{Spec}(A\times B)$. Since $A,B$ are nonzero, $(1,0)(0,1)=0$ contradicts the domain condition. Therefore

$$
\boxed{X\text{ is integral}\iff X\text{ is reduced and irreducible}.}
$$

The [generic point](../../../../../generic-point.md) of an [integral scheme](../../../../../integral-scheme.md) $X$ is the unique point $\eta$ with $\overline{\{\eta\}}=X$. For existence, take a nonempty [affine open subscheme](../../../../../affine-open-subscheme.md) $V=\operatorname{Spec}A$. Its point $(0)$ has closure containing $V$, which is dense in $X$, so its closure in $X$ is all of $X$. For uniqueness, both proposed [generic points](../../../../../generic-point.md) lie in every nonempty [open subset](../../../../../open-set.md), hence in $V$, where the only dense point is $(0)$. The [function field](../../../../../function-field-of-an-algebraic-variety.md) is

$$
K(X)=\mathcal O_{X,\eta}=\operatorname{Frac}(A).
$$

Here the [stalk](../../../../../stalk-of-a-sheaf.md) description shows that the [field of fractions](../../../../../field-of-fractions.md) is independent of the choice of nonempty [affine open subscheme](../../../../../affine-open-subscheme.md).

Every nonempty [open subscheme](../../../../../open-subscheme.md) $U$ contains $\eta$, so taking a [germ](../../../../../germ-of-a-sheaf-section.md) there defines $\Gamma(U,\mathcal O_X)\to K(X)$. If a section has zero germ, restrict it to any nonempty [affine open subscheme](../../../../../affine-open-subscheme.md) $V\subseteq U$. Its image in $\operatorname{Frac}\Gamma(V,\mathcal O_X)$ is zero. Since this [coordinate ring](../../../../../coordinate-ring.md) is an [integral domain](../../../../../integral-domain.md), the section is zero on $V$. Such affines cover $U$, and the [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md) makes the section zero on $U$. Thus the [generic-point embedding of regular functions](../../../../../generic-point-embedding-of-regular-functions.md) is

$$
\boxed{\Gamma(U,\mathcal O_X)\hookrightarrow K(X).}
$$

For a [nonreduced reducible fibre between integral schemes](../../../../../nonreduced-reducible-fibre-between-integral-schemes.md), take both source and target to be the [affine line](../../../../../affine-line.md) over $\mathbb C$, and use the [ring homomorphism](../../../../../ring-homomorphism.md)

$$
\mathbb C[t]\longrightarrow\mathbb C[x],\qquad t\longmapsto x^2(x-1)^2.
$$

Both [coordinate rings](../../../../../coordinate-ring.md) are [integral domains](../../../../../integral-domain.md), so both [schemes](../../../../../scheme.md) are integral. At the target [closed point](../../../../../closed-point.md) $t=0$, the [scheme-theoretic fibre](../../../../../scheme-theoretic-fibre.md) has ring

$$
\mathbb C[x]/\bigl(x^2(x-1)^2\bigr)
\cong\mathbb C[x]/(x^2)\times\mathbb C[x]/((x-1)^2),
$$

by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md). Its underlying space has two distinct [closed points](../../../../../closed-point.md), so it is reducible. The class of $x(x-1)$ is nonzero but has square zero, so it is not reduced. **Even a morphism between integral schemes can have a fibre consisting of two nonreduced double points.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
