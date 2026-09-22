<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\theta=M\cap\operatorname{Ord}$ be the [ordinal height of a model of set theory](../../../../../../ordinal-height-of-a-model-of-set-theory.md). First $\theta\geq\omega_1$. Indeed, if $\theta$ were countable, the internal [axiom of choice](../../../../../../axiom-of-choice.md) would give, for every $x\in M$, a bijection in $M$ between $x$ and some ordinal below $\theta$. Such a bijection is also valid externally, making $x$ externally countable. In particular every internal rank $V_\xi^M$, $\xi<\theta$, would be countable. Every element of $M$ lies in one of these internal ranks, so

$$
M=\bigcup_{\xi<\theta}V_\xi^M
$$

would be a [countable union of countable sets](../../../../../../countable-union-of-countable-sets.md), a contradiction. This is why an [uncountable transitive set model has uncountable ordinal height](../../../../../../uncountable-transitive-set-model-has-uncountable-ordinal-height.md).

For $\xi<\theta$, [absoluteness of constructible levels](../../../../../../absoluteness-of-constructible-levels.md) gives $L_\xi^M=L_\xi$, and that level is an element of $M$. The reason is that satisfaction in a fixed set structure uses the same domain and finite formulas in both universes, so successor definitions agree; [transfinite recursion](../../../../../../transfinite-recursion.md) then also makes limit stages agree. Transitivity consequently gives

$$
L_{\omega_1}\subseteq L_\theta\subseteq M.
$$

It remains to locate a countability witness. Given an ambient [countable ordinal](../../../../../../countable-ordinal.md) $\alpha$, choose an injection $f:\alpha\to\omega$. Since $V=L$, it belongs to the [constructible universe](../../../../../../constructible-universe.md). Its [transitive closure](../../../../../../transitive-closure.md), together with $f$ itself, is countable. Choose a countable [elementary substructure](../../../../../../elementary-substructure.md) $X\prec L_\eta$ of a sufficiently large limit level containing this closure pointwise. The [condensation lemma for the constructible universe](../../../../../../condensation-lemma-for-the-constructible-universe.md) identifies the collapse with $L_\beta$ for some countable $\beta$. The collapse fixes $f$, since all its hereditary members were included. Thus $f\in L_\beta\subseteq L_{\omega_1}\subseteq M$.

The ordinal $\alpha$ itself is in $M$, since $\alpha<\omega_1\leq\theta$. Being an injection between these fixed sets is a [bounded formula in set theory](../../../../../../bounded-formula-in-set-theory.md), so $M$ recognizes $f$ as a countability witness. This proves [countable-ordinal correctness under constructibility](../../../../../../countable-ordinal-correctness-under-constructibility.md):

$$
\boxed{\alpha\in M\quad\text{and}\quad M\models\text{“}\alpha\text{ is countable”}\qquad(\alpha<\omega_1).}
$$

The use of condensation supplies a witness below the height of $M$; merely knowing that $f$ belongs somewhere to $L$ would not be sufficient.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 121](../../../paper-121-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
