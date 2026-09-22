<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A theory is [recursively axiomatizable](../../../../../semidecidable-axiomatization.md) when it has an effective enumeration of axioms, equivalently when its deductive closure is [computably enumerable](../../../../../recursively-enumerable-set.md). If the definition requires a decidable axiom set, the equivalent formulation is obtained by replacing an axiom enumerated at stage $s$ by a fixed left-associated [logical conjunction](../../../../../logical-conjunction.md) of $s+1$ copies of it. To recognize a proposed padded axiom, inspect its finitely many possible decompositions into repeated conjuncts and check the corresponding finite enumeration stages. The padding preserves logical equivalence, so the resulting decidable axiom set generates the same theory. In either convention, enumerate [formal proofs](../../../../../formal-proof.md) using the finite sets of axioms seen so far. This effectively enumerates every theorem.

Let $T$ be a [sound arithmetic theory](../../../../../soundness-of-an-arithmetic-theory.md) of the standard [natural numbers](../../../../../natural-number.md), sufficiently strong to encode finite computations, proofs and substitution and to establish the [diagonal lemma](../../../../../diagonal-lemma.md); an extension of [Robinson arithmetic](../../../../../robinson-arithmetic.md) suffices. With a [semidecidable axiomatization](../../../../../semidecidable-axiomatization.md), the [arithmetical provability predicate](../../../../../arithmetical-provability-predicate.md) $\operatorname{Pr}_T(v)$ expresses that a proof of the sentence with code $v$ exists. A proof certificate can include enumeration stages for its axioms, so this predicate is arithmetically expressible even when the given axiom set is only [computably enumerable](../../../../../recursively-enumerable-set.md).

The [diagonal lemma](../../../../../diagonal-lemma.md) produces a sentence $G$ such that

$$
T\vdash G\longleftrightarrow\neg\operatorname{Pr}_T(\ulcorner G\urcorner).
$$

Here is the mechanism, including its effectiveness. For the computable substitution [function](../../../../../function-split.md) $d$ taking a one-variable formula code $e$ to the code of that formula with the numeral $\overline e$ substituted, let $D(v,w)$ represent its graph. Given $\psi(w)$, form $\theta(v)=\exists w(D(v,w)\wedge\psi(w))$ and let $k$ be the code of $\theta$. The sentence $\theta(\overline k)$ has code $d(k)$. Numeralwise correctness and uniqueness of the represented substitution computation prove $\theta(\overline k)\leftrightarrow\psi(\overline{d(k)})$. This constructs a fixed point effectively from the code of $\psi$. Applying it to $\psi=\neg\operatorname{Pr}_T$ gives $G$.

If $T$ proved $G$, [arithmetic soundness](../../../../../soundness-of-an-arithmetic-theory.md) would make $G$ true, while the existence of that proof would make $\operatorname{Pr}_T(\ulcorner G\urcorner)$ true. The displayed equivalence would then make $G$ false, a contradiction. Thus $T$ does not prove $G$. In the standard [natural numbers](../../../../../natural-number.md) its [arithmetical provability predicate](../../../../../arithmetical-provability-predicate.md) is therefore false at this code, so $G$ is true. [Arithmetic soundness](../../../../../soundness-of-an-arithmetic-theory.md) now rules out a proof of $\neg G$ as well. Hence **$T$ is incomplete: neither $G$ nor $\neg G$ is a theorem, and $G$ is true**.

For a fixed effective enumeration $(W_e)$ of [computably enumerable sets](../../../../../recursively-enumerable-set.md), a [productive set](../../../../../productive-set.md) $P$ has a [partial computable function](../../../../../computable-function.md) $p$ such that

$$
W_e\subseteq P\quad\Longrightarrow\quad p(e)\downarrow\ \text{ and }\ p(e)\in P\setminus W_e.
$$

The condition applies to every [computably enumerable](../../../../../recursively-enumerable-set.md) subset, including finite subsets. No condition is imposed on $p(e)$ when the inclusion fails.

Let $\mathrm{Tr}$ be the set of codes of true [arithmetic](../../../../../arithmetic-split.md) sentences; numbers which are not sentence codes are excluded. Uniformly in $e$, there is an [arithmetic](../../../../../arithmetic-split.md) formula $E_e(v)$ expressing $v\in W_e$: it says that a finite enumeration computation outputs $v$. Apply the [effective diagonal lemma](../../../../../effective-diagonal-lemma.md) to obtain $G_e$ with

$$
\mathbb N\models G_e\longleftrightarrow\neg E_e(\ulcorner G_e\urcorner),\qquad p(e)=\ulcorner G_e\urcorner.
$$

The operation producing this sentence code is total computable. Suppose $W_e\subseteq\mathrm{Tr}$. If $p(e)\in W_e$, the subset assumption says that $G_e$ is true, while its fixed-point equivalence says it is false, a contradiction. Thus $p(e)\notin W_e$. The same equivalence now says $G_e$ is true, so $p(e)\in\mathrm{Tr}$. We have proved

$$
\boxed{W_e\subseteq\mathrm{Tr}\quad\Longrightarrow\quad p(e)\in\mathrm{Tr}\setminus W_e,\qquad p\text{ is total computable}.}
$$

Therefore **[arithmetic truth](../../../../../true-arithmetic.md) is a [productive set](../../../../../productive-set.md)**. This proves [productivity of arithmetic truth](../../../../../productivity-of-arithmetic-truth.md). It cannot itself be [computably enumerable](../../../../../recursively-enumerable-set.md), since taking $W_e=\mathrm{Tr}$ would contradict the defining property. Applying the productive procedure to the enumerable theorem set of a [sound arithmetic theory](../../../../../soundness-of-an-arithmetic-theory.md) also gives a true sentence outside that theory. The productive construction does not require the enumerable subset of truths to be a theory or to be deductively closed.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
