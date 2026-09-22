<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use [relative constructible level recognition](../../../../../../relative-constructible-level-recognition.md). The finite coding conditions matter here: merely writing “every set is relatively constructible” inside an arbitrary [transitive set](../../../../../../transitive-set.md) does not ensure that its computations are correct.

Let $\mathsf A$ be a single finite conjunction expressing [finite relation closure for set-theoretic coding](../../../../../../finite-relation-closure-for-set-theoretic-coding.md). Concretely require the empty [set](../../../../../../set-split.md), pairing, [set union](../../../../../../set-union.md), [set difference](../../../../../../set-difference.md), [Cartesian products](../../../../../../cartesian-product.md), and the following uniform relation operations: for each finite [ordinal](../../../../../../ordinal.md) $n$ and each [set](../../../../../../set-split.md) $A$, the set $A^n$ of finite tuples exists; relations on these tuple domains can be complemented, intersected, projected along a coordinate and pulled back along finite coordinate maps; the equality and membership relations restricted to $A^2$ exist. These are finitely many first-order closure assertions with $n$ quantified, not an axiom schema. Each operation is specified by its usual elementwise membership equivalence. Transitivity makes the operations correct externally. Finite tuple domains are also correct: every individual finite tuple is already present by pairing and union.

These conditions make [satisfaction for a set structure](../../../../../../satisfaction-for-a-set-structure.md) absolute. For a fixed coded [first-order formula](../../../../../../first-order-formula.md), compute its truth relations on $A^n$ by induction: equality and membership give the atomic cases, [relative complement](../../../../../../set-difference.md) gives [negation](../../../../../../negation.md), intersection gives [logical conjunction](../../../../../../logical-conjunction.md), and projection gives existential quantification. All required truth tables exist by $\mathsf A$ and agree with the actual ones. Thus the first-order assertion $B=\operatorname{Def}(A)$ is absolute whenever $A,B$ belong to a transitive structure satisfying $\mathsf A$: require that each member of $B$ has such a finite formula-and-parameter definition, and that each coded definition contributes a member of $B$. Codes are finite objects; no truth predicate for the ambient universe is being used.

Write $S_x(\xi,B)$ for the [coded relative constructible stage](../../../../../../coded-relative-constructible-stage.md) assertion: $\xi$ is an [ordinal](../../../../../../ordinal.md) and there is a function $f$ with domain $\xi+1$, with $f(0)=x$, $f(\eta+1)=\operatorname{Def}(f(\eta))$, $f(\lambda)=\bigcup_{\eta<\lambda}f(\eta)$ at nonzero [limit ordinals](../../../../../../limit-ordinal.md), and $f(\xi)=B$. Under $\mathsf A$, any such internal code is correct by [transfinite induction](../../../../../../transfinite-induction.md). Restrictions of a code to shorter domains exist by the relation operations. Define the one-free-variable [first-order formula](../../../../../../first-order-formula.md)

$$
\boxed{\begin{aligned}
\Phi(x):={}&\mathsf A\ \land\ x\text{ is transitive}\\
&\land\ \forall y\,\exists\xi\,\exists B\,(S_x(\xi,B)\land y\in B)\\
&\land\ \forall\xi\,\forall B\,(S_x(\xi,B)\Rightarrow\exists\eta\,\exists C\,(\xi<\eta\land S_x(\eta,C))).
\end{aligned}}
$$

All displayed abbreviations expand into [first-order formulas](../../../../../../first-order-formula.md) of the membership language.

Suppose $M$ is transitive, $X\in M$, and $M\models\Phi(X)$. Let $I$ be the externally defined set of indices of stage codes in $M$. It contains $0$, is downward closed by restricting codes, and has no largest member by the last conjunct. Thus $I$ is a nonzero [limit ordinal](../../../../../../limit-ordinal.md) $\alpha$. Correctness of stage codes gives $L_\xi(X)\in M$ for $\xi<\alpha$, hence $L_\xi(X)\subseteq M$ by transitivity. Conversely the exhaustion conjunct puts every $y\in M$ in some such level. Therefore

$$
M=\bigcup_{\xi<\alpha}L_\xi(X)=L_\alpha(X).
$$

For the converse, every $L_\alpha(X)$ with nonzero limit $\alpha$ satisfies $\mathsf A$: each listed operation on parameters from one level is definable at finitely many later levels, still below $\alpha$. Moreover [stage histories appear below every limit constructible level](../../../../../../stage-histories-appear-below-every-limit-constructible-level.md). Here is the essential limit step of that lemma. If the histories $f_\eta$ for $\eta<\lambda$ are available in $L_\lambda(X)$, the correct predicate $S_X$ defines their graph of endpoints as a subset of $L_\lambda(X)$. No endpoint $L_\eta(X)$ with $\eta\geq\lambda$ can belong to $L_\lambda(X)$, because $L_\lambda(X)\subseteq L_\eta(X)$ would then give $L_\eta(X)\in L_\eta(X)$, contradicting [Axiom of foundation](../../../../../../axiom-of-regularity.md). The defined graph therefore has domain exactly $\lambda$. Adjoining its final pair $(\lambda,L_\lambda(X))$ takes finitely many more stages. Together with finite successor extensions, this proves by [transfinite induction](../../../../../../transfinite-induction.md) that every $f_\xi$ belongs to $L_{\xi+k}(X)$ for some finite $k$.

Thus all histories for $\xi<\alpha$ belong to $L_\alpha(X)$. Exhaustion follows from continuity, and $\xi+1<\alpha$ supplies a larger represented stage. Hence $L_\alpha(X)\models\Phi(X)$, proving both directions without assuming [ZF](../../../../../../zermelo-fraenkel-set-theory.md) for the arbitrary input structure $M$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
