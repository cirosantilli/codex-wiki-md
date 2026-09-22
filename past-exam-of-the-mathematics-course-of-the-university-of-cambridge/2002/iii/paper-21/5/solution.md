<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [saturated model](../../../../../saturated-model.md) condition in degree $\kappa$ means that a [first-order model](../../../../../model-of-a-first-order-theory.md) $M$ realizes every one-variable [complete type](../../../../../complete-type.md) over a parameter [set](../../../../../set-split.md) $A\subseteq M$ of size less than $\kappa$. Equivalently every finitely satisfiable such [complete type](../../../../../complete-type.md) is realized, since it can be extended to a [complete type](../../../../../complete-type.md). Without a specified degree, saturated usually means $|M|$-saturated. [Countable](../../../../../countable-set.md) saturation means $\aleph_1$-saturation, including [complete types](../../../../../complete-type.md) over countably many parameters.

Here is a general [saturated elementary extension theorem](../../../../../saturated-elementary-extension-theorem.md), with proof: for every infinite [regular cardinal](../../../../../regular-cardinal.md) $\kappa$, every [first-order structure](../../../../../first-order-structure.md) $M$ has a $\kappa$-saturated [elementary extension](../../../../../elementary-extension.md). At a stage $M_\alpha$, list all [complete types](../../../../../complete-type.md) over its [subsets](../../../../../subset.md) of size less than $\kappa$. There is a [set](../../../../../set-split.md) of them, since their formulas lie in a set-sized language. Add a witness constant for each [complete type](../../../../../complete-type.md) to the [elementary diagram](../../../../../elementary-diagram-of-a-structure.md) of $M_\alpha$, together with every formula in that [complete type](../../../../../complete-type.md) evaluated at its witness constant. A finite part mentions finitely many [complete types](../../../../../complete-type.md) and finitely many formulas from each; each finite conjunction is realizable in $M_\alpha$, and the witnesses for different [complete types](../../../../../complete-type.md) are unconstrained relative to each other. Thus the finite part is satisfiable. The [compactness theorem](../../../../../compactness-theorem.md) produces an [elementary extension](../../../../../elementary-extension.md) $M_{\alpha+1}$ realizing all those [complete types](../../../../../complete-type.md). At limits take elementary unions, justified by the [elementary chain theorem](../../../../../elementary-chain-theorem.md).

Iterate for $\kappa$ stages and put $N=\bigcup_{\alpha<\kappa}M_\alpha$. If $A\subseteq N$ has size below $\kappa$, regularity bounds the stages at which its elements enter, so $A\subseteq M_\alpha$ for some $\alpha<\kappa$. A [complete type](../../../../../complete-type.md) over $A$ consistent with $N$ is finitely satisfiable in $M_\alpha$: each finite conjunction is an existential formula with parameters from $M_\alpha$, and elementarity transfers its truth from $N$. The [complete type](../../../../../complete-type.md) is therefore realized in $M_{\alpha+1}$. This proves

$$
\boxed{M\preccurlyeq N,\qquad N\text{ is }\kappa\text{-saturated}.}
$$

For a singular desired degree, apply the theorem at a larger [regular cardinal](../../../../../regular-cardinal.md). If $M$ is infinite and an uncountable regular $\kappa$ satisfies $\kappa^{<\kappa}=\kappa$, with $|L|<\kappa$ and $|M|\le\kappa$, the construction can keep every stage of size $\kappa$. There are then at most $\kappa$ parameter [sets](../../../../../set-split.md) and [complete types](../../../../../complete-type.md), and downward Löwenheim-Skolem gives that size after each extension; adding $\kappa$ distinct elements initially ensures final size exactly $\kappa$. The resulting model is saturated in the unqualified sense. The cardinal-arithmetic hypothesis belongs to this size refinement, not to the general existence theorem.

An explicit [ultraproduct](../../../../../ultraproduct.md) version is useful too. In a [countable](../../../../../countable-set.md) language let $U$ be a [nonprincipal ultrafilter](../../../../../nonprincipal-ultrafilter.md) on $\omega$ and $N=\prod_{i<\omega}M_i/U$, where each factor is nonempty. Enumerate a [countable](../../../../../countable-set.md) finitely satisfiable [complete type](../../../../../complete-type.md), including its chosen parameter representatives, as $\varphi_1(x),\varphi_2(x),\ldots$. By the [Łoś theorem](../../../../../los-theorem.md), the [set](../../../../../set-split.md) $A_n$ of coordinates where the first $n$ formulas have a simultaneous witness belongs to $U$. Put

$$
B_n=\{i:i\ge n\}\cap\bigcap_{j\le n}A_j.
$$

These are decreasing members of $U$. At coordinate $i$, let $k(i)$ be the greatest $n\le i$ with $i\in B_n$, if there is one. Choose a witness to the first $k(i)$ formulas there, and an arbitrary element when there is none. For fixed $n$, every coordinate in $B_n$ has $k(i)\ge n$, so the chosen function satisfies $\varphi_n$ on a $U$-large [set](../../../../../set-split.md). Its [ultraproduct](../../../../../ultraproduct.md) class realizes the whole [complete type](../../../../../complete-type.md). A [countable](../../../../../countable-set.md) language over a [countable](../../../../../countable-set.md) parameter [set](../../../../../set-split.md) has only countably many formulas, so this proves [countable saturation of a nonprincipal ultraproduct over omega](../../../../../countable-saturation-of-a-nonprincipal-ultraproduct-over-omega.md).

For [NFU](../../../../../new-foundations-with-urelements.md), we give the [rank-indiscernible construction of an NFU model](../../../../../rank-indiscernible-construction-of-an-nfu-model.md) explicitly. [NFU](../../../../../new-foundations-with-urelements.md) has a unary predicate $S$ for [sets](../../../../../set-split.md), atoms have no members, [extensionality](../../../../../axiom-of-extensionality.md) applies to [sets](../../../../../set-split.md), and comprehension applies to every [stratified formula](../../../../../stratified-formula.md). A stratification assigns integer types to variables so that equality uses equal types and $x\in y$ requires $\operatorname{type}(y)=\operatorname{type}(x)+1$. A unary [set](../../../../../set-split.md) predicate adds no type difference.

Start with the actual [set](../../../../../set-split.md) structure $B=(V_{\omega+\omega},\in)$. This structure satisfies [extensionality](../../../../../axiom-of-extensionality.md) and every pure-membership [separation](../../../../../axiom-schema-of-specification.md) instance: the [subset](../../../../../subset.md) defined in a [set](../../../../../set-split.md) $a$ of rank below $\omega+\omega$ still has rank below $\omega+\omega$. We do not assert that $B$ satisfies [replacement](../../../../../axiom-schema-of-replacement.md) or all of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md). Expand it by [Skolem functions](../../../../../skolem-function.md). In it use the [sequence](../../../../../sequence.md) of rank objects $V_{\omega+n+6}$, $n<\omega$. For two such objects $d<e$ in [sequence](../../../../../sequence.md) order, we have

$$
d\subsetneq e,\qquad \forall x\,(x\subseteq d\Longrightarrow x\in e),
$$

with quantifiers in $B$. The second statement holds because every [subset](../../../../../subset.md) of $V_\alpha$ belongs to $V_{\alpha+1}$, and the later rank is at least $\alpha+1$.

Introduce constants $d_i$, $i\in\mathbb Z$, and require them to be order indiscernibles in the Skolem language, satisfying these two assertions whenever $i<j$. Also require $V_{\omega+5}\subseteq d_i$ for every $i$; this fixed rank object is first-order definable in $B$. Every finite part of these requirements together with $\operatorname{Th}(B^*)$ is satisfiable: color finite increasing tuples of the original rank [sequence](../../../../../sequence.md) by the truth values of the finitely many formulas mentioned, and use [Ramsey's theorem](../../../../../ramsey-s-theorem.md) to get a homogeneous [subsequence](../../../../../subsequence.md). The rank assertions hold for every increasing tuple there. The [compactness theorem](../../../../../compactness-theorem.md) gives a model of the full theory. In its [Skolem hull](../../../../../skolem-hull.md) $N$ generated by the $d_i$, the integer shift extends to an [automorphism](../../../../../automorphism.md) $j$ with $j(d_i)=d_{i+1}$, by the term-transport proof of the [Ehrenfeucht-Mostowski theorem](../../../../../ehrenfeucht-mostowski-theorem.md). Thus $N$ still satisfies [extensionality](../../../../../axiom-of-extensionality.md) and all pure-membership [separation](../../../../../axiom-schema-of-specification.md) instances, and

$$
N\models\forall x\,(x\subseteq d_i\Longrightarrow x\in d_{i+1})
\quad(i\in\mathbb Z).
$$

This is a set-sized [first-order model](../../../../../model-of-a-first-order-theory.md); no satisfaction predicate for a proper-class universe is being assumed.

Externally let $D_i=\{x\in N:N\models x\in d_i\}$. The [automorphism](../../../../../automorphism.md) bijects $D_i$ onto $D_{i+1}$. Interpret a typed structure with sort $i$ equal to $D_i$. At sort $i+1$, declare $y$ a [set](../../../../../set-split.md) exactly when $N\models y\subseteq d_i$; otherwise it is an atom. Define adjacent-sort membership by

$$
x\in_i y\quad\Longleftrightarrow\quad N\models(y\subseteq d_i\ \land\ x\in y).
$$

The guard is necessary: a typed atom might have some ordinary $N$-members in $D_i$, and those must not become its typed members. Set-extensionality follows from [extensionality](../../../../../axiom-of-extensionality.md) in $N$, because the ordinary members of a typed [set](../../../../../set-split.md) all lie in $D_i$. For any typed formula on sort $i$, its quantifiers can be restricted to the corresponding $d_l$, its [set](../../../../../set-split.md) predicates replaced by [subset](../../../../../subset.md) assertions, and its memberships replaced by the guarded relation. This is an ordinary pure-membership formula of $N$ with finitely many parameters. [Separation](../../../../../axiom-schema-of-specification.md) gives its extension $X\subseteq d_i$, and the displayed closure assertion gives $X\in d_{i+1}$. It is therefore a typed [set](../../../../../set-split.md) witnessing comprehension. The [automorphism](../../../../../automorphism.md) shifts these sorted domains and preserves the [set](../../../../../set-split.md) flags and guarded memberships.

Collapse the types onto $D_0$. Define

$$
S(y)\quad\Longleftrightarrow\quad N\models j(y)\subseteq d_0,
\qquad x\mathrel E y\quad\Longleftrightarrow\quad S(y)\ \land\ N\models x\in j(y).
$$

Objects not satisfying $S$ have no $E$-members. If two [sets](../../../../../set-split.md) have the same $E$-members, their images under $j$ are [subsets](../../../../../subset.md) of $d_0$ with the same ordinary members, so are equal by [extensionality](../../../../../axiom-of-extensionality.md) of $N$; injectivity of $j$ gives equality of the original objects.

To verify every stratified comprehension instance, assign a variable $v$ its stratification type $t(v)$ and translate its value $a\in D_0$ to $j^{t(v)}(a)\in D_{t(v)}$. Equality is preserved. An atomic $E(x,y)$ translates to the guarded adjacent-sort membership because $t(y)=t(x)+1$; the unary predicate $S(y)$ translates to $j^{t(y)}(y)\subseteq d_{t(y)-1}$. [Induction](../../../../../mathematical-induction.md) on formulas, using the domain bijections for quantifiers, preserves truth. If the free variable $x$ has type $t$, typed comprehension produces its extension $X\subseteq d_t$, with $X\in d_{t+1}$. Put $b=j^{-(t+1)}(X)\in D_0$. Then $S(b)$ holds, and for every $a\in D_0$,

$$
a\mathrel E b\quad\Longleftrightarrow\quad N\models j^t(a)\in X
\quad\Longleftrightarrow\quad \varphi(a,\vec p).
$$

This is exactly the required [NFU](../../../../../new-foundations-with-urelements.md) [set](../../../../../set-split.md). No formula containing the external [automorphism](../../../../../automorphism.md) $j$ has been used in a [separation](../../../../../axiom-schema-of-specification.md) or comprehension scheme; $j$ only transports values after the pure formula is formed.

The construction also permits the usual [infinity](../../../../../infinity.md) requirement. The ordinary $\omega$ and its successor graph $f$ are definable in $N$, hence fixed by $j$, and lie below $V_{\omega+5}$, so belong to all the required domains. Under $E$, the members of $\omega$ are still its ordinary $N$-members. The new Kuratowski pair satisfies

$$
\langle x,y\rangle_E=j^{-2}(\langle x,y\rangle_N).
$$

Since $j(f)=f$, membership of this pair in $f$ under $E$ is equivalent to $\langle x,y\rangle_N\in f$. Thus $f$ is an internal injection of $\omega$ into itself omitting zero, giving a Dedekind-infinite [set](../../../../../set-split.md).

We have built a model of [NFU](../../../../../new-foundations-with-urelements.md), with [infinity](../../../../../infinity.md) if it is included in the formulation, in ordinary [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md) metatheory:

$$
\boxed{\text{ZFC proves the existence of a model of NFU.}}
$$

In particular $\operatorname{Con}(\mathrm{ZFC})\Rightarrow\operatorname{Con}(\mathrm{NFU})$. This proof does not assume $\operatorname{Con}(\mathrm{ZFC})$ as an additional internal axiom: its starting structure is the [set](../../../../../set-split.md) $V_{\omega+\omega}$, not a model of [ZFC](../../../../../zermelo-fraenkel-set-theory-with-choice.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
