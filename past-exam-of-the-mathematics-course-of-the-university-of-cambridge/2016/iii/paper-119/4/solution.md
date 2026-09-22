<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an [adjunction](../../../../../adjoint-functors.md) $F:\mathcal C\rightleftarrows\mathcal D:G$ with [unit and counit of an adjunction](../../../../../unit-and-counit-of-an-adjunction.md) $\eta,\varepsilon$, the [monad induced by an adjunction](../../../../../monad-induced-by-an-adjunction.md) is $T=GF$, with multiplication $\mu=G\varepsilon F$. Its [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) is

$$
K:\mathcal D\to\mathcal C^T,\qquad K(D)=(GD,G\varepsilon_D),\qquad K(f)=Gf.
$$

Here $\mathcal C^T$ is the [Eilenberg-Moore category](../../../../../eilenberg-moore-category.md). If $\mathcal D$ has [reflexive coequalizers](../../../../../reflexive-coequalizer.md), the [Left adjoint to the Eilenberg-Moore comparison functor](../../../../../left-adjoint-to-the-eilenberg-moore-comparison-functor.md) is defined on an [algebra for a monad](../../../../../algebra-for-a-monad.md) $(A,a)$ by

$$
FTA\mathrel{\substack{\xrightarrow{Fa}\\[-2pt]\xrightarrow[\varepsilon_{FA}]{} }}FA\longrightarrow L(A,a),
$$

where the last arrow is a [coequalizer](../../../../../coequalizer.md). The parallel pair has common section $F\eta_A$, so it is a [reflexive pair](../../../../../reflexive-pair.md). The [coequalizer](../../../../../coequalizer.md) property induces $L$ on algebra morphisms and gives $L\dashv K$.

Starting with $K_0=G$, iterate this construction: if $L_i\dashv K_i:\mathcal D\to\mathcal E_i$, put $\mathcal E_{i+1}=\mathcal E_i^{K_iL_i}$ and let $K_{i+1}:\mathcal D\to\mathcal E_{i+1}$ be its comparison. The **[monadic length](../../../../../monadic-length.md)** is the least $\ell$ for which $K_\ell$ is an [equivalence of categories](../../../../../equivalence-of-categories.md). Thus an equivalence has length zero, and an already [monadic adjunction](../../../../../monadic-adjunction.md) whose right adjoint is not an equivalence has length one. The assumed [reflexive coequalizers](../../../../../reflexive-coequalizer.md) ensure the needed left adjoints; in the example we identify them explicitly.

For the [nested partial unary operation category](../../../../../nested-partial-unary-operation-category.md) $\mathcal C_n$, write

$$
A_n=\{a\in A:\alpha_n(a)\text{ is defined and equals }a\}\quad(n\geq1).
$$

For the empty list of operations, take $\mathcal C_0=\mathbf{Set}$ and $A_0=A$. We use positive chain indices $k\geq1$ for new points, so the index zero already labels the copy of $A$. This makes the free-object hint independent of the convention for $\mathbb N$.

For $n\geq1$, the [free extension of nested partial unary operations](../../../../../free-extension-of-nested-partial-unary-operations.md) $F_nA$ has underlying set

$$
(A\times\{0\})\amalg(A_n\times\mathbb N_{>0}).
$$

Keep the old operations on the zero layer. On new points define only

$$
\alpha_1(a,k)=(a,k+1)\quad(k\geq1),
$$

and leave every $\alpha_i$, $2\leq i\leq n$, undefined there. Define the new top operation by

$$
\alpha_{n+1}(a,0)=(a,1)\quad(a\in A_n),
$$

and leave it undefined elsewhere. These are precisely the permitted domains: the first unary operation on every new point moves it, so none of the higher operations is defined there. When $n=0$, take $F_0A=A\times\mathbb N_{\geq0}$ with $\alpha_1(a,k)=(a,k+1)$. In either case the unit is $a\mapsto(a,0)$.

For $B\in\mathcal C_{n+1}$, let its operations be $\beta_i$. Any $\mathcal C_n$ morphism $f:A\to G_nB$ extends uniquely to

$$
\bar f(a,0)=f(a),\qquad
\bar f(a,k)=\beta_1^{k-1}\bigl(\beta_{n+1}(f(a))\bigr)\quad(a\in A_n,\ k\geq1).
$$

The value $\beta_{n+1}(f(a))$ is defined because $f$ preserves the previous fixed-point equations. The extension respects the top operation at old fixed points and respects the first operation along each new chain; there are no other defined operations on those chains to check. Uniqueness follows from the same forced formulas. For $n=0$ the formula is $\bar f(a,k)=\beta_1^k(f(a))$. These extensions are natural and prove

$$
\boxed{F_n\dashv G_n.}
$$

On a morphism $f$ the free [functor](../../../../../functor.md) sends $(a,k)$ to $(f(a),k)$.

Crucially, **the top operation of $F_nA$ has no fixed points**: its defined old values move to new points, and it has no defined new values when $n\geq1$; for $n=0$ it is the shift. The next free extension therefore adds no points and equips the object with an everywhere-undefined next operation. The same remains true at every subsequent free extension. Hence, for $m>n$, the composite left adjoint $F_{m-1}\cdots F_n$ has the same first $n+1$ operations and underlying set as $F_n$.

This agreement includes the [monad](../../../../../monad.md) structure, not just its underlying [endofunctor](../../../../../endofunctor.md). The units are the same zero-layer inclusions. The composite counit on an object of $\mathcal C_m$ is the same forced extension formula, depending only on its first $n+1$ operations. Applying the composite forgetful [functor](../../../../../functor.md) therefore gives the same multiplication $G_n\varepsilon F_n$. Thus

$$
\boxed{G_n\cdots G_{m-1}F_{m-1}\cdots F_n\cong G_nF_n\text{ as monads on }\mathcal C_n.}
$$

Next prove creation of the required [split coequalizers](../../../../../split-coequalizer.md). Suppose $f,g:B\rightrightarrows C$ are arrows in $\mathcal C_{n+1}$ and their images have a split [coequalizer](../../../../../coequalizer.md) $q:C\to Q$ in $\mathcal C_n$. Choose the splitting orientation

$$
qs=1_Q,\qquad ft=1_C,\qquad gt=sq,\qquad qf=qg,
$$

with $s:Q\to C$, $t:C\to B$ morphisms in $\mathcal C_n$. Denote the top operations on $B,C$ by $b,c$. For $z\in Q_n$ define

$$
\gamma(z)=q\bigl(c(s(z))\bigr).
$$

Since $s$ preserves the lower operations, $s(z)\in C_n$ and this value exists. For $y\in C_n$, $t(y)\in B_n$, so preservation by $f,g$ gives

$$
q\bigl(c(y)\bigr)=qf\bigl(b(t(y))\bigr)
=qg\bigl(b(t(y))\bigr)=q\bigl(c(sq(y))\bigr)
=\gamma(q(y)).
$$

Thus $q$ respects the top operation. The splitting $s$ and $qs=1$ also show that this is the unique operation on its prescribed domain $Q_n$ for which $q$ is a morphism. For $n=0$ all these domains mean the whole underlying set.

If $u:C\to D$ is a $\mathcal C_{n+1}$ morphism equalizing $f,g$, its unique factor $v:Q\to G_nD$ in $\mathcal C_n$ satisfies, on $Q_n$,

$$
v\gamma(z)=u\bigl(c(s(z))\bigr)=d(u(s(z)))=d(v(z)),
$$

where $d$ is the top operation of $D$. Hence $v$ is a $\mathcal C_{n+1}$ morphism. This proves **$G_n$ creates [coequalizers](../../../../../coequalizer.md) of $G_n$-split pairs**.

Moreover, $G_n$ reflects [isomorphisms](../../../../../isomorphism.md): an isomorphism of the first $n$ operations reflects their fixed-point conditions, hence the domain of the next operation; the inverse of a bijective top-operation-preserving map then preserves that operation too. The [Beck monadicity theorem](../../../../../beck-s-monadicity-theorem.md) now gives

$$
\mathcal C_n^{G_nF_n}\simeq\mathcal C_{n+1}.
$$

Under this equivalence, the first [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) for the long composite is exactly forgetting all operations after the $(n+1)$st: its algebra structure is the top-operation extension formula already computed. Repeating the argument identifies its monadic tower with the successive categories

$$
\mathcal C_n,\ \mathcal C_{n+1},\ \ldots,\ \mathcal C_m.
$$

At each stage the corresponding comparison has the remaining composite of the already constructed free extensions as a [left adjoint](../../../../../adjoint-functors.md).

No earlier stage can be an [equivalence of categories](../../../../../equivalence-of-categories.md). For $j<m$, take the two-point set with its first $j$ operations all identities. One extension to $\mathcal C_m$ has every later operation the identity; another has its $(j+1)$st operation interchange the two points, and all subsequent operations undefined. Both have the same image in $\mathcal C_j$, but the identity function between those images is not a morphism between the extensions. Thus forgetting from $\mathcal C_m$ to $\mathcal C_j$ is not full. The final comparison at $j=m$ is an equivalence. This proves the [monadic tower for nested partial unary operations](../../../../../monadic-tower-for-nested-partial-unary-operations.md) has

$$
\boxed{\text{monadic length }m-n.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
