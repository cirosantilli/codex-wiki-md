<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First consider the preliminary cohomological facts. The exam's term flabby means [flasque sheaf](../../../../../../flasque-sheaf.md): every restriction map is surjective. For open sets $V\subseteq U$, lift a section of $\mathcal F_3(V)$ to $\mathcal F_2(V)$ using the given surjectivity when $\mathcal F_1$ is flasque. Extend that lift to $U$ using the [flasque sheaf](../../../../../../flasque-sheaf.md) $\mathcal F_2$, then project to $\mathcal F_3(U)$. This proves that $\mathcal F_3$ is a [flasque sheaf](../../../../../../flasque-sheaf.md).

One construction of a [flasque resolution](../../../../../../flasque-resolution.md) starts with the sheaf $\mathcal C^0(\mathcal F)(U)=\prod_{P\in U}\mathcal F_P$, with pointwise restriction. It is a [sheaf of abelian groups](../../../../../../sheaf-of-abelian-groups.md) with surjective restrictions, and sending a section to all its germs embeds $\mathcal F$ in it. Repeating on the cokernels constructs an [exact sequence](../../../../../../exact-sequence.md)

$$
0\longrightarrow\mathcal F\longrightarrow\mathcal I^0\longrightarrow\mathcal I^1\longrightarrow\cdots
$$

with each $\mathcal I^j$ flasque. Define [sheaf cohomology](../../../../../../sheaf-cohomology.md) by the cohomology of the [cochain complex](../../../../../../cochain-complex.md) of global sections of such a resolution; the groups are independent of the chosen [flasque resolution](../../../../../../flasque-resolution.md). If $\mathcal F$ is itself flasque, the quotient result just proved makes every successive cokernel flasque. Applying the assumed surjectivity of sections to each successive [short exact sequence of sheaves](../../../../../../short-exact-sequence-of-sheaves.md) proves exactness of the global-section complex in positive degrees. Thus $H^i(X,\mathcal F)=0$ for $i>0$.

Now let $K=k(X)$ be the [function field](../../../../../../function-field-of-an-algebraic-variety.md) of the [smooth algebraic curve](../../../../../../smooth-algebraic-curve.md). Its [divisor class group](../../../../../../divisor-class-group.md) is

$$
\operatorname{Cl}(X)=\operatorname{Div}(X)/\operatorname{Prin}(X),\qquad
\operatorname{Div}(X)=\bigoplus_{P\text{ closed}}\mathbb ZP,\qquad
\operatorname{div}(f)=\sum_P\nu_P(f)P\quad(f\in K^*).
$$

Here $\nu_P$ is the [discrete valuation](../../../../../../discrete-valuation.md) of the [discrete valuation ring](../../../../../../discrete-valuation-ring.md) $\mathcal O_{X,P}$, and $\operatorname{Prin}(X)$ consists of the [principal divisor](../../../../../../principal-divisor-on-an-algebraic-curve.md) elements $\operatorname{div}(f)$. These sums have finite support: on a finite affine cover, represent $f$ as a fraction of regular functions; each nonzero numerator or denominator has only finitely many zeros on a curve, since a proper closed subset of a Noetherian one-dimensional irreducible space is finite.

For a [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md) $D=\sum_P n_PP$, define the [line bundle associated to a divisor](../../../../../../line-bundle-associated-to-a-divisor.md) by

$$
\mathcal O_X(D)(U)=\{f\in K:\nu_P(f)+n_P\geq0\text{ for all closed }P\in U\}\cup\{0\}.
$$

In this expression the valuation condition applies to nonzero $f$. If $t_P$ is a [uniformizer](../../../../../../uniformizer.md), the stalk is $t_P^{-n_P}\mathcal O_{X,P}$. Shrinking around $P$ removes all other zeros and poles of $t_P$ and all other points in the support of $D$, so this also gives an actual local generator. Thus $\mathcal O_X(D)$ is a [locally free sheaf](../../../../../../locally-free-sheaf.md) of rank one. Multiplication gives an isomorphism

$$
\mathcal O_X(D)\otimes_{\mathcal O_X}\mathcal O_X(E)\cong\mathcal O_X(D+E)
$$

on every stalk. If $D=\operatorname{div}(g)$, then $\mathcal O_X(D)=g^{-1}\mathcal O_X$, so the construction factors through a homomorphism $\operatorname{Cl}(X)\to\operatorname{Pic}(X)$.

It is injective: if $\mathcal O_X(D)$ is trivial, an isomorphism from $\mathcal O_X$ supplies a nonzero global rational generator $h$. At each closed point, $h$ generates $t_P^{-n_P}\mathcal O_{X,P}$, giving $\nu_P(h)=-n_P$, hence $D=-\operatorname{div}(h)$.

It is surjective: take a [line bundle](../../../../../../line-bundle.md) $\mathcal L$ and a nonzero rational section $s$, obtained by choosing a frame on any nonempty trivializing open set. If $e_i$ is a local frame, write $s=f_i e_i$ with $f_i\in K^*$. Since changes of frame are units, $\nu_P(f_i)$ is independent of the frame near $P$. A finite trivializing cover shows that these numbers have finite support. Set $D=\sum_P\nu_P(f_i)P$. The map $f\mapsto fs$ gives $\mathcal O_X(D)\cong\mathcal L$, because at $P$ the condition $\nu_P(f)+\nu_P(f_i)\geq0$ is exactly regularity of $fs$. Replacing $s$ by $gs$ changes $D$ by $\operatorname{div}(g)$, so this construction is well defined on classes. This proves the [divisor class group and Picard group of a smooth curve](../../../../../../divisor-class-group-and-picard-group-of-a-smooth-curve.md) identification

$$
\boxed{\operatorname{Cl}(X)\cong\operatorname{Pic}(X),\qquad[D]\longmapsto[\mathcal O_X(D)].}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
