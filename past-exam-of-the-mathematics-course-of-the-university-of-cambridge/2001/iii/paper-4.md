# Paper 4

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper4.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper4.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $\mathcal U=(U_0,\ldots,U_m)$ be a finite [affine open cover](../../../topology.md#affine-open-cover) of the [projective scheme](../../../ringed-space.md#projective-scheme) $X$. For a [coherent sheaf](../../../ringed-space.md#coherent-sheaf) $\mathcal F$, form the [Čech cochain complex](../../../ringed-space.md#cech-cochain-complex)

$$
\check C^p(\mathcal U,\mathcal F)=\prod_{i_0<\cdots<i_p}\Gamma(U_{i_0}\cap\cdots\cap U_{i_p},\mathcal F),\qquad
(\delta c)_{i_0\ldots i_{p+1}}=\sum_{j=0}^{p+1}(-1)^j c_{i_0\ldots\widehat{i_j}\ldots i_{p+1}}\big|_{U_{i_0}\cap\cdots\cap U_{i_{p+1}}}.
$$

The two ways to omit any pair of indices have opposite signs, giving $\delta^2=0$. Its [cohomology groups](../../../cohomology.md#cohomology-group) are

$$
\check H^p(\mathcal U,\mathcal F)=\ker\delta^p/\operatorname{im}\delta^{p-1}.
$$

A [projective scheme](../../../ringed-space.md#projective-scheme) over a [field](../../../algebra.md#field) is a [separated scheme](../../../ringed-space.md#separated-scheme). Finite intersections of its affine opens are affine, and a [coherent sheaf](../../../ringed-space.md#coherent-sheaf) is [quasi-coherent](../../../ringed-space.md#quasi-coherent-sheaf). Higher [sheaf cohomology](../../../ringed-space.md#sheaf-cohomology) of a quasi-coherent sheaf on an [affine scheme](../../../ringed-space.md#affine-scheme) vanishes. Thus this is an acyclic cover and the [acyclic cover theorem](../../../ringed-space.md#leray-s-theorem) identifies the displayed [Čech cohomology](../../../ringed-space.md#cech-cohomology) with $H^p(X,\mathcal F)$. In particular its degree-zero kernel glues compatible local sections to $\Gamma(X,\mathcal F)$. A cover by $m+1$ opens also gives vanishing for $p>m$.

For the [cohomology of twists on projective space](../../../ringed-space.md#cohomology-of-twists-on-projective-space), take $S=k[X_0,\ldots,X_r]$ with the usual grading and $U_i=D_+(X_i)$. On an intersection indexed by the nonempty set $J$,

$$
\Gamma(U_J,\mathcal O(n))=\bigl(S[X_j^{-1}:j\in J]\bigr)_n.
$$

This follows directly from the construction of the [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space): sections of the twist are the degree-$n$ homogeneous fractions in the corresponding [localization](../../../commutative-algebra.md#localization-of-a-ring). The [Čech differential](../../../ringed-space.md#cech-differential) preserves each [Laurent monomial](../../../polynomial.md#laurent-monomial) $X^a=X_0^{a_0}\cdots X_r^{a_r}$, where $a_i\in\mathbb Z$ and $\sum_i a_i=n$. Such a monomial appears precisely in summands with

$$
N(a):=\{i:a_i<0\}\subseteq J.
$$

The complex therefore decomposes as the direct sum of finite-dimensional [cochain complexes](../../../algebra.md#cochain-complex) indexed by these exponent vectors. Their differentials have only the alternating signs of the simplex incidence maps.

If $N(a)=\varnothing$, this is the ordinary unaugmented [simplex](../../../algebraic-topology.md#simplex) cochain complex: its degree-zero kernel consists of the common value on every vertex and has dimension one, while all higher cohomology vanishes. If $\varnothing\ne N(a)\ne\{0,\ldots,r\}$, choose $v\notin N(a)$. A [cochain homotopy](../../../homology.md#cochain-homotopy) inserting $v$ into the ordered index list, with the sign of that insertion, contracts this subcomplex. Insertion or deletion of $v$ preserves the condition $N(a)\subseteq J$; in $\delta h+h\delta$, terms inserting and deleting different vertices cancel in pairs, while the term inserting then deleting $v$ is the identity. Thus this entire monomial subcomplex is acyclic. Finally, if all $a_i<0$, the monomial occurs only in the full intersection, in degree $r$, and contributes one copy of $k$ there.

For $r\ge1$, these three cases give the complete answer:

$$
\boxed{H^i(\mathbf P_k^r,\mathcal O(n))\cong
\begin{cases}
S_n,&i=0,\ n\ge0,\\
\displaystyle\bigoplus_{\substack{a_0,\ldots,a_r<0\\a_0+\cdots+a_r=n}}k\,X_0^{a_0}\cdots X_r^{a_r},&i=r,\ n\le-r-1,\\
0,&\text{otherwise}.
\end{cases}}
$$

In the first case counting nonnegative exponent vectors gives $h^0=\binom{n+r}{r}$. In the top case write $a_i=-1-b_i$ with $b_i\ge0$; then $\sum b_i=-n-r-1$, giving

$$
\boxed{h^r(\mathbf P_k^r,\mathcal O(n))=\binom{-n-1}{r}\quad(n\le-r-1).}
$$

This is the [Laurent-monomial description of top cohomology on projective space](../../../ringed-space.md#laurent-monomial-description-of-top-cohomology-on-projective-space). All intermediate degrees vanish for every twist, and the top degree vanishes when $n\ge-r$. If $r=0$, then $\mathbf P_k^0=\operatorname{Spec}k$ and every twist is trivial, so **$H^0(\mathbf P_k^0,\mathcal O(n))=k$ for every integer $n$, with all higher groups zero**.

## 2

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use [homogeneous coordinates](../../../projective-space.md#homogeneous-coordinate) $X_0,\ldots,X_n$. Multiplication by these degree-one sections defines the [sheaf morphism](../../../algebraic-geometry.md#morphism-of-sheaves)

$$
\epsilon:\mathcal O(-1)^{\oplus(n+1)}\longrightarrow\mathcal O,\qquad(s_0,\ldots,s_n)\longmapsto\sum_{j=0}^n X_j s_j.
$$

On $U_i=D_+(X_i)$, write $t_j^{(i)}=X_j/X_i$, with $t_i^{(i)}=1$, and let $E_j^{(i)}$ be the standard vector in component $j$ using the local [line bundle](../../../ringed-space.md#line-bundle) frame $X_i^{-1}$ of $\mathcal O(-1)$. Then $\epsilon(E_j^{(i)})=t_j^{(i)}$, so $\epsilon$ is surjective since $\epsilon(E_i^{(i)})=1$. Its [kernel](../../../linear-algebra.md#kernel-of-a-linear-map) is a [locally free sheaf](../../../ringed-space.md#locally-free-sheaf) with basis

$$
F_j^{(i)}=E_j^{(i)}-t_j^{(i)}E_i^{(i)}\qquad(j\ne i).
$$

Indeed any vector in the kernel is uniquely a sum of these vectors, by solving for its $i$-th component.

The [Kähler differential sheaf](../../../ringed-space.md#sheaf-of-kahler-differentials-over-a-field) $\Omega^1_{\mathbf P^n/k}$ has basis $dt_j^{(i)}$ on $U_i$, since this chart is a polynomial [affine scheme](../../../ringed-space.md#affine-scheme). Define the local map $dt_j^{(i)}\mapsto F_j^{(i)}$. To check that these isomorphisms glue, on $U_i\cap U_\ell$ put $u=t_i^{(\ell)}$ and $v=t_j^{(\ell)}$. Then

$$
t_j^{(i)}=\frac vu,\qquad dt_j^{(i)}=u^{-1}dt_j^{(\ell)}-vu^{-2}dt_i^{(\ell)}.
$$

The [twisting sheaf on projective space](../../../ringed-space.md#twisting-sheaf-on-projective-space) frame changes by $E_j^{(i)}=u^{-1}E_j^{(\ell)}$, hence

$$
F_j^{(i)}=u^{-1}F_j^{(\ell)}-vu^{-2}F_i^{(\ell)}.
$$

For $j=\ell$, use $t_\ell^{(\ell)}=1$, $dt_\ell^{(\ell)}=0$ and $F_\ell^{(\ell)}=0$; the same formula applies. Thus the differential and kernel frames have identical transition matrices. We obtain the cotangent form of the [Euler sequence](../../../algebraic-geometry.md#euler-sequence):

$$
\boxed{0\longrightarrow\Omega^1_{\mathbf P^n/k}\longrightarrow\mathcal O(-1)^{\oplus(n+1)}\xrightarrow{\epsilon}\mathcal O\longrightarrow0.}
$$

This construction works over any [field](../../../algebra.md#field), including positive characteristic.

The [Kähler differential sheaf](../../../ringed-space.md#sheaf-of-kahler-differentials-over-a-field) has rank $n$. Taking [determinant line bundles](../../../fiber-bundle.md#determinant-line-bundle) in this locally split [short exact sequence of sheaves](../../../algebraic-geometry.md#short-exact-sequence-of-sheaves) gives

$$
\det(\mathcal O(-1)^{\oplus(n+1)})\cong\det(\Omega^1_{\mathbf P^n/k})\otimes\det(\mathcal O).
$$

The left side is the tensor product of $n+1$ copies of $\mathcal O(-1)$, and $\det(\mathcal O)=\mathcal O$. Consequently

$$
\boxed{\bigwedge^n\Omega^1_{\mathbf P^n/k}\cong\mathcal O(-n-1).}
$$

It is the [canonical bundle of projective space](../../../ringed-space.md#canonical-bundle-of-projective-space). The determinant identity can also be seen directly by taking the wedge of the kernel basis followed by a lift of the quotient basis; changing that lift by a kernel vector leaves the wedge unchanged.

## 3

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The identification with $\mathbf P^1$ means that $C$ is a [smooth plane conic](../../../algebraic-geometry.md#smooth-plane-conic). An arbitrary singular or nonreduced conic over an [algebraically closed field](../../../algebra.md#algebraically-closed-field) cannot be identified with the projective line, so this is a necessary qualification implicit in the requested description.

Choose an equation $\ell=0$ for $L\subset\mathbf P^3$ and a degree-two equation $q=0$ whose restriction to $L$ defines $C$. Its [homogeneous ideal](../../../commutative-algebra.md#homogeneous-ideal) in $\mathbf P^3$ is $(\ell,q)$. These equations form a [regular sequence](../../../commutative-algebra.md#regular-sequence): $\ell$ is a non-zero-divisor in the polynomial ring, and modulo $\ell$ the ring is a polynomial ring in three variables, in which the nonzero quadratic $q$ is again a non-zero-divisor. The generator classes therefore form a basis of the [conormal sheaf](../../../ringed-space.md#conormal-sheaf), with their grading shifts:

$$
\mathcal I_C/\mathcal I_C^2\cong\mathcal O_C(-1)\oplus\mathcal O_C(-2).
$$

One can verify the absence of relations from the two-generator [Koszul complex](../../../homology.md#koszul-complex): a relation between $\ell,q$ is a multiple of $(q,-\ell)$, whose coefficients become zero modulo $\mathcal I_C$. This is the [normal sheaf of a projective complete intersection](../../../ringed-space.md#normal-sheaf-of-a-projective-complete-intersection) calculation. Dualizing the conormal sheaf gives

$$
N_{C/\mathbf P^3}\cong\mathcal O_C(1)\oplus\mathcal O_C(2).
$$

These twists are restrictions from $\mathbf P^3$, not intrinsic degree-one twists on $\mathbf P^1$. A line in the plane cuts the degree-two curve in two points counted with multiplicity, so the [degree of a line bundle](../../../ringed-space.md#degree-of-a-line-bundle) $\mathcal O_C(1)$ is two. The [Picard group of the projective line](../../../ringed-space.md#picard-group-of-the-projective-line) then gives

$$
\mathcal O_C(1)\cong\mathcal O_{\mathbf P^1}(2),\qquad\mathcal O_C(2)\cong\mathcal O_{\mathbf P^1}(4).
$$

Equivalently, the degree-two [Veronese embedding](../../../ringed-space.md#veronese-embedding) $[s:t]\mapsto[s^2:st:t^2]$ pulls each linear coordinate back to a quadratic. Thus the [normal bundle of a smooth plane conic](../../../algebraic-geometry.md#normal-bundle-of-a-smooth-plane-conic) is

$$
\boxed{N_{C/\mathbf P^3}\cong\mathcal O_{\mathbf P^1}(4)\oplus\mathcal O_{\mathbf P^1}(2),\qquad\{a,b\}=\{4,2\}.}
$$

The same splitting follows from the normal sequence for the two embeddings:

$$
0\longrightarrow N_{C/L}\longrightarrow N_{C/\mathbf P^3}\longrightarrow N_{L/\mathbf P^3}|_C\longrightarrow0.
$$

Its outer terms are $\mathcal O_{\mathbf P^1}(4)$ and $\mathcal O_{\mathbf P^1}(2)$. The [extension group](../../../algebra.md#extension-group) class lies in $\operatorname{Ext}^1(\mathcal O(2),\mathcal O(4))=H^1(\mathbf P^1,\mathcal O(2))=0$, by the preceding [Čech cohomology](../../../ringed-space.md#cech-cohomology) calculation, so the sequence splits. Both methods distinguish the ambient twist from the intrinsic degree on the curve.

## 4

↑ **Parent:** [Paper 4](paper-4.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a [projective scheme](../../../ringed-space.md#projective-scheme) $X$ over $k$, define its [Hilbert functor](../../../algebraic-geometry.md#hilbert-functor) on $k$-schemes by assigning to $T$ the set of [closed subschemes](../../../ringed-space.md#closed-subscheme) $W\subseteq X\times_kT$ such that $W\to T$ is a [flat morphism](../../../ringed-space.md#flat-morphism) of finite presentation and is proper. For projective $X$, the properness is automatic for these closed families. A morphism $T'\to T$ sends a family to $W\times_TT'\subseteq X\times_kT'$; [base change](../../../ringed-space.md#base-change-of-a-morphism-of-schemes) preserves the required properties, making this a contravariant [functor](../../../category.md#functor). The embedding in $X\times T$ is part of the data, so these are embedded families rather than families modulo automorphisms of $X$.

Choose a very ample [line bundle](../../../ringed-space.md#line-bundle) on $X$. In a flat projective family of finite presentation the fibre [Hilbert polynomial](../../../algebraic-geometry.md#hilbert-polynomial) is locally constant. Requiring polynomial $P$ gives a subfunctor represented by $\operatorname{Hilb}^P(X)$; the unrestricted [Hilbert functor](../../../algebraic-geometry.md#hilbert-functor) is represented by the disjoint union over $P$. For the specified $Z$, use its polynomial $P_Z$ and let $h=[Z]$ be the resulting $k$-point of the [Hilbert scheme](../../../algebraic-geometry.md#hilbert-scheme) $H$.

A [Zariski tangent space](../../../algebraic-geometry.md#zariski-tangent-space) vector at $h$ is a $k$-morphism

$$
v:\operatorname{Spec}D\longrightarrow H,\qquad D=k[\varepsilon]/(\varepsilon^2),
$$

whose restriction to $\operatorname{Spec}k$ is $h$. Here $D$ is the ring of [dual numbers](../../../commutative-algebra.md#dual-number). Locally such a morphism sends $a$ to $a(h)+\varepsilon d(a)$, where $d(ab)=a(h)d(b)+b(h)d(a)$, so these morphisms form the vector space $\operatorname{Hom}_k(\mathfrak m_h/\mathfrak m_h^2,k)$. By the representing property of the [Hilbert scheme](../../../algebraic-geometry.md#hilbert-scheme), the same tangent vector is exactly a [first-order embedded deformation](../../../algebraic-geometry.md#first-order-embedded-deformation)

$$
Z_\varepsilon\subseteq X\times_k\operatorname{Spec}D,\qquad Z_\varepsilon\text{ flat over }D,\qquad Z_\varepsilon\times_Dk=Z
$$

with the last equality an equality of embedded [closed subschemes](../../../ringed-space.md#closed-subscheme).

Let $\mathcal I$ be the [ideal sheaf](../../../ringed-space.md#ideal-sheaf-of-a-closed-subscheme) of $i:Z\hookrightarrow X$, and define its [normal sheaf](../../../ringed-space.md#normal-sheaf) by

$$
\mathcal N_{Z/X}=\mathcal Hom_{\mathcal O_Z}(\mathcal I/\mathcal I^2,\mathcal O_Z).
$$

This definition is valid even when $X$ or $Z$ is singular; it need not give a locally free sheaf. We now derive the tangent-space identification by constructing inverse maps, rather than merely invoking the normal sheaf's name.

Work on an [affine open subscheme](../../../ringed-space.md#affine-open-subscheme) $\operatorname{Spec}A\subseteq X$, put $B=A/I$, and let $J\subseteq A\oplus\varepsilon A$ define a flat deformation with special fibre $B$. The [flatness criterion over dual numbers](../../../module-theory.md#flatness-criterion-over-dual-numbers) says that a $D$-module $M$ is flat exactly when

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

This is an [ideal](../../../commutative-algebra.md#ideal): multiplying by $a+\varepsilon b$ gives $af+\varepsilon(ag+bf)$, and $ag+bf\bmod I=a\phi(f)=\phi(af)$. Its reduction is $I$. To prove that its quotient is flat, suppose $\varepsilon[a+\varepsilon b]=0$. The condition $\varepsilon a\in J_\phi$ says $a\in I$. Choose $g$ lifting $\phi(a)$; then $a+\varepsilon g\in J_\phi$, so

$$
[a+\varepsilon b]=\varepsilon[b-g].
$$

Thus the kernel of $\varepsilon$ is its image, and the criterion proves flatness. These constructions are inverse: the graph condition reconstructs every lift in $J$, and changes by $\varepsilon I$ account for all choices.

[Localization](../../../commutative-algebra.md#localization-of-a-ring) respects both constructions. The local maps $I/I^2\to B$ therefore glue exactly to [global sections](../../../ringed-space.md#global-section) of the [internal Hom sheaf](../../../ringed-space.md#internal-hom-sheaf) $\mathcal N_{Z/X}$; conversely such a section gives compatible local ideals that glue to $Z_\varepsilon$. Hence

$$
\boxed{T_{[Z]}\operatorname{Hilb}(X)\cong\operatorname{Hom}_{\mathcal O_X}(\mathcal I,i_*\mathcal O_Z)\cong H^0(Z,\mathcal N_{Z/X}).}
$$

The middle identification uses that every map to $\mathcal O_Z$ kills $\mathcal I^2$. The zero map gives the product deformation $Z\times\operatorname{Spec}D$; addition and scalar multiplication of the maps $\phi$ give the canonical vector-space operations on the tangent space. This proves the [Zariski tangent space of a Hilbert scheme](../../../algebraic-geometry.md#zariski-tangent-space-of-a-hilbert-scheme) formula without a smoothness or regular-embedding hypothesis.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
