<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $X$ be a separated [Noetherian scheme](../../../../../noetherian-scheme.md) over a field $k$ and $\mathcal F$ a [coherent sheaf](../../../../../coherent-sheaf.md). [Coherent cohomology](../../../../../coherent-cohomology.md) studies the groups $H^q(X,\mathcal F)$: [global sections](../../../../../global-section.md) in degree zero and the obstructions to gluing local sections in higher degrees. Coherence means finite generation locally, and on a Noetherian scheme it is preserved by kernels, cokernels and extensions. This makes [coherent sheaves](../../../../../coherent-sheaf.md) suitable for exact-sequence calculations.

For an ordered open cover $\mathcal U=(U_i)$, the [Čech cochain groups](../../../../../cech-cochain-group.md) are

$$
\check C^q(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_q}\mathcal F(U_{i_0}\cap\cdots\cap U_{i_q}),
$$

with differential

$$
(\delta c)_{i_0\ldots i_{q+1}}
=\sum_{j=0}^{q+1}(-1)^j\left.c_{i_0\ldots\widehat{i_j}\ldots i_{q+1}}\right|_{U_{i_0}\cap\cdots\cap U_{i_{q+1}}}.
$$

Each double omission occurs twice with opposite signs, so $\delta^2=0$. The [Čech cohomology](../../../../../cech-cohomology.md) of the cover is $\check H^q=\ker\delta/\operatorname{im}\delta$, and taking the direct limit over refinements defines cover-independent Čech cohomology. In degree zero the [sheaf gluing axiom](../../../../../sheaf-gluing-axiom.md) identifies it with $\Gamma(X,\mathcal F)$.

The comparison with derived-functor [sheaf cohomology](../../../../../sheaf-cohomology.md) is particularly effective algebraically. Positive-degree cohomology of a [quasi-coherent sheaf](../../../../../quasi-coherent-sheaf.md) on an [affine scheme](../../../../../affine-scheme.md) vanishes. A separated scheme has affine intersections of affine opens, so a finite affine cover is acyclic for $\mathcal F$. Its [Čech cochain complex](../../../../../cech-cochain-complex.md) consequently computes $H^q(X,\mathcal F)$ directly. For a [short exact sequence of sheaves](../../../../../short-exact-sequence-of-sheaves.md), sections over each affine intersection are exact on quasi-[coherent sheaves](../../../../../coherent-sheaf.md). The resulting short exact sequence of Čech complexes gives the [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md). In particular, the connecting map measures the failure of a global section of the quotient to lift globally.

Several central projective results make the theory finite and computable. On a [projective variety](../../../../../projective-variety.md) over $k$, every coherent cohomology group is finite-dimensional. The [Grothendieck vanishing](../../../../../grothendieck-vanishing.md) theorem gives $H^q(X,\mathcal F)=0$ for $q>\dim X$. If $\mathcal O_X(1)$ is ample, [Serre vanishing](../../../../../serre-vanishing.md) gives $H^{q>0}(X,\mathcal F(m))=0$ for sufficiently large $m$, and these large twists are [globally generated sheaves](../../../../../globally-generated-sheaf.md). On [projective space](../../../../../projective-space-split.md) a [coherent sheaf](../../../../../coherent-sheaf.md) has a [finite twisting resolution of a coherent sheaf on projective space](../../../../../finite-twisting-resolution-of-a-coherent-sheaf-on-projective-space.md): finite sums of $\mathcal O(a)$ resolve it. The explicit line-bundle cohomology below and the long exact sequences prove finiteness and positive-twist vanishing. For a closed embedding $i:X\hookrightarrow\mathbb P^n$, $i_*\mathcal F$ is coherent and $H^q(X,\mathcal F)=H^q(\mathbb P^n,i_*\mathcal F)$, reducing these results to [projective space](../../../../../projective-space-split.md). A sufficiently positive twist of a finite presentation by sums of $\mathcal O(-a)$ also proves global generation.

The [Euler characteristic of a coherent sheaf](../../../../../euler-characteristic-of-a-coherent-sheaf.md)

$$
\chi(X,\mathcal F)=\sum_q(-1)^q\dim_kH^q(X,\mathcal F)
$$

is therefore defined, and the long exact sequence makes it additive. With a fixed projective embedding, $\chi(X,\mathcal F(m))$ is its [Hilbert polynomial](../../../../../hilbert-polynomial.md), and for sufficiently large $m$ it equals $h^0(X,\mathcal F(m))$. On a smooth projective variety of dimension $r$, [Serre duality](../../../../../serre-duality.md) gives, for a [vector bundle](../../../../../vector-bundle.md) $E$,

$$
H^q(X,E)^*\cong H^{r-q}(X,E^*\otimes\omega_X).
$$

For an arbitrary [coherent sheaf](../../../../../coherent-sheaf.md) the correct counterpart is $H^q(X,\mathcal F)^*\cong\operatorname{Ext}^{r-q}_X(\mathcal F,\omega_X)$; replacing this Ext group indiscriminately by the cohomology of the ordinary sheaf dual would lose local extension information.

We now calculate the basic examples. For $n\ge1$, use the standard cover $U_i=D_+(x_i)$ of $\mathbb P^n$. Sections of $\mathcal O(m)$ on an intersection are degree-$m$ [Laurent monomials](../../../../../laurent-monomial.md) in which negative exponents are allowed only for coordinates inverted on that intersection. Decompose the [Čech cochain complex](../../../../../cech-cochain-complex.md) by exponent vectors $(a_0,\ldots,a_n)$ with sum $m$. If no exponent is negative, the corresponding simplex complex contributes only in degree zero. If all exponents are negative, the monomial occurs only on the full intersection and contributes only in degree $n$. When the negative-index set is nonempty and proper, inserting any index outside it gives a contracting homotopy, so the monomial complex is acyclic. Hence the [cohomology of twisting sheaves on projective space](../../../../../cohomology-of-twisting-sheaves-on-projective-space.md) is

$$
H^q(\mathbb P^n,\mathcal O(m))\cong
\begin{cases}
k[x_0,\ldots,x_n]_m,&q=0,\ m\ge0,\\
k^{\binom{-m-1}{n}},&q=n,\ m\le-n-1,\\
0,&\text{otherwise}.
\end{cases}
$$

In the top group a basis consists of the [Laurent monomials](../../../../../laurent-monomial.md) with every exponent at most $-1$. Writing $a_i=-1-b_i$ reduces the count to nonnegative solutions of $\sum b_i=-m-n-1$, giving the displayed binomial coefficient. In particular, all intermediate cohomology vanishes, and $\omega_{\mathbb P^n}=\mathcal O(-n-1)$ agrees with [Serre duality](../../../../../serre-duality.md). For $\mathbb P^0$ separately, every twist is trivial and $H^0=k$.

On the [projective line](../../../../../projective-line.md) this gives

$$
h^0(\mathcal O(m))=\max(m+1,0),\qquad h^1(\mathcal O(m))=\max(-m-1,0),\qquad\chi(\mathcal O(m))=m+1.
$$

Thus positive and negative degrees produce quite different groups, while their alternating difference is a single polynomial. The [twisted cubic](../../../../../twisted-cubic.md) is isomorphic to $\mathbb P^1$ and its hyperplane bundle corresponds to $\mathcal O_{\mathbb P^1}(3)$. Consequently $h^0(X,\mathcal O_X(m))=3m+1$ for $m\ge0$, agreeing with Q2, and $h^1(X,\mathcal O_X(m))=\max(-3m-1,0)$.

For a smooth plane curve $C$ of degree $d\ge1$, the [ideal-sheaf sequence of a projective hypersurface](../../../../../ideal-sheaf-sequence-of-a-projective-hypersurface.md) is

$$
0\longrightarrow\mathcal O_{\mathbb P^2}(-d)\longrightarrow\mathcal O_{\mathbb P^2}\longrightarrow i_*\mathcal O_C\longrightarrow0.
$$

The [long exact sequence in sheaf cohomology](../../../../../long-exact-sequence-in-sheaf-cohomology.md) and the preceding formula give $H^0(C,\mathcal O_C)=k$ and $H^1(C,\mathcal O_C)\cong H^2(\mathbb P^2,\mathcal O(-d))$. Therefore

$$
\boxed{g(C)=\frac{(d-1)(d-2)}2.}
$$

For $d=1,2$ this is zero; for a plane cubic it is one. Twisting the same exact sequence gives $\chi(C,\mathcal O_C(m))=dm+1-g$. These examples illustrate how [Čech cohomology](../../../../../cech-cohomology.md), vanishing, [Serre duality](../../../../../serre-duality.md) and exact sequences convert local equations into global numerical invariants.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
