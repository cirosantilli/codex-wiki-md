<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**The exact sequence and associated modules.** Put $A=k[x]$ and $\mathfrak m=(x)$. Evaluation at zero gives the [short exact sequence](../../../../short-exact-sequence.md) of $A$-[modules](../../../../module-mathematics.md)

$$
0\longrightarrow(x)\xrightarrow{\ j\ }A\xrightarrow{\ \operatorname{ev}_0\ }A/(x)=k\longrightarrow0.
$$

The [affine module sheaf](../../../../affine-module-sheaf.md) associated to $(x)$ is the [ideal sheaf](../../../../ideal-sheaf-of-a-closed-subscheme.md) $\mathcal J$ of the [closed point](../../../../closed-point.md) $p$, and the one associated to $A$ is the [structure sheaf](../../../../structure-sheaf-of-a-scheme.md) $\mathcal O_{\mathbb A^1_k}$. To identify the third term, on a [principal open subset](../../../../principal-open-subscheme.md) $D(g)$,

$$
\Gamma(D(g),\widetilde k)=k_g
=\begin{cases}k,&g(0)\ne0,\\0,&g(0)=0,\end{cases}
$$

which equals $\Gamma(i^{-1}D(g),\mathcal O_p)$. The restrictions also agree, so $\widetilde k\cong i_*\mathcal O_p$. [Exactness of localization](../../../../exactness-of-localization.md) proves that applying the [affine module sheaf](../../../../affine-module-sheaf.md) construction to the module sequence remains exact: on every [stalk](../../../../stalk-of-a-sheaf.md) the sequence is its [localization](../../../../localization-of-a-ring.md). Thus

$$
\boxed{0\longrightarrow\mathcal J\longrightarrow\mathcal O_{\mathbb A^1_k}\longrightarrow i_*\mathcal O_p\longrightarrow0.}
$$

Each term is an [affine module sheaf](../../../../affine-module-sheaf.md), hence a [quasi-coherent sheaf](../../../../quasi-coherent-sheaf.md). In this example each is also a [coherent sheaf](../../../../coherent-sheaf.md), since its defining [module](../../../../module-mathematics.md) is finitely generated over the [Noetherian ring](../../../../noetherian-ring.md) $k[x]$.

**The failure of left exactness.** For an [affine module sheaf](../../../../affine-module-sheaf.md) $\widetilde M$, the [pullback of a sheaf of modules](../../../../pullback-of-a-sheaf-of-modules.md) along $i$ corresponds to the [tensor product of modules](../../../../tensor-product-of-modules.md) $k\otimes_A M$. In particular,

$$
i^*\mathcal J\ \leftrightarrow\ (x)\otimes_A A/(x)
\cong(x)/(x)^2\cong k,
\qquad
i^*\mathcal O_{\mathbb A^1_k}\ \leftrightarrow\ k.
$$

The first [vector space](../../../../vector-space-split.md) is nonzero, with [basis](../../../../basis.md) the class of $x$. But $i^*j$ sends this class to the class of $x$ in $A/(x)$, which is zero. Thus $i^*j$ is the zero map $k\to k$, and is not injective. More explicitly, the pulled-back sequence is

$$
0\longrightarrow k\xrightarrow{\ 0\ }k\xrightarrow{\ \operatorname{id}\ }k\longrightarrow0,
$$

where exactness fails at its first copy of $k$. Thus $i^*$ is not a [left-exact functor](../../../../finite-limit-preserving-functor.md):

$$
\boxed{i^*\text{ is not a left-exact functor on sheaves of }\mathcal O_{\mathbb A^1_k}\text{-modules}.}
$$

Although $(x)$ is a [free module](../../../../free-module.md) over $A$ with one generator, its inclusion into $A$ becomes multiplication by $x$ after choosing its generator; the [tensor product of modules](../../../../tensor-product-of-modules.md) with $A/(x)$ kills that map. This makes explicit why local freeness of $\mathcal J$ does not preserve this injection under the given [pullback](../../../../pullback-category-theory.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
