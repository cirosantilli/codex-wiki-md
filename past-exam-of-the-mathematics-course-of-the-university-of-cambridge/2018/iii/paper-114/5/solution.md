<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Put $F=\mathbb F_2$. Under the usual bundle convention of a paracompact base, choose a fiber metric and let $D(E),S(E)$ be the [disk bundle](../../../../../disk-bundle.md) and [sphere bundle](../../../../../sphere-bundle.md) of the rank-$n$ real [vector bundle](../../../../../vector-bundle.md). A mod-two [Thom class](../../../../../thom-class.md) is a [relative cohomology](../../../../../relative-cohomology.md) class

$$
\boxed{u\in H^n(D(E),S(E);F)}
$$

whose restriction to every fiber pair $(D^n,S^{n-1})$ is the nonzero generator. Equivalently it is a class in $H^n(E,E\setminus B;F)$, where $B$ is identified with the zero section. No orientation choices are needed over $F$.

The [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) asserts that this class exists and that, for every $r$, the map

$$
\boxed{\Phi:H^{r-n}(B;F)\xrightarrow{\sim}H^r(D(E),S(E);F),\qquad
\Phi(a)=\pi^*a\smile u}
$$

is an isomorphism. The disk bundle retracts to the zero section $s:B\to D(E)$, so $H^r(D(E);F)\cong H^r(B;F)$. Define the mod-two [Euler class](../../../../../euler-class-of-a-vector-bundle.md) $e_2(E)=s^*u\in H^n(B;F)$, where the pullback includes the passage from relative to absolute cohomology. Under the Thom identification, the map from relative to absolute cohomology sends $a$ to $a\smile e_2(E)$. Substituting into the pair's [long exact sequence in cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) gives the [Gysin sequence of a sphere bundle](../../../../../gysin-sequence-of-a-sphere-bundle.md):

$$
\boxed{\cdots\longrightarrow H^{r-n}(B;F)\xrightarrow{\smile e_2(E)}H^r(B;F)
\xrightarrow{\pi^*}H^r(S(E);F)\xrightarrow{\pi_!}H^{r-n+1}(B;F)
\xrightarrow{\smile e_2(E)}H^{r+1}(B;F)\longrightarrow\cdots.}
$$

Here $\pi_!$ is the connecting homomorphism followed by $\Phi^{-1}$. Thus the sequence and the cup-product map have been derived from the Thom theorem, not just stated. The Thom/Gysin constructions are also discussed in [Hatcher's Vector Bundles and K-Theory, §3.2](https://pi.math.cornell.edu/~hatcher/VBKT/VB.pdf).

The original PDF specifies the [tautological bundle](../../../../../tautological-bundle.md) on $\mathbb{RP}^n$; the occurrences of $\mathbb R^n$ in this part of the TeX transcription have lost the projective-space symbol. Let $L\to\mathbb{RP}^n$ be this real line bundle. Its sphere bundle consists of pairs $(\ell,v)$ with $v$ a unit vector in the line $\ell$, so $S(L)\cong S^n$, with projection the antipodal double covering. Write $t=e_2(L)$.

The additive mod-two groups, obtainable from the one-cell-in-each-dimension [cellular chain complex](../../../../../cellular-chain-complex.md), are

$$
H^r(\mathbb{RP}^n;F)\cong
\begin{cases}F,&0\leq r\leq n,\\0,&\text{otherwise}.\end{cases}
$$

For $n\geq1$, both the base and $S^n$ are connected, so $\pi^*:H^0(\mathbb{RP}^n;F)\to H^0(S^n;F)$ is an isomorphism. Exactness makes the following $\pi_!$ zero and multiplication by $t$ injective from $H^0$ to $H^1$. For $1\leq r<n$, the term $H^r(S^n;F)$ vanishes, so the same [Gysin sequence](../../../../../gysin-sequence-of-a-sphere-bundle.md) makes

$$
\smile t:H^r(\mathbb{RP}^n;F)\longrightarrow H^{r+1}(\mathbb{RP}^n;F)
$$

injective. Since these groups are one-dimensional, the maps are isomorphisms. Hence $1,t,\ldots,t^n$ are the respective nonzero generators, while $t^{n+1}=0$ by dimension. The [mod-two cohomology ring of real projective space](../../../../../mod-two-cohomology-ring-of-real-projective-space.md) is therefore

$$
\boxed{H^*(\mathbb{RP}^n;F)\cong F[t]/(t^{n+1}),\qquad |t|=1.}
$$

For $n=0$ this is simply $F$, with $t=0$.

For integral coefficients, the additive groups are

$$
H^r(\mathbb{RP}^n;\mathbb Z)\cong
\begin{cases}
\mathbb Z,&r=0,\\
\mathbb Z/2,&r\text{ even and }0<r\leq n,\\
\mathbb Z,&r=n\text{ and }n\text{ odd},\\
0,&\text{otherwise}.
\end{cases}
$$

Indeed, the [cellular homology of real projective space](../../../../../cellular-homology-of-real-projective-space.md) has boundary multiplication by $2$ in even positive chain degrees and zero in odd degrees, and the integral cochain differential is its transpose. It remains to determine the products; the additive groups alone do not do so.

For $n\geq2$, the coefficient sequence $0\to\mathbb Z\xrightarrow{2}\mathbb Z\to F\to0$ has a [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) $\beta$. Because $H^1(\mathbb{RP}^n;\mathbb Z)=0$ and $H^2(\mathbb{RP}^n;\mathbb Z)=\mathbb Z/2$, exactness makes $a=\beta(t)$ the nonzero integral degree-two class. Reduction $\rho:H^2(\mathbb{RP}^n;\mathbb Z)\to H^2(\mathbb{RP}^n;F)$ is injective: its kernel is the image of multiplication by $2$, which is zero. Thus

$$
\rho(a)=t^2.
$$

More generally, reduction is injective in each positive even degree, and its compatibility with the [cup product](../../../../../cup-product.md) gives $\rho(a^j)=t^{2j}$. Consequently $a^j$ is the nonzero generator whenever $2j\leq n$. Also $2a=0$, and powers beyond the dimension vanish.

If $n=2m$ is even, these powers and the unit account for all groups, so the [integral cohomology ring of real projective space](../../../../../integral-cohomology-ring-of-real-projective-space.md) is

$$
\boxed{H^*(\mathbb{RP}^{2m};\mathbb Z)\cong\mathbb Z[a]/(2a,a^{m+1}),\qquad |a|=2.}
$$

If $n=2m+1$ is odd, add an integral top-dimensional [orientation class](../../../../../fundamental-class.md) $b$ of degree $2m+1$. Its reduction is the nonzero class $t^{2m+1}$. Every product $ab$ and $b^2$ is zero by dimension, and $b$ has infinite additive order. Hence

$$
\boxed{H^*(\mathbb{RP}^{2m+1};\mathbb Z)\cong
\mathbb Z[a,b]/(2a,a^{m+1},ab,b^2),\qquad |a|=2,\quad |b|=2m+1.}
$$

These formulas include $m=0$: the even space is a point with ring $\mathbb Z$, and the odd space is a circle with ring $\mathbb Z[b]/(b^2)$, $|b|=1$. The polynomial presentations are interpreted with the displayed grading and products; no extra positive-degree products are left unspecified.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
