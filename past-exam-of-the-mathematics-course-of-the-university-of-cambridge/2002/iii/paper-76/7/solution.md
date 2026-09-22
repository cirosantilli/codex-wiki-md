<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Use the [pointed complete partial order](../../../../../pointed-complete-partial-order.md) convention: a [partially ordered set](../../../../../partially-ordered-set.md) has a least element and every nonempty [directed set](../../../../../directed-set.md) has a [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md). The argument also works for the convention requiring only suprema of increasing countable chains. The [function space of complete partial orders](../../../../../function-space-of-complete-partial-orders.md) $[D\to E]$ consists of [Scott continuous maps](../../../../../scott-continuous-map.md), namely monotone maps preserving directed suprema, ordered pointwise. Its least element is the constant map with value $\bot_E$.

For a directed family $\{f_i\}$, define $f(x)=\sup_i f_i(x)$. This is its [pointwise directed supremum](../../../../../pointwise-directed-supremum.md) and is monotone. If $A\subseteq D$ is directed, then

$$
f(\sup A)=\sup_i f_i(\sup A)=\sup_i\sup_{a\in A}f_i(a)=\sup_{a\in A}\sup_i f_i(a)=\sup_{a\in A}f(a).
$$

The interchange is justified because $\{f_i(a):i,a\}$ is directed: choose a common upper map and a common upper input. Thus $f$ is Scott continuous, proving that **$[D\to E]$ is a cpo**. Evaluation is also jointly Scott continuous: for a directed family $(f_i,x_i)$, the pairs of independently chosen indices are cofinal in a common larger index, so $(\sup_i f_i)(\sup_i x_i)=\sup_i f_i(x_i)$. The same pointwise calculation proves continuity of currying.

Suppose the continuous maps $e:[D\to D]\to D$, $p:D\to[D\to D]$ satisfy $p\circ e=\mathrm{id}$. Define

$$
\boxed{a\cdot b=p(a)(b).}
$$

For an environment $\rho$, interpret a variable by $\rho(x)$, application by $\cdot$, and an abstraction by

$$
\llbracket\lambda x.M\rrbracket_\rho=e\bigl(d\mapsto\llbracket M\rrbracket_{\rho[x:=d]}\bigr).
$$

Induction on syntax, using evaluation, currying and continuity of $e,p$, shows that every environment-dependent interpretation is Scott continuous, so this abstraction is defined. A further syntax induction proves the substitution lemma

$$
\llbracket M[x:=N]\rrbracket_\rho=\llbracket M\rrbracket_{\rho[x:=\llbracket N\rrbracket_\rho]}.
$$

For abstraction the bound variable is first renamed fresh. Consequently $p(e(f))=f$ proves the beta equation for every environment. Consistent renaming proves alpha invariance, and the compositional interpretation respects all contexts. This is a [lambda model](../../../../../lambda-model.md). A retraction alone does not assert $e\circ p=\mathrm{id}$, so [eta conversion](../../../../../eta-conversion.md) need not be valid.

For the [graph model of lambda calculus](../../../../../graph-model-of-lambda-calculus.md), take $P\omega=\mathcal P(\mathbb N)$ with inclusion, bottom $\varnothing$ and directed supremum equal to union. Let $e_k$ be the finite set of positions of one-bits in $k$, and choose the [pairing function](../../../../../pairing-function.md)

$$
\langle k,n\rangle=\frac{(k+n)(k+n+1)}2+n.
$$

Define

$$
p(a)(b)=a\cdot b=\{n:\exists k\;(e_k\subseteq b\ \text{and}\ \langle k,n\rangle\in a)\},\qquad e(f)=\{\langle k,n\rangle:n\in f(e_k)\}.
$$

A finite witness $e_k$ lies in one member of any directed union containing it, proving continuity in $b$; a graph entry lies in one member of any directed union of graphs, proving continuity in $a$. The displayed definition of $e$ preserves pointwise directed unions as well. Finally

$$
p(e(f))(b)=\bigcup_{e_k\subseteq b}f(e_k)=f(b),
$$

since the finite subsets of $b$ are directed with union $b$. This proves the retraction and all claimed model properties. The composite $e\circ p$ generally enlarges a graph by adding entries with larger finite-input witnesses; it is not generally the identity.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
