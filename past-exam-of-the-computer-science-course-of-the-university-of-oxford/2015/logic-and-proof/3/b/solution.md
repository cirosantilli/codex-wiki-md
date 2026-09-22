<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First convert the four [first-order sentences](../../../../../first-order-sentence.md) to [clausal form](../../../../../clausal-form.md). In the first, pull the [existential quantifier](../../../../../existential-quantification.md) across the [logical disjunction](../../../../../logical-disjunction.md), then replace its witness by a fresh unary [Skolem function](../../../../../skolem-function.md) $f(x)$. The usual nonempty-domain convention for [first-order logic](../../../../../first-order-logic.md) makes this transformation valid even when $H(x)$ already holds. The four [Skolem normal forms](../../../../../skolem-normal-form.md) are

$$
\begin{aligned}
A'&=\forall x\,[H(x)\lor L(x,f(x))],\\
B'&=\forall x\forall y\,[\neg L(x,y)\lor L(x,\ell)],\\
C'&=\forall x\forall y\,[\neg L(y,x)\lor\neg L(x,y)\lor H(x)],\\
D'&=\forall x\,[\neg H(\ell)\lor M(x)].
\end{aligned}
$$

The [Skolemization](../../../../../skolemization.md) of $A$ preserves satisfiability in an expanded [first-order signature](../../../../../first-order-signature.md); it does not assert [logical equivalence](../../../../../logical-equivalence.md) for every arbitrary interpretation of the new [Skolem function](../../../../../skolem-function.md). The other three [first-order sentences](../../../../../first-order-sentence.md) only require elimination of implications and movement of [universal quantifiers](../../../../../universal-quantification.md).

For a [ground resolution](../../../../../ground-resolution.md) refutation, negate the desired conclusion and introduce a fresh constant $c$ for a person who is not merry. This adds the [ground clause](../../../../../ground-clause.md) $\neg M(c)$. Use these ground instances of the four universal [first-order sentences](../../../../../first-order-sentence.md):

$$
\begin{aligned}
K_1&=H(\ell)\lor L(\ell,f(\ell)),\\
K_2&=\neg L(\ell,f(\ell))\lor L(\ell,\ell),\\
K_3&=\neg L(\ell,\ell)\lor H(\ell),\\
K_4&=\neg H(\ell)\lor M(c),\\
K_5&=\neg M(c).
\end{aligned}
$$

Here $K_3$ comes from $C'$ with $x=y=\ell$, after removing a duplicate negative literal. All [first-order terms](../../../../../first-order-term.md) in these [ground clauses](../../../../../ground-clause.md) are ground. Resolving gives

$$
\begin{aligned}
K_6&=\operatorname{Res}_{L(\ell,f(\ell))}(K_1,K_2)
      =H(\ell)\lor L(\ell,\ell),\\
K_7&=\operatorname{Res}_{L(\ell,\ell)}(K_6,K_3)=H(\ell),\\
K_8&=\operatorname{Res}_{H(\ell)}(K_7,K_4)=M(c),\\
K_9&=\operatorname{Res}_{M(c)}(K_8,K_5)=\square.
\end{aligned}
$$

Repeated positive literals in $K_7$ have again been removed. The empty [ground clause](../../../../../ground-clause.md) proves unsatisfiability of the premises together with the negated conclusion. Therefore

$$
\boxed{A,B,C,D\models\forall x\,M(x).}
$$

The key is to apply the first three premises to Lucy herself: either she is already happy, or she loves somebody, hence loves herself, which forces her happiness and activates the final premise.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Logic and proof](../../../logic-and-proof-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
