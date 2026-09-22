<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For an idempotent [monad](../../../../../monad.md), the unit laws give $T\eta=\eta T=\mu^{-1}$. If $a:TA\to A$ is an algebra, $a\eta_A=1$ and naturality give

$$
\eta_Aa=Ta\,\eta_{TA}=Ta\,T\eta_A=T(a\eta_A)=1.
$$

Thus algebras are exactly the objects on which $\eta_A$ is invertible, with the unique algebra structure $\eta_A^{-1}$. They form a full reflective subcategory with reflector $T$. The assumed preservation of [finite limits](../../../../../finite-limit.md) makes this a [left-exact reflective subcategory](../../../../../left-exact-reflective-subcategory.md).

For a [subobject](../../../../../subobject.md) $S\hookrightarrow A$, define its closure by

$$
\overline S=A\times_{TA}TS\hookrightarrow A,
$$

using the unit and the [monomorphism](../../../../../monomorphism.md) $TS\hookrightarrow TA$. This [closure operation induced by a left-exact reflector](../../../../../closure-operation-induced-by-a-left-exact-reflector.md) is extensive by unit naturality, stable under pullback and preserves intersections because $T$ preserves [finite limits](../../../../../finite-limit.md). Applying $T$ to its defining square and using $T\eta$ invertible identifies $T\overline S$ with $TS$ over $TA$. Closing a second time therefore gives the same [subobject](../../../../../subobject.md). It is a universal idempotent closure operation, hence defines a [local operator](../../../../../lawvere-tierney-topology.md) $j$ by classifying the closure of $t:1\hookrightarrow\Omega$; closure of any mono is then classified by composing its classifier with $j$.

A mono $s:S\hookrightarrow A$ is $j$-dense exactly when $Ts$ is invertible. One implication follows immediately from the closure square. Conversely if its closure is all of $A$, the unit $\eta_A$ factors through $Ts$. Applying $T$ and using the invertible $T\eta_A$ makes $Ts$ split epic; since it is also monic, it is invertible. Every fixed object $B$ is consequently a $j$-sheaf, since the [adjunction](../../../../../adjoint-functors.md) gives

$$
\mathcal E(A,B)\cong\mathcal E(TA,B),\qquad\mathcal E(S,B)\cong\mathcal E(TS,B),
$$

and a dense restriction becomes an [isomorphism](../../../../../isomorphism.md).

Conversely let $B$ be a $j$-sheaf. Its diagonal is closed: the two projections from the closure of the diagonal agree on the dense diagonal, so uniqueness of extension into $B$ makes them agree everywhere. The closure formula identifies this closed diagonal with the [kernel pair](../../../../../kernel-pair.md) of $\eta_B$, since $T$ takes the diagonal of $B$ to the diagonal of $TB$. Thus $\eta_B$ is monic. Also $T\eta_B$ is invertible, so this mono is dense. The sheaf property extends $1_B$ across it to a retraction $TB\to B$. Since $TB$ is fixed and hence itself a sheaf, uniqueness across that dense mono also makes the other composite the identity. Therefore $\eta_B$ is invertible. We have proved **the algebra category is exactly the category of $j$-sheaves**.

Its topos structure is concrete. [Finite limits](../../../../../finite-limit.md) are computed in $\mathcal E$. For sheaves $A,B$, the ambient exponential $B^A$ is a sheaf: extension across a dense mono reduces, by transposition, to extension into $B$ across its product with $A$, again a dense mono. The classifier is $\Omega_j=\operatorname{Eq}(j,1_\Omega)$ with the induced truth point; it classifies closed [subobjects](../../../../../subobject.md). Colimits are obtained by taking the ambient colimit and applying $T$. These supply an elementary topos, as required.

For the second part, use the [square reader monad](../../../../../square-reader-monad.md)

$$
\eta_A(a)=(a,a),\qquad\mu_A((a,b),(c,d))=(a,d).
$$

The two unit laws select $(a,b)$ again. Each side of associativity selects the entries indexed $(0,0,0)$ and $(1,1,1)$ in an eight-entry array, so the [monad](../../../../../monad.md) laws hold. An algebra is an operation $*:A\times A\to A$ satisfying

$$
x*x=x,\qquad (x*y)*(z*w)=x*w.
$$

These imply associativity, since $(x*y)*z=(x*y)*(z*z)=x*z$ and $x*(y*z)=(x*x)*(y*z)=x*z$. They are the [rectangular band](../../../../../rectangular-band.md) laws.

For nonempty $A$, choose $e\in A$, and put $B=\{a*e:a\in A\}$, $C=\{e*a:a\in A\}$. Define $\phi(a)=(a*e,e*a)$ and $\psi(b,c)=b*c$. Then $(a*e)*(e*a)=a*a=a$, and for $b=x*e$, $c=e*y$ the laws give $(b*c)*e=b$ and $e*(b*c)=c$. Thus $\phi,\psi$ are inverse bijections. In these coordinates the operation is

$$
\boxed{(b,c)*(b',c')=(b,c').}
$$

Conversely any nonempty product with this operation satisfies the algebra laws, proving the requested correspondence with product decompositions. A homomorphism between nonempty products has its first coordinate depending only on the first factor and its second only on the second, as follows by applying it to the displayed operation. Hence it is exactly a pair of factor maps. There is in addition the unique empty algebra, a strict [initial object](../../../../../initial-object.md).

This algebra category is [Cartesian closed](../../../../../cartesian-closed-category.md). For nonempty $A=B\times C$ and $D=E\times F$, its exponential is $E^B\times F^C$ with rectangular multiplication: the usual set [adjunction](../../../../../adjoint-functors.md) in each factor gives the universal property. For the empty cases, $D^0=1$ and $0^A=0$ when $A$ is nonempty; these formulas also give $0^0=1$. They verify the [adjunction](../../../../../adjoint-functors.md) against empty test objects as well. Thus **the algebra category is [Cartesian closed](../../../../../cartesian-closed-category.md)**.

It is not a topos. If a classifier existed, its global elements would correspond to the two [subobjects](../../../../../subobject.md) of the terminal singleton algebra, so its underlying set would have two elements. A two-element [rectangular band](../../../../../rectangular-band.md) is either left-zero or right-zero: its two nonempty factors have sizes $(2,1)$ or $(1,2)$. A homomorphism from the four-element band $\{0,1\}\times\{0,1\}$ to a left-zero classifier depends only on the first coordinate, so the preimage of truth cannot be a single point; for a right-zero classifier the same failure occurs in the second coordinate. Yet a single point is a subalgebra and its inclusion is monic. Pullbacks of algebra maps are computed on underlying sets, so this [subobject](../../../../../subobject.md) could not be classified. Therefore **there is no [subobject classifier](../../../../../subobject-classifier.md) and the algebra category is not a topos**, despite its cartesian closure.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
