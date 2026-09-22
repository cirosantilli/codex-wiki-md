<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [preframe](../../../../../preframe.md) has finite meets and joins of nonempty [directed sets](../../../../../directed-set.md), with finite meets distributing over these joins. A [preframe](../../../../../preframe.md) homomorphism preserves both operations. Its [preframe tensor product](../../../../../preframe-tensor-product.md) $P\#Q$ has generators $p\#q$ and relations making $(p,q)\mapsto p\#q$ a homomorphism separately in each variable. Equivalently,

$$
\operatorname{PFrm}(P\#Q,R)\cong\{\beta:P\times Q\to R:\beta\text{ preserves finite meets and directed joins separately}\}.
$$

In particular $1\#q=p\#1=1$. The tensor unit is the free [preframe](../../../../../preframe.md) on one generator: classically it is $\mathbf2$, and constructively it is the [frame](../../../../../complete-heyting-algebra.md) $\Omega$ of truth values, with generator $0$.

Regard a [frame](../../../../../complete-heyting-algebra.md) $L$ as a commutative [monoid object](../../../../../monoid-object.md) in [preframes](../../../../../preframe.md), with multiplication $x*y=x\vee y$ and unit $0$. Binary [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) preserves finite meets and directed joins separately. Conversely take a commutative [monoid object](../../../../../monoid-object.md) $(M,*,e)$ in [preframes](../../../../../preframe.md) and put

$$
R(M)=\{x\in M:e\leq x,\ x*x=x\}.
$$

This set contains $e$ and $1$, since preservation of the empty [meet](../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) gives $1*x=1$. If $x,y\in R(M)$, then $x*y\geq x,y$, and

$$
(x\wedge y)*(x\wedge y)=(x*x)\wedge(x*y)\wedge(y*x)\wedge(y*y)=x\wedge y.
$$

Thus finite meets are inherited. If $D\subseteq R(M)$ is nonempty and directed, separate preservation of directed joins gives

$$
\left(\bigvee D\right)*\left(\bigvee D\right)=\bigvee_{d,d'\in D}d*d'=\bigvee D,
$$

because a common upper bound $t\in D$ gives $d*d'\leq t*t=t$. Directed joins are inherited too. Associativity and commutativity show that $x*y$ is [idempotent](../../../../../idempotent.md); it is the least [idempotent](../../../../../idempotent.md) upper bound of $x,y$. Therefore $e$ is the bottom and $*$ is binary [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) on $R(M)$. Arbitrary joins are directed joins of finite products, including the empty product $e$. Finally

$$
(x\wedge y)*(x\wedge z)=(x*x)\wedge(x*z)\wedge(y*x)\wedge(y*z)=x\wedge(y*z),
$$

so binary distributivity, together with directed distributivity, proves that $R(M)$ is a [frame](../../../../../complete-heyting-algebra.md).

A homomorphism from a [frame](../../../../../complete-heyting-algebra.md) [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) monoid to $M$ sends every element to an [idempotent](../../../../../idempotent.md) above $e$ and therefore factors uniquely through $R(M)$. The factor preserves finite joins and directed joins, hence arbitrary joins. Conversely the inclusion $R(M)\to M$ preserves the [preframe](../../../../../preframe.md) and [monoid](../../../../../monoid.md) operations. Also a [preframe](../../../../../preframe.md) monoid homomorphism between [frames](../../../../../complete-heyting-algebra.md) is automatically a [frame homomorphism](../../../../../frame-homomorphism.md). This proves the full embedding and its [right adjoint](../../../../../adjoint-functors.md): **$\mathbf{Frm}$ is a [coreflective subcategory](../../../../../coreflective-subcategory.md) of $\mathbf{CMon}(\mathbf{PFrm})$**, with coreflector $R$.

The [coproduct](../../../../../coproduct.md) of commutative [monoid objects](../../../../../monoid-object.md) in a [symmetric monoidal category](../../../../../symmetric-monoidal-category.md) is their tensor: the maps are $x\mapsto x\#e_N$, $y\mapsto e_M\#y$, and a pair $f,g$ induces $x\#y\mapsto f(x)*g(y)$. For two [frames](../../../../../complete-heyting-algebra.md) $L,K$, the induced multiplication on pure generators is

$$
(a\#b)*(a'\#b')=(a\vee a')\#(b\vee b'),\qquad e=0\#0.
$$

Every pure generator is [idempotent](../../../../../idempotent.md) and above $e$. Those properties are preserved by finite meets and directed joins, as just proved, so hold throughout the generated [preframe](../../../../../preframe.md). It is therefore already a [frame](../../../../../complete-heyting-algebra.md), rather than requiring a further coreflection. Consequently

$$
\boxed{L\amalg_{\mathbf{Frm}}K=L\#_{\mathbf{PFrm}}K,\qquad a\#b=i_L(a)\vee i_K(b).}
$$

Rectangles in the localic product are instead $i_L(a)\wedge i_K(b)=(a\#0)\wedge(0\#b)$.

For a [filtered colimit in a category](../../../../../filtered-colimit-in-a-category.md) of [frames](../../../../../complete-heyting-algebra.md), form the colimit $P$ in [preframes](../../../../../preframe.md), with stage maps $i_j$. It can be presented by stage elements, all their finite-meet and directed-join relations, and the transition relations. Since tensoring is a [left adjoint](../../../../../adjoint-functors.md), it preserves colimits. Filteredness makes the diagonal diagram cofinal in the product index diagram, so the stage multiplications induce $P\#P\to P$. The units agree. Each stage element is [idempotent](../../../../../idempotent.md) above the common unit; generation again implies $P=R(P)$. The resulting [frame](../../../../../complete-heyting-algebra.md) is the [filtered colimit in a category](../../../../../filtered-colimit-in-a-category.md) in $\mathbf{Frm}$; its binary [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) is induced by computing two representatives at a common later stage. Thus **binary coproducts and filtered colimits of [frames](../../../../../complete-heyting-algebra.md) are computed in [preframes](../../../../../preframe.md)**, with the indicated induced [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) operation.

We now prove compactness. For a [compact locale](../../../../../compact-locale.md), its [frame](../../../../../complete-heyting-algebra.md) $L$ has a top test $q_L:L\to\Omega$, $q_L(a)=[a=1]$, preserving finite meets and directed joins. For compact $L,K$, tensor the tests and use the unit isomorphism $\Omega\#\Omega\cong\Omega$ to obtain a [preframe](../../../../../preframe.md) map $q:L\#K\to\Omega$ with

$$
q(a\#b)=[a=1]\vee[b=1].
$$

It reflects top on every pure generator. The property $q(x)=1\Longrightarrow x=1$ is closed under finite meets and directed joins: for a directed [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md), preservation of the [join](../../../../../least-upper-bound-in-a-partially-ordered-set.md) says that its truth value is the existential disjunction of the individual truth values, so some term has value $1$. Since pure generators generate the [preframe](../../../../../preframe.md), $q$ reflects top everywhere. Applying $q$ to a directed cover of $1$ therefore shows that a term of that cover is $1$. This proves compactness of the binary coproduct [frame](../../../../../complete-heyting-algebra.md), hence of the binary product [locale](../../../../../locale.md).

For a filtered diagram of compact [frames](../../../../../complete-heyting-algebra.md), define on stage $j$

$$
q_j(a)=[\text{there is an arrow }j\to k\text{ for which }a\text{ becomes }1\text{ at stage }k].
$$

These truth-valued maps preserve finite meets: witnesses can be taken to a common later stage, using filteredness. They preserve directed joins: compactness at the witnessing later stage selects a member of the directed family. They are compatible with transitions, again by filteredness, so induce a [preframe](../../../../../preframe.md) map $q:P\to\Omega$. On stage generators, $q(i_j(a))=1$ implies $i_j(a)=1$. The same generation argument proves that $q$ reflects top throughout $P$. Thus the filtered colimit [frame](../../../../../complete-heyting-algebra.md) is compact.

Finally the arbitrary [coproduct](../../../../../coproduct.md) of the [frames](../../../../../complete-heyting-algebra.md) $\mathcal O(X_i)$ is the filtered colimit of their finite coproducts, indexed by finite subsets of the index set; the empty finite coproduct is $\Omega$, itself compact. Finite coproducts are compact by the binary argument, and their filtered colimit is compact by the preceding paragraph. Opposing the categories gives

$$
\boxed{\prod_{i\in I}X_i\text{ is compact whenever every }X_i\text{ is compact}.}
$$

This proves the [localic Tychonoff theorem](../../../../../localic-tychonoff-theorem.md) through [preframes](../../../../../preframe.md), without choosing points or invoking the [axiom of choice](../../../../../axiom-of-choice.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 20](../../paper-20-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
