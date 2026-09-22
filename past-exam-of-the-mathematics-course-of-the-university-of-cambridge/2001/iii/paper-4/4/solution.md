<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [projective scheme](../../../../../projective-scheme.md) $X$ over $k$, define its [Hilbert functor](../../../../../hilbert-functor.md) on $k$-schemes by assigning to $T$ the set of [closed subschemes](../../../../../closed-subscheme.md) $W\subseteq X\times_kT$ such that $W\to T$ is a [flat morphism](../../../../../flat-morphism.md) of finite presentation and is proper. For projective $X$, the properness is automatic for these closed families. A morphism $T'\to T$ sends a family to $W\times_TT'\subseteq X\times_kT'$; [base change](../../../../../base-change-of-a-morphism-of-schemes.md) preserves the required properties, making this a contravariant [functor](../../../../../functor.md). The embedding in $X\times T$ is part of the data, so these are embedded families rather than families modulo automorphisms of $X$.

Choose a very ample [line bundle](../../../../../line-bundle.md) on $X$. In a flat projective family of finite presentation the fibre [Hilbert polynomial](../../../../../hilbert-polynomial.md) is locally constant. Requiring polynomial $P$ gives a subfunctor represented by $\operatorname{Hilb}^P(X)$; the unrestricted [Hilbert functor](../../../../../hilbert-functor.md) is represented by the disjoint union over $P$. For the specified $Z$, use its polynomial $P_Z$ and let $h=[Z]$ be the resulting $k$-point of the [Hilbert scheme](../../../../../hilbert-scheme.md) $H$.

A [Zariski tangent space](../../../../../zariski-tangent-space.md) vector at $h$ is a $k$-morphism

$$
v:\operatorname{Spec}D\longrightarrow H,\qquad D=k[\varepsilon]/(\varepsilon^2),
$$

whose restriction to $\operatorname{Spec}k$ is $h$. Here $D$ is the ring of [dual numbers](../../../../../dual-number.md). Locally such a morphism sends $a$ to $a(h)+\varepsilon d(a)$, where $d(ab)=a(h)d(b)+b(h)d(a)$, so these morphisms form the vector space $\operatorname{Hom}_k(\mathfrak m_h/\mathfrak m_h^2,k)$. By the representing property of the [Hilbert scheme](../../../../../hilbert-scheme.md), the same tangent vector is exactly a [first-order embedded deformation](../../../../../first-order-embedded-deformation.md)

$$
Z_\varepsilon\subseteq X\times_k\operatorname{Spec}D,\qquad Z_\varepsilon\text{ flat over }D,\qquad Z_\varepsilon\times_Dk=Z
$$

with the last equality an equality of embedded [closed subschemes](../../../../../closed-subscheme.md).

Let $\mathcal I$ be the [ideal sheaf](../../../../../ideal-sheaf-of-a-closed-subscheme.md) of $i:Z\hookrightarrow X$, and define its [normal sheaf](../../../../../normal-sheaf.md) by

$$
\mathcal N_{Z/X}=\mathcal Hom_{\mathcal O_Z}(\mathcal I/\mathcal I^2,\mathcal O_Z).
$$

This definition is valid even when $X$ or $Z$ is singular; it need not give a locally free sheaf. We now derive the tangent-space identification by constructing inverse maps, rather than merely invoking the normal sheaf's name.

Work on an [affine open subscheme](../../../../../affine-open-subscheme.md) $\operatorname{Spec}A\subseteq X$, put $B=A/I$, and let $J\subseteq A\oplus\varepsilon A$ define a flat deformation with special fibre $B$. The [flatness criterion over dual numbers](../../../../../flatness-criterion-over-dual-numbers.md) says that a $D$-module $M$ is flat exactly when

$$
\ker(\varepsilon:M\to M)=\varepsilon M.
$$

Flatness implies this by tensoring $0\to(\varepsilon)\to D\to k\to0$. Conversely lift a $k$-basis of $M/\varepsilon M$ to $M$. It generates $M$ over $D$: after removing the linear combination representing an element modulo $\varepsilon$, the remainder is $\varepsilon$ times another element, whose residue is another finite basis combination. For independence, reduce a relation modulo $\varepsilon$ to remove its constant coefficients. The remaining relation says that a linear combination of the lifts belongs to the kernel of $\varepsilon$, hence to $\varepsilon M$, so its remaining coefficients vanish modulo $\varepsilon$ too. The lifts are a free $D$-basis, establishing flatness.

Applying this criterion to $M=(A\oplus\varepsilon A)/J$ gives

$$
J\cap\varepsilon A=\varepsilon I.
$$

Indeed $\varepsilon I\subseteq J$ follows by lifting each $f\in I$ to $f+\varepsilon g\in J$ and multiplying by $\varepsilon$. Conversely, if $\varepsilon a\in J$, then the class of $a$ is in the kernel of $\varepsilon$ on $M$, hence in $\varepsilon M$; reducing modulo $\varepsilon$ gives $a\in I$.

For $f\in I$, choose a lift $f+\varepsilon g\in J$ and define

$$
\phi(f)=g\bmod I\in B.
$$

Two lifts differ by an element of $J\cap\varepsilon A=\varepsilon I$, so this is well defined. Addition and multiplication of lifts by elements of $A$ prove that $\phi$ is $A$-linear. For $f_1,f_2\in I$, one has $\phi(f_1f_2)=f_1\phi(f_2)=0$ in $B$, so it factors through an element of $\operatorname{Hom}_B(I/I^2,B)$.

Conversely, for such a homomorphism define

$$
J_\phi=\{f+\varepsilon g:f\in I,\quad g\bmod I=\phi(f)\}\subseteq A\oplus\varepsilon A.
$$

This is an [ideal](../../../../../ideal.md): multiplying by $a+\varepsilon b$ gives $af+\varepsilon(ag+bf)$, and $ag+bf\bmod I=a\phi(f)=\phi(af)$. Its reduction is $I$. To prove that its quotient is flat, suppose $\varepsilon[a+\varepsilon b]=0$. The condition $\varepsilon a\in J_\phi$ says $a\in I$. Choose $g$ lifting $\phi(a)$; then $a+\varepsilon g\in J_\phi$, so

$$
[a+\varepsilon b]=\varepsilon[b-g].
$$

Thus the kernel of $\varepsilon$ is its image, and the criterion proves flatness. These constructions are inverse: the graph condition reconstructs every lift in $J$, and changes by $\varepsilon I$ account for all choices.

[Localization](../../../../../localization-of-a-ring.md) respects both constructions. The local maps $I/I^2\to B$ therefore glue exactly to [global sections](../../../../../global-section.md) of the [internal Hom sheaf](../../../../../internal-hom-sheaf.md) $\mathcal N_{Z/X}$; conversely such a section gives compatible local ideals that glue to $Z_\varepsilon$. Hence

$$
\boxed{T_{[Z]}\operatorname{Hilb}(X)\cong\operatorname{Hom}_{\mathcal O_X}(\mathcal I,i_*\mathcal O_Z)\cong H^0(Z,\mathcal N_{Z/X}).}
$$

The middle identification uses that every map to $\mathcal O_Z$ kills $\mathcal I^2$. The zero map gives the product deformation $Z\times\operatorname{Spec}D$; addition and scalar multiplication of the maps $\phi$ give the canonical vector-space operations on the tangent space. This proves the [Zariski tangent space of a Hilbert scheme](../../../../../zariski-tangent-space-of-a-hilbert-scheme.md) formula without a smoothness or regular-embedding hypothesis.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
