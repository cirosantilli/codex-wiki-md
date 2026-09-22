<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $X$ be an [affine variety](../../../../../affine-algebraic-set.md) over an [algebraically closed field](../../../../../algebraically-closed-field.md) $k$, with reduced [coordinate ring](../../../../../coordinate-ring.md) $A=k[X]$. On an open subset $U$, define $\mathcal O_X(U)$ to be the functions $h:U\to k$ which, near every point, have an expression $a/b$ with $a,b\in A$ and $b$ nowhere zero on that neighbourhood. Restriction is ordinary restriction of functions. Compatible local functions glue uniquely and remain locally quotients, so this defines the [structure sheaf](../../../../../structure-sheaf-of-a-scheme.md). On the [principal open subset](../../../../../principal-open-subscheme.md) $D(f)$ it gives $A_f$, and at $P$ it gives the [local ring](../../../../../local-ring.md) $A_{\mathfrak m_P}$. The principal-open identification can also be seen by identifying $D(f)$ with the affine algebraic set obtained by adjoining a coordinate $t$ and the equation $tf=1$; its [coordinate ring](../../../../../coordinate-ring.md) is $A[t]/(tf-1)\cong A_f$. This construction permits several [irreducible components](../../../../../irreducible-component.md); no division by a function vanishing identically on a component is assumed.

An abstract [algebraic variety](../../../../../algebraic-variety.md) is a [locally ringed space](../../../../../locally-ringed-space.md) locally isomorphic to such affine models, with a finite affine cover; we use the usual separated convention. Reducible [varieties](../../../../../algebraic-variety.md) are allowed here. The separation condition says that the [diagonal morphism](../../../../../diagonal-morphism.md) is a [closed immersion](../../../../../closed-immersion.md). Two [varieties](../../../../../algebraic-variety.md) are related by a [birational map](../../../../../birational-map.md) with an inverse when some dense open subset of one is [isomorphic](../../../../../isomorphism.md) as a locally ringed space to a dense open subset of the other.

Define the [ring of rational functions on a reduced variety](../../../../../ring-of-rational-functions-on-a-reduced-variety.md) by pairs $(U,h)$, where $U\subseteq X$ is dense open and $h\in\mathcal O_X(U)$, identifying two pairs when their restrictions agree on a common dense open subset. Finite intersections of dense open subsets are dense, so addition and multiplication on these intersections are well defined. For an [irreducible variety](../../../../../irreducible-variety.md) this gives the usual [function field](../../../../../function-field-of-an-algebraic-variety.md); for a reducible [variety](../../../../../algebraic-variety.md) it need not be a [field](../../../../../field.md). Restriction to any dense open subset $V$ induces an [isomorphism](../../../../../isomorphism.md)

$$
\operatorname{Rat}(X)\cong\operatorname{Rat}(V).
$$

Indeed, intersecting domains with $V$ defines the restriction, and a dense open subset of $V$ is also dense open in $X$, which defines its inverse. An [isomorphism](../../../../../isomorphism.md) between dense opens therefore induces an [isomorphism](../../../../../isomorphism.md) of their rational rings. Thus **birational [varieties](../../../../../algebraic-variety.md) have isomorphic rings of rational functions**, also in the reducible case.

For the finite-cover assertion, write the closed complement of $U$ as $V(I)$, where $I=(f_1,\ldots,f_r)$ is an [ideal](../../../../../ideal.md) of the [Noetherian ring](../../../../../noetherian-ring.md) $A$. Then

$$
U=D(f_1)\cup\cdots\cup D(f_r).
$$

Let $\mathfrak p_1,\ldots,\mathfrak p_t$ be the [minimal prime ideals](../../../../../minimal-prime-ideal.md) of $A$, corresponding to its [irreducible components](../../../../../irreducible-component.md). Since $U$ is dense, it meets every component, so $I$ is contained in none of these primes. [Prime avoidance](../../../../../prime-avoidance.md) supplies $s\in I$ outside their union. Consequently $D(s)\subseteq U$ meets a dense open subset of every component and is dense in $X$. Add $D(s)$ to the finite cover if necessary. This proves that **a finite principal-open cover can be chosen with a dense member**. It does not say that every principal-open cover already has such a member: for $X=V(xy)$, the dense open $X\setminus\{(0,0)\}=D(x)\cup D(y)$ has neither displayed member dense, although adding $D(x+y)$ supplies a dense member.

For clarity, the [zero divisors](../../../../../zero-divisor.md) in this reduced [Noetherian ring](../../../../../noetherian-ring.md) are exactly $\bigcup_i\mathfrak p_i$. If $ab=0$ and $a$ avoids every $\mathfrak p_i$, reduction in the domain $A/\mathfrak p_i$ forces $b\in\mathfrak p_i$ for all $i$, hence $b=0$. Conversely, if $a\in\mathfrak p_i$, choose for every $j\ne i$ an element $b_j\in\mathfrak p_j\setminus\mathfrak p_i$, possible because distinct minimal primes are incomparable. Their product $b$ is not in $\mathfrak p_i$ but belongs to all the other primes. Then $b\ne0$ and $ab\in\bigcap_j\mathfrak p_j=0$. For a single minimal prime, reducedness makes that prime zero and this argument uses $b=1$. It follows that

$$
s\text{ is a non-zero-divisor}\quad\Longleftrightarrow\quad D(s)\text{ is dense}.
$$

The [total quotient ring](../../../../../total-ring-of-fractions.md) $S^{-1}A$, where $S$ consists of these [non-zero-divisors](../../../../../non-zero-divisor.md), maps to $\operatorname{Rat}(X)$ by

$$
a/s\longmapsto\text{the class of the regular function }a/s\text{ on }D(s).
$$

The equivalence relation for [localization](../../../../../localization-of-a-ring.md) makes this a well-defined $k$-algebra homomorphism. For surjectivity, a rational class represented on $U$ restricts to the dense principal open $D(s)\subseteq U$ constructed above. Its section there belongs to $A_s$, so it is $a/s^r$ and lies in the image. For injectivity, if such a fraction is zero on a dense open subset, its numerator vanishes on that dense subset. The numerator's zero set is closed, so it vanishes everywhere on $X$ and is zero in the reduced [coordinate ring](../../../../../coordinate-ring.md). Thus

$$
\boxed{\operatorname{Rat}(X)\cong S^{-1}A.}
$$

In particular $A\to S^{-1}A$ is canonically [injective](../../../../../injective-function.md): $a/1=0$ implies $sa=0$ for some [non-zero-divisor](../../../../../non-zero-divisor.md) $s$, hence $a=0$.

Finally let $Y$ be the reduced closed union of exactly those [irreducible components](../../../../../irreducible-component.md) of $X$ which contain $P$. Removing all the other components gives an open neighbourhood of $P$ on which $X$ and $Y$ coincide, including their [structure sheaves](../../../../../structure-sheaf-of-a-scheme.md). Hence $\mathcal O_{X,P}\cong\mathcal O_{Y,P}$. Write $B=k[Y]$ and let $\mathfrak n_P$ be its maximal ideal at $P$. Every minimal prime of $B$ is contained in $\mathfrak n_P$, because every component of $Y$ contains $P$. If $b\notin\mathfrak n_P$, it avoids each such prime and is a [non-zero-divisor](../../../../../non-zero-divisor.md). Therefore the map of [localizations](../../../../../localization-of-a-ring.md)

$$
B_{\mathfrak n_P}\longrightarrow Q(B)=\operatorname{Rat}(Y),
\qquad a/b\longmapsto a/b,
$$

is defined and [injective](../../../../../injective-function.md): if its value is zero, a [non-zero-divisor](../../../../../non-zero-divisor.md) annihilates $a$, so $a=0$. We obtain the desired [local ring embeds in rational functions on incident components](../../../../../local-ring-embeds-in-rational-functions-on-incident-components.md):

$$
\boxed{\mathcal O_{X,P}\hookrightarrow\operatorname{Rat}(Y),
\qquad Y=\bigcup_{P\in X_i}X_i\ \text{with reduced structure}.}
$$

At an intersection point one must retain all incident components. For example, the [local ring](../../../../../local-ring.md) of $V(xy)$ at the origin has two nonzero germs $x,y$ with $xy=0$; it cannot embed into the [function field](../../../../../function-field-of-an-algebraic-variety.md) of just one of its axes.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
