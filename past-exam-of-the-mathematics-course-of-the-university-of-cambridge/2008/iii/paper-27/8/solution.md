<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Here “constructive [ZF](../../../../../zermelo-fraenkel-set-theory.md)” is understood as full [intuitionistic Zermelo–Fraenkel set theory](../../../../../intuitionistic-zermelo-fraenkel-set-theory.md), with power [set](../../../../../set-split.md), full separation, collection and [set](../../../../../set-split.md) induction. It is not the predicative theory CZF with restricted separation and subset collection. We construct a negative inner interpretation of classical [ZF](../../../../../zermelo-fraenkel-set-theory.md). Its classical logic belongs to the interpreted universe, not to the ambient intuitionistic universe. A bare double-negation of the ordinary [set](../../../../../set-split.md) axioms does not by itself solve the extensionality and power-set difficulties.

Work inside [IZF](../../../../../intuitionistic-zermelo-fraenkel-set-theory.md). Let $1=\{0\}$ and regard subsets of $1$ as truth values. For $p\subseteq1$, put $j(p)=\{0\in1:\neg\neg(0\in p)\}$. Define the [double-negation Boolean algebra](../../../../../double-negation-boolean-algebra.md)

$$
B=\{p\in\mathcal P(1):j(p)=p\}.
$$

Meets are intersections, joins are $j$ of unions, and complement is $\neg p=\{0\in1:0\notin p\}$. Arbitrary intersections of stable predicates are stable. The laws $\neg\neg\neg P\leftrightarrow\neg P$ and $\neg\neg(P\lor\neg P)$ give complementation, and distributing a stable conjunction through a regularized disjunction gives distributivity. Thus $B$ is a [complete Boolean algebra](../../../../../complete-boolean-algebra.md), constructively. In particular $p\vee_B\neg p=1$, even when their ordinary union is not known to be $1$.

Construct a class $W$ of [Boolean-valued names](../../../../../boolean-valued-name.md). A name has a [set](../../../../../set-split.md) of immediate subnames and a coefficient in $B$ on each; the subname relation is inductively well-founded. More concretely, take set-sized rooted-tree codes with Boolean labels on their edges, requiring that every progressive subset of their nodes contains every node. A subset is progressive when containing all children of a node implies containing that node. This set-quantified condition is definable using power [set](../../../../../set-split.md) and supplies induction for each formula by separation. On these trees recursively code each root by the function assigning its children's coded names their edge coefficients; repeated equal codes can be combined by joining their coefficients. The class of these codes is definable by the existence of such a well-founded construction tree. Every set-indexed family of names with coefficients produces another name by adjoining a new root. Collection gathers a [set](../../../../../set-split.md) of construction trees witnessing the given subnames, and gluing all these witnesses under the new root avoids choosing one witness tree for each subname; repetitions have identical codes and coefficients. Well-founded recursion on these trees collects compatible partial evaluations by collection; uniqueness identifies all overlapping evaluations, so no selection of witnesses is required. Double induction gives the corresponding recursion on pairs of trees. This avoids assuming a classical linear ordering of all constructive ordinals.

For names $a,b$, define valued membership and equality simultaneously:

$$
\begin{aligned}
\llbracket a\in b\rrbracket
&=\bigvee_{u\in\operatorname{dom}b}\bigl(b(u)\wedge\llbracket a=u\rrbracket\bigr),\\
\llbracket a=b\rrbracket
&=\left(\bigwedge_{u\in\operatorname{dom}a}
(a(u)\Rightarrow\llbracket u\in b\rrbracket)\right)
\wedge\left(\bigwedge_{v\in\operatorname{dom}b}
(b(v)\Rightarrow\llbracket v\in a\rrbracket)\right).
\end{aligned}
$$

Here $p\Rightarrow q=\neg p\vee_Bq$. Each recursive call replaces at least one argument by an immediate subname, so well-founded double recursion applies. Induction proves reflexivity, symmetry and transitivity of valued equality and its substitution laws. For example the diagonal term in the membership join gives $a(u)\le\llbracket u\in a\rrbracket$, establishing reflexivity; expanding joins and using distributivity gives transitivity and substitution at the next step.

Interpret logical connectives by the Boolean operations, and quantifiers by meets and joins over names. Although $W$ is a class, the values being joined form a subset of the [set](../../../../../set-split.md) $B$: for each fixed formula, full separation forms $\{p\in B:\exists a\in W\ (p=\llbracket\varphi(a)\rrbracket)\}$. This defines each fixed formula's truth value inductively. It does not give a uniform truth predicate for all formulas of the ambient universe. Substitution and the [complete Boolean algebra](../../../../../complete-boolean-algebra.md) laws verify the classical logical rules, including excluded middle. We now verify the [set](../../../../../set-split.md) axioms with explicit names.

The empty-domain name is empty. The name with domain $\{a,b\}$ and coefficient $1$ on both is a pair, since its membership value is $\llbracket x=a\rrbracket\vee_B\llbracket x=b\rrbracket$. For union of $a$, use domain $\bigcup_{u\in\operatorname{dom}a}\operatorname{dom}u$, with coefficient at $v$ equal to $\bigvee_u a(u)\wedge u(v)$, taking missing coefficients to be zero. The membership definition distributes to the required existential membership condition. Extensionality follows from the definition of valued equality: agreeing on the membership value of every name in particular implies both displayed inclusion conditions.

For separation, keep the domain of $a$ and replace its coefficient at $u$ by $a(u)\wedge\llbracket\varphi(u)\rrbracket$. Substitution makes membership in the resulting name equal to $\llbracket x\in a\rrbracket\wedge\llbracket\varphi(x)\rrbracket$. For power [set](../../../../../set-split.md), write $d=\operatorname{dom}a$. Every function $h:d\to B$ gives a name $a_h$ with coefficients $a(u)\wedge h(u)$. The functions form the [set](../../../../../set-split.md) $B^d$, so collect all $a_h$ as a domain with coefficient $1$. Each is a valued subset of $a$. Conversely, for an arbitrary name $c$, put $h(u)=\llbracket u\in c\rrbracket$. If $t=\llbracket c\subseteq a\rrbracket$, the membership and substitution formulas give

$$
t\le\llbracket c=a_h\rrbracket.
$$

Thus, to the full extent that $c$ is a subset of $a$, it belongs to the constructed power-set name. This proves the full power-set axiom without treating every external subset of a name as an internal subset.

The subtle point is [collection for Boolean-valued names](../../../../../collection-for-boolean-valued-names.md). For a fixed formula $\varphi(u,v)$ form by full separation the [set](../../../../../set-split.md)

$$
S=\{(u,p)\in d\times B:\exists v\in W\;
 p\le a(u)\wedge\llbracket\varphi(u,v)\rrbracket\}.
$$

Every pair in $S$ has a witness name. The ambient [axiom schema of collection](../../../../../axiom-schema-of-collection.md) supplies a [set](../../../../../set-split.md) $C$ of witness names covering all these pairs; separation discards any non-name elements. Make a name $b$ with domain $C$ and all coefficients $1$. For each $u\in d$, every value $a(u)\wedge\llbracket\varphi(u,v)\rrbracket$ occurring with an arbitrary name $v$ is itself a permissible $p$ in $S$. Its collected witness $w\in C$ has value at least $p$. Hence

$$
a(u)\wedge\bigvee_{v\in W}\llbracket\varphi(u,v)\rrbracket
\le\bigvee_{w\in C}\llbracket\varphi(u,w)\rrbracket.
$$

If $t=\llbracket\forall x\in a\,\exists y\,\varphi(x,y)\rrbracket$, this inequality says $t\wedge a(u)$ is covered by the witnesses in $b$ for every $u$. The bounded universal truth formula therefore gives $t\le\llbracket\forall x\in a\,\exists y\in b\,\varphi(x,y)\rrbracket$. This is exactly the collection axiom's implication at value $1$. It also yields replacement under a uniqueness hypothesis. We collected all Boolean portions of the existential truth; no choice of a single top-valued witness was assumed.

For infinity, form the canonical names $\check n$ recursively, with domain $\{\check m:m<n\}$ and coefficients $1$, and the name $\check\omega$ with all $\check n$ in its domain. It is inductive. For [set](../../../../../set-split.md) induction, let $p$ be the value of $\forall x[(\forall y\in x\,\psi(y))\to\psi(x)]$. Induction on the construction of a name $a$, using the bounded universal formula, gives $p\le\llbracket\psi(a)\rrbracket$ from the same inequalities for all its subnames. Consequently $p\le\llbracket\forall x\,\psi(x)\rrbracket$. Thus [set](../../../../../set-split.md) induction has value $1$, and classical logic in the interpreted universe converts it to the usual foundation axiom.

We have proved all axioms of classical [ZF](../../../../../zermelo-fraenkel-set-theory.md) in the [Boolean-valued inner universe over intuitionistic set theory](../../../../../boolean-valued-inner-universe-over-intuitionistic-set-theory.md), with bottom distinct from top. Any finite classical proof of contradiction would translate, instance by instance, to an intuitionistic proof that $0=1$ in $B$, an ambient contradiction. Therefore

$$
\boxed{\operatorname{Con}(\mathsf{IZF})\Rightarrow\operatorname{Con}(\mathsf{ZF}).}
$$

Conversely classical [ZF](../../../../../zermelo-fraenkel-set-theory.md) proves the intuitionistic [set](../../../../../set-split.md) axioms and allows their logical rules, so the consistency strengths agree. This is a proof-translation argument, not an assertion that [IZF](../../../../../intuitionistic-zermelo-fraenkel-set-theory.md) proves its own consistency. The valued construction is an inner interpretation of the same negative-model kind as the stable-set approach. Closing arbitrary [sets](../../../../../set-split.md) under the unbounded predicate $\neg\neg(x\in a)$ would require an additional double-complement axiom; the bounded truth-value construction above avoids that assumption. The distinction is discussed in [the study of double complement](https://hanuljeon95.github.io/files/doublecomplement_draft.pdf); [the treatment of intuitionistic valued models](https://academic.oup.com/book/32627/chapter-abstract/270515606) gives the broader semantic setting.

## ↑ Ancestors (10)

1. [8](../8.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
