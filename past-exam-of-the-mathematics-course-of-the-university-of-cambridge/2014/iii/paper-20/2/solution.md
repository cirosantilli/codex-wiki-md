<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [local operator](../../../../../lawvere-tierney-topology.md), also called a [Lawvere-Tierney topology](../../../../../lawvere-tierney-topology.md), is a map $j:\Omega\to\Omega$ which internally satisfies

$$
p\leq jp,\quad j\top=\top,\quad j(p\wedge q)=jp\wedge jq,\quad jjp=jp.
$$

The [closure operation of a local operator](../../../../../closure-operation-of-a-local-operator.md) sends a mono with characteristic map $\chi$ to the [subobject](../../../../../subobject.md) classified by $j\chi$. It is inflationary, idempotent and [pullback](../../../../../pullback-category-theory.md)-stable. A mono is [j-dense](../../../../../j-dense-monomorphism.md) if its closure is its whole codomain, and [j-closed](../../../../../j-closed-monomorphism.md) if it equals its closure. A [j-sheaf](../../../../../j-sheaf.md) $S$ is an object for which restriction

$$
\mathcal E(B,S)\longrightarrow\mathcal E(A,S)
$$

is a bijection for every j-dense mono $A\hookrightarrow B$; requiring only injectivity defines a [j-separated object](../../../../../j-separated-object.md).

Here is a construction underlying the [sheaf reflector for a local operator](../../../../../sheaf-reflector-for-a-local-operator.md). The [closed-subobject classifier](../../../../../closed-subobject-classifier.md) $\Omega_j=\{p:jp=p\}$ is a j-sheaf: closed [subobjects](../../../../../subobject.md) on a dense [subobject](../../../../../subobject.md) extend uniquely by taking their closure in the larger object. Powers $\Omega_j^X$ are also sheaves, because products of a dense mono with $X$ remain dense. A j-closed [subobject](../../../../../subobject.md) of a sheaf is a sheaf: first extend a map into the ambient sheaf, then use density to force its image into the closed [subobject](../../../../../subobject.md).

Close the diagonal of $X$. Its j-closure is an equivalence relation, using preservation of finite meets and [pullback](../../../../../pullback-category-theory.md)-stability to verify transitivity. The effective quotient $X\twoheadrightarrow X_s$ is the separated reflection: every map from $X$ into a separated object identifies that closed diagonal and factors uniquely. For separated $X_s$, the closed-singleton map

$$
X_s\longrightarrow\Omega_j^{X_s},\qquad x\longmapsto\bigl(z\longmapsto j(z=x)\bigr)
$$

is monic. Its j-closed image closure $a_jX$ is a sheaf, and $X_s\hookrightarrow a_jX$ is dense. Unique extension across that mono, following the separated quotient factorization, proves

$$
\mathcal E(X,S)\cong\mathbf{sh}_j(\mathcal E)(a_jX,S)
$$

for every sheaf $S$. This proves reflectivity. The closure construction is [pullback](../../../../../pullback-category-theory.md)-stable; equivalently, separated quotients and the subsequent dense embeddings commute with the finite limiting comparisons, giving the usual left-exact sheaf reflector.

[Finite limits](../../../../../finite-limit.md) of sheaves are computed in $\mathcal E$, because unique extensions can be taken componentwise. If $S$ is a sheaf, $S^T$ is a sheaf for any $T$, by the same product-with-dense-mono argument. Thus sheaf exponentials are the ambient exponentials. Monos between sheaves have j-closed images: their closure is a sheaf, and the dense inclusion into it splits by the extension property, hence is an isomorphism. Therefore $\Omega_j$ classifies precisely their [subobjects](../../../../../subobject.md). These observations establish **$\mathbf{sh}_j(\mathcal E)$ is a reflective topos**.

Now let $u:1\to\Omega$ classify the given [subterminal object](../../../../../subterminal-object.md). Its [open local operator](../../../../../open-local-operator.md) and [closed local operator](../../../../../closed-local-operator.md) are

$$
\boxed{o(U)(p)=(u\Rightarrow p),\qquad c(U)(p)=u\vee p.}
$$

The [Heyting algebra](../../../../../heyting-algebra.md) identities verify all local-operator axioms: implication by fixed $u$ preserves meets and is idempotent, while adjoining $u$ preserves meets by distributivity and is idempotent.

For a mono in $B$ with characteristic predicate $p$, closedness for $c(U)$ means $u\vee p=p$, or $u\leq p$. Density for $o(U)$ means $(u\Rightarrow p)=\top$, again $u\leq p$. Thus **the c(U)-closed monos are exactly the o(U)-dense monos**.

Both densities together force $u\leq p$ and $u\vee p=\top$, hence $p=\top$: the only jointly dense monos are isomorphisms. More explicitly, the meet of these operators is pointwise and

$$
(u\Rightarrow p)\wedge(u\vee p)=p,
$$

so $o(U)\wedge c(U)=\mathrm{id}_\Omega$.

For their join, every mono $A\hookrightarrow B$ factors through the union with the [pullback](../../../../../pullback-category-theory.md) $U_B=U\times B$:

$$
A\hookrightarrow A\cup U_B\hookrightarrow B.
$$

The first mono is c(U)-dense, because adjoining $U$ fills its codomain; the second is o(U)-dense, because its image contains $U_B$. Any [local operator](../../../../../lawvere-tierney-topology.md) above both must therefore make every mono dense, since its dense monos are closed under composition. It is the largest operator $p\mapsto\top$. Consequently

$$
\boxed{o(U)\wedge c(U)=\mathrm{id}_\Omega,\qquad o(U)\vee c(U)=\top.}
$$

These are the [complementary open and closed local operators](../../../../../complementary-open-and-closed-local-operators.md) in the ordered lattice of [local operators](../../../../../lawvere-tierney-topology.md), with order given by pointwise implication.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [Section A](../section-a.md)
3. [Paper 20](../../paper-20-split.md)
4. [Iii](../../split.md)
5. [2014](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
