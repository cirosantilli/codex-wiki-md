<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [locally ringed space](../../../../../locally-ringed-space.md) is a [topological space](../../../../../topological-space.md) $X$ equipped with a [sheaf](../../../../../sheaf-mathematics.md) of commutative [rings](../../../../../ring.md) $\mathcal O_X$ whose [stalk](../../../../../stalk-of-a-sheaf.md) $\mathcal O_{X,x}$ at every point is a [local ring](../../../../../local-ring.md). A [morphism of locally ringed spaces](../../../../../morphism-of-locally-ringed-spaces.md) $(f,f^\#):(Y,\mathcal O_Y)\to(X,\mathcal O_X)$ consists of a [continuous map](../../../../../continuous-map.md) $f:Y\to X$ and a [morphism of sheaves](../../../../../morphism-of-sheaves.md) of [rings](../../../../../ring.md) $f^\#: \mathcal O_X\to f_*\mathcal O_Y$, with every induced [stalk](../../../../../stalk-of-a-sheaf.md) map $\mathcal O_{X,f(y)}\to\mathcal O_{Y,y}$ a [local homomorphism](../../../../../local-homomorphism-of-local-rings.md): the inverse image of the target [maximal ideal](../../../../../maximal-ideal.md) is the source [maximal ideal](../../../../../maximal-ideal.md). Here $f_*\mathcal O_Y$ is the [direct image sheaf](../../../../../direct-image-sheaf.md), with sections $\mathcal O_Y(f^{-1}U)$ on $U$.

Let $\phi:A\to B$ be a [ring homomorphism](../../../../../ring-homomorphism.md). Define the map between the [spectra of rings](../../../../../spectrum-of-a-commutative-ring.md) by

$$
f(\mathfrak q)=\phi^{-1}(\mathfrak q).
$$

The inverse image is a [prime ideal](../../../../../prime-ideal.md), and $f^{-1}(D(a))=D(\phi(a))$. Thus $f$ is a [continuous map](../../../../../continuous-map.md), because the [principal open subsets](../../../../../principal-open-subscheme.md) form a basis. On these [principal open subsets](../../../../../principal-open-subscheme.md), define the [structure sheaf](../../../../../structure-sheaf-of-a-scheme.md) map using the [localizations](../../../../../localization-of-a-ring.md)

$$
A_a\longrightarrow B_{\phi(a)},\qquad \frac{b}{a^r}\longmapsto\frac{\phi(b)}{\phi(a)^r}.
$$

These maps commute with restrictions and consequently give a [morphism of sheaves](../../../../../morphism-of-sheaves.md). At $\mathfrak q$, putting $\mathfrak p=\phi^{-1}\mathfrak q$, the [stalk](../../../../../stalk-of-a-sheaf.md) map is $A_{\mathfrak p}\to B_{\mathfrak q}$. An element $b/s$ belongs to its inverse image of $\mathfrak qB_{\mathfrak q}$ exactly when $b\in\mathfrak p$, so this is a [local homomorphism](../../../../../local-homomorphism-of-local-rings.md). We have constructed a [morphism of locally ringed spaces](../../../../../morphism-of-locally-ringed-spaces.md).

Conversely, take a [morphism of locally ringed spaces](../../../../../morphism-of-locally-ringed-spaces.md) $f:\operatorname{Spec}B\to\operatorname{Spec}A$. Its map on [global sections](../../../../../global-section.md) gives a [ring homomorphism](../../../../../ring-homomorphism.md)

$$
\phi:A=\Gamma(X,\mathcal O_X)\longrightarrow\Gamma(Y,\mathcal O_Y)=B.
$$

Locality of the [stalk](../../../../../stalk-of-a-sheaf.md) map implies, for every $a\in A$,

$$
a\in f(\mathfrak q)\quad\Longleftrightarrow\quad a/1\in\mathfrak m_{f(\mathfrak q)}\quad\Longleftrightarrow\quad\phi(a)/1\in\mathfrak qB_{\mathfrak q}\quad\Longleftrightarrow\quad\phi(a)\in\mathfrak q.
$$

Hence the point map must be $\mathfrak q\mapsto\phi^{-1}\mathfrak q$. On $D(a)$, its [structure sheaf](../../../../../structure-sheaf-of-a-scheme.md) map must send $b/1$ to $\phi(b)/1$ and the inverse of $a$ to the inverse of $\phi(a)$. Thus it is precisely the [localization](../../../../../localization-of-a-ring.md) map constructed above. Agreement on this basis proves agreement of the [morphisms of sheaves](../../../../../morphism-of-sheaves.md). In particular, **the inducing ring homomorphism exists and is unique**.

If $\phi$ is surjective, write $B=A/I$. The correspondence between [prime ideals](../../../../../prime-ideal.md) of $A/I$ and [prime ideals](../../../../../prime-ideal.md) of $A$ containing $I$ identifies $\operatorname{Spec}B$ homeomorphically with the closed subset $V(I)$: the [principal open subsets](../../../../../principal-open-subscheme.md) correspond on both sides. Moreover, the [stalk](../../../../../stalk-of-a-sheaf.md) maps are the surjections $A_{\mathfrak p}\to(A/I)_{\mathfrak p/I}$, so $\mathcal O_X\to f_*\mathcal O_Y$ is surjective.

For the converse, it is important not to assume that [global sections](../../../../../global-section.md) preserve an arbitrary surjection of [sheaves](../../../../../sheaf-mathematics.md). Here the [affine module-sheaf equivalence](../../../../../affine-module-sheaf-equivalence.md) supplies the extra information: on every $D(a)$,

$$
(f_*\mathcal O_Y)(D(a))=B_{\phi(a)}=B\otimes_AA_a.
$$

Thus $f_*\mathcal O_Y$ is the [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) associated with the $A$-[module](../../../../../module-mathematics.md) $B$, and the [cokernel sheaf](../../../../../cokernel-sheaf.md) of $\mathcal O_X\to f_*\mathcal O_Y$ is associated with the [module](../../../../../module-mathematics.md) $C=\operatorname{coker}(A\to B)$, since [localization of a module](../../../../../localization-of-a-module.md) is exact. Surjectivity of the [morphism of sheaves](../../../../../morphism-of-sheaves.md) gives $C_{\mathfrak p}=0$ for every [prime ideal](../../../../../prime-ideal.md) $\mathfrak p$. This implies $C=0$: if $0\ne c\in C$, its proper annihilator lies in a [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak m$, and then $c/1\ne0$ in $C_{\mathfrak m}$. Therefore $A\to B$ is surjective. We have proved the [closed immersion criterion for affine schemes](../../../../../closed-immersion-criterion-for-affine-schemes.md):

$$
\boxed{\phi\text{ surjective}\ \Longleftrightarrow\ f\text{ is a homeomorphism onto a closed subset and }\mathcal O_X\twoheadrightarrow f_*\mathcal O_Y.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
