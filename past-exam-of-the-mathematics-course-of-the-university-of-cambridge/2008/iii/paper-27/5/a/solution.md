<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here is the first incompleteness theorem in its modern consistency form: **every consistent computably enumerable theory $T$ extending [Robinson arithmetic](../../../../../../robinson-arithmetic.md) is incomplete.** The original [Gödel sentence](../../../../../../godel-sentence.md) proof assumes omega-consistency to obtain both unprovabilities; we give that proof and the strengthening that removes this assumption. We also give the second incompleteness conclusion for theories extending [Peano arithmetic](../../../../../../peano-arithmetic.md).

First arithmetize syntax. Code strings and finite derivations by [natural numbers](../../../../../../natural-number.md). If the axioms of $T$ are merely computably enumerable, include the finite enumeration certificate for each nonlogical axiom used in a proof. The resulting proof-checking relation $\operatorname{Prf}_T(p,q)$ is primitive recursive. Finite strings and computation histories are coded by finite sequences, with bounded local verification of every step; these give arithmetic formulas representing the coding operations. In [Robinson arithmetic](../../../../../../robinson-arithmetic.md) every true or false instance with fixed numeral inputs is provable with the appropriate sign. [Set](../../../../../../set-split.md)

$$
\operatorname{Prov}_T(q)=\exists p\,\operatorname{Prf}_T(p,q).
$$

The [diagonal lemma](../../../../../../diagonal-lemma.md) gives, for any formula $\theta(x)$, a sentence $D$ with $Q\vdash D\leftrightarrow\theta(\ulcorner D\urcorner)$. To see the construction, let $d(e)$ be the computable syntactic operation substituting the numeral for $e$ into the formula coded by $e$. Form the formula $\delta(x)=\theta(d(x))$, interpreting the displayed coding function through its arithmetic representation, and let $n=\ulcorner\delta\urcorner$. Then $D=\delta(\bar n)$, and $d(n)=\ulcorner D\urcorner$. The representation proves that fixed computation, giving the asserted equivalence.

Apply the [diagonal lemma](../../../../../../diagonal-lemma.md) to $\neg\operatorname{Prov}_T(x)$, obtaining

$$
T\vdash G\leftrightarrow\neg\operatorname{Prov}_T(\ulcorner G\urcorner).
$$

If $T\vdash G$, an actual finite proof has code $n$, so $Q$ proves its proof-checking instance and $T$ proves $\operatorname{Prov}_T(\ulcorner G\urcorner)$. The fixed-point equivalence gives its negation, contradicting consistency. Hence $T\nvdash G$. For each standard numeral $n$, $Q$ proves $\neg\operatorname{Prf}_T(\bar n,\ulcorner G\urcorner)$ because there is no such proof. If $T\vdash\neg G$, the equivalence gives $T\vdash\exists p\,\operatorname{Prf}_T(p,\ulcorner G\urcorner)$, contrary to omega-consistency. Thus the original proof gives two unprovabilities under that hypothesis. It also shows that $G$ is true in the standard [natural numbers](../../../../../../natural-number.md) when $T$ is consistent.

For consistency alone use the [Rosser sentence](../../../../../../rosser-sentence.md)

$$
T\vdash R\leftrightarrow
\forall p\bigl(\operatorname{Prf}_T(p,\ulcorner R\urcorner)
\to\exists q\le p\,\operatorname{Prf}_T(q,\ulcorner\neg R\urcorner)\bigr).
$$

If $T\vdash R$ with code $n$, consistency excludes every proof of $\neg R$. In particular the finitely many codes $q\le n$ all fail their primitive recursive proof tests. [Robinson arithmetic](../../../../../../robinson-arithmetic.md) verifies those finitely many failures and the actual proof at $n$, and hence proves $\neg R$, a contradiction. If $T\vdash\neg R$ with code $m$, consistency excludes every proof of $R$. For $p<m$, [Robinson arithmetic](../../../../../../robinson-arithmetic.md) verifies all the finitely many failed proof tests. For $p\ge m$, it verifies that $q=m$ is a proof of $\neg R$ with $q\le p$. The elementary arithmetic dichotomy between $p<m$ and $m\le p$ therefore proves the entire displayed condition, hence $R$, again a contradiction. Thus

$$
\boxed{T\nvdash R\quad\text{and}\quad T\nvdash\neg R.}
$$

For the [Gödel second incompleteness theorem](../../../../../../godel-second-incompleteness-theorem.md), now assume $T\supseteq\mathsf{PA}$ and use its ordinary certified proof predicate. PA formalizes proof concatenation and the verification of a coded proof, giving the derivability conditions: if $T\vdash A$ then $T\vdash\operatorname{Prov}_T(\ulcorner A\urcorner)$; and inside $T$,

$$
\operatorname{Prov}_T(\ulcorner A\to B\urcorner)\to
(\operatorname{Prov}_T(\ulcorner A\urcorner)\to\operatorname{Prov}_T(\ulcorner B\urcorner)),
\qquad
\operatorname{Prov}_T(\ulcorner A\urcorner)\to
\operatorname{Prov}_T(\ulcorner\operatorname{Prov}_T(\ulcorner A\urcorner)\urcorner).
$$

The first internal implication is certified by combining two proofs; the second is certified by producing the arithmetic proof that a given finite proof passes its check, with existential introduction. Apply them to $G\to\neg\operatorname{Prov}_T(\ulcorner G\urcorner)$. From $\operatorname{Prov}_T(\ulcorner G\urcorner)$, the two internal implications yield provability of both $\operatorname{Prov}_T(\ulcorner G\urcorner)$ and its negation, and hence provability of $\bot$. Consequently

$$
T\vdash\operatorname{Con}(T)\to\neg\operatorname{Prov}_T(\ulcorner G\urcorner)\to G,
\qquad\operatorname{Con}(T)=\neg\operatorname{Prov}_T(\ulcorner\bot\urcorner).
$$

A proof of this consistency sentence in a consistent $T$ would prove $G$, which the first argument excludes. Therefore **$\boxed{T\nvdash\operatorname{Con}(T)}$**. This concerns the standard arithmetic consistency sentence and the stated effective, arithmetic hypotheses; it is not a prohibition on proving consistency in a stronger theory.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
