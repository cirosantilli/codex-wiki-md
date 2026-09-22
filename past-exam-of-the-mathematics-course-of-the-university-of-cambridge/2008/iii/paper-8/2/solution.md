<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [uniform module](../../../../../uniform-module.md) is a nonzero module in which any two nonzero submodules intersect nontrivially. An [essential extension](../../../../../essential-extension.md) $V\subseteq E$ means that $V$ is an [essential submodule](../../../../../essential-submodule.md) of $E$: every nonzero submodule of $E$ meets $V$. Since $R$ is a [left Noetherian ring](../../../../../left-noetherian-ring.md), the finitely generated $M$ is a [Noetherian module](../../../../../noetherian-module.md).

Every nonzero [Noetherian module](../../../../../noetherian-module.md) contains a uniform submodule. Otherwise split a nonuniform submodule into two disjoint nonzero submodules, retain one for further splitting and set the other aside. If no uniform submodule is reached, the pieces set aside form an infinite direct sum, whose partial sums contradict the ascending chain condition. Now successively choose uniform submodules disjoint from the current direct sum. The process again must stop by Noetherianity, giving $V=\bigoplus_{i=1}^rV_i\subseteq M$. At termination no nonzero submodule is disjoint from $V$, so

$$
\boxed{\bigoplus_{i=1}^rV_i\ \subseteq_{\rm ess}\ M.}
$$

This proves the [finite uniform decomposition of a Noetherian module](../../../../../finite-uniform-decomposition-of-a-noetherian-module.md).

An [injective hull](../../../../../injective-hull.md) $E(M)$ is an [injective module](../../../../../injective-module.md) containing $M$ essentially. It is equivalently a minimal injective extension; we use the general existence theorem for [injective hulls](../../../../../injective-hull.md). To prove uniqueness, let $E_1,E_2$ be two hulls of $M$. Injectivity of $E_2$ extends the identity on $M$ to $f:E_1\to E_2$. Its kernel is disjoint from $M$ and therefore zero by essentiality. Its image is injective, so its inclusion splits in $E_2$. The complementary summand is disjoint from $M$, hence zero. Thus $f$ is an isomorphism fixing $M$.

A finite direct sum of [injective modules](../../../../../injective-module.md) is injective, and a finite direct sum of essential inclusions is essential. For the latter assertion, start with a nonzero vector and process its coordinates in turn: if a coordinate lies outside its specified [essential submodule](../../../../../essential-submodule.md), multiply by a ring element taking that coordinate nontrivially into that submodule. Already processed coordinates stay inside their submodules; the chosen coordinate keeps the vector nonzero. Essentiality is also transitive. Consequently both $E(M)$ and $\bigoplus_iE(V_i)$ are [injective hulls](../../../../../injective-hull.md) of $V$, so uniqueness gives

$$
\boxed{E(M)\cong\bigoplus_{i=1}^rE(V_i).}
$$

The [essential extension](../../../../../essential-extension.md) of a [uniform module](../../../../../uniform-module.md) is uniform, since intersecting any two nonzero submodules with the original [uniform module](../../../../../uniform-module.md) already gives a nonzero common intersection.

Write $E=E(V_i)$ and $S=\operatorname{End}_R(E)$. If $f\in S$ is injective, its image is isomorphic to the [injective module](../../../../../injective-module.md) $E$, hence is a direct summand. Uniformity leaves no nonzero complementary summand, so $f$ is an automorphism. Therefore the nonunits are exactly the noninjective endomorphisms. Let $J$ be their set. Two such maps have nonzero kernels, whose intersection is nonzero by uniformity; their sum kills this intersection. For a product, composition on the left preserves the original kernel. Composition on the right either has a noninjective right factor, or that factor is an automorphism and transports the original nonzero kernel. Thus $J$ is a proper two-sided ideal. Every element outside $J$ is a unit, so every nonzero residue class is invertible and every proper left or right ideal is contained in $J$. This proves the [local endomorphism ring of a uniform injective module](../../../../../local-endomorphism-ring-of-a-uniform-injective-module.md) assertion:

$$
\boxed{S/J\text{ is a division ring},\qquad J\text{ is the unique maximal ideal}.}
$$

For the whole hull, let $E_i=E(V_i)$. Its [endomorphism ring](../../../../../endomorphism-ring.md) is the ring of finite block matrices

$$
\boxed{\operatorname{End}_R(E(M))\cong
\bigl(\operatorname{Hom}_R(E_j,E_i)\bigr)_{1\le i,j\le r},}
$$

with multiplication given by summing compositions. The diagonal entries have the local rings just proved. Off-diagonal entries are homomorphism groups, not necessarily zero; in particular this ring is not generally the product of its diagonal rings. Repeated isomorphic summands give matrix blocks over their common local [endomorphism ring](../../../../../endomorphism-ring.md).

For the left regular module of $A_1(\mathbb C)$, the [Bernstein filtration](../../../../../bernstein-filtration.md) has graded ring $\mathbb C[x,\xi]$, so finite leading-term cancellation proves that $A_1$ is left and right Noetherian and a domain. Let $Q$ be its classical [division ring](../../../../../division-ring.md) of fractions. It is an [essential extension](../../../../../essential-extension.md) of $A_1$: a nonzero fraction $q=s^{-1}a$ satisfies $sq=a\ne0$ in $A_1$.

To prove that $Q$ is injective, use the [Baer criterion](../../../../../baer-criterion.md). For a homomorphism $f:I\to Q$ on a nonzero left ideal, fix $a\in I\setminus\{0\}$. For any nonzero $x\in I$, take common left multiples $sx=ta$ with $s,t\ne0$. Then $sf(x)=tf(a)$, so in the [division ring](../../../../../division-ring.md)

$$
f(x)=s^{-1}tf(a)=xa^{-1}f(a).
$$

Thus right multiplication by $a^{-1}f(a)$ extends $f$ from $I$ to $A_1$. The zero ideal is harmless. Hence $Q$ is injective and $E({}_{A_1}A_1)=Q$. For any $A_1$-linear endomorphism $F$ of $Q$, clearing the left denominator in $q$ gives $F(q)=qF(1)$. These are all right multiplications, and their composition reverses the multiplying elements. Therefore

$$
\boxed{E(M)=Q,\qquad\operatorname{End}_{A_1}({}_{A_1}Q)\cong Q^{\rm op}.}
$$

The opposite ring in the [injective hull of an Ore domain](../../../../../injective-hull-of-an-ore-domain.md) computation is essential for left-module conventions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
