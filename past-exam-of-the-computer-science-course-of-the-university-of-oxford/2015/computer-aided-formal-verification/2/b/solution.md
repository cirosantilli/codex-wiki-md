<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Denote the three families found in part (a) by $A=(s_0s_1)^\omega$, $B_n=(s_0s_1)^n s_2^\omega$ and $C_m=s_3^m s_4s_5^\omega$, where $n,m\geq1$. All are fair [paths in a transition system](../../../../../path-in-a-transition-system.md). The verdicts are

$$
\boxed{(TS\models_{\mathrm{fair}}\varphi_i)_{i=1}^6
=(\text{false},\text{false},\text{false},\text{false},\text{true},\text{false}).}
$$

Each verdict follows from the infinite [path in a transition system](../../../../../path-in-a-transition-system.md) semantics, rather than from a finite prefix alone.

For $\varphi_1=FGa$, take $C_1=s_3s_4s_5^\omega$. From $s_4$ onwards, $a$ is always false, so there is no time after which $a$ is always true. Therefore **the first specification fails**, with fair [counterexample](../../../../../counterexample.md) $C_1$. The [path in a transition system](../../../../../path-in-a-transition-system.md) $A$ is another fair [counterexample](../../../../../counterexample.md), because it encounters $s_1$, where $a$ is false, infinitely often. Each $B_n$ does satisfy $FGa$, since $s_2$ satisfies $a$ forever.

For $\varphi_2=(X\neg a)\to FGa$, take $A$. Its next [state](../../../../../state-computer-science.md) is $s_1$, so $X\neg a$ is true, but $FGa$ is false as just shown. Thus **the second specification fails**, with fair [counterexample](../../../../../counterexample.md) $A$. Alternatively, $C_1$ has next [state](../../../../../state-computer-science.md) $s_4$, making its antecedent true and its consequent false. For $C_m$ with $m\geq2$, the next [state](../../../../../state-computer-science.md) is still $s_3$, so this implication is true there because its antecedent is false; this does not rescue a universally quantified specification.

For $\varphi_3=Ga$, the fair [path in a transition system](../../../../../path-in-a-transition-system.md) $C_1$ reaches $s_4$, where $a$ is false. Thus **the third specification fails**, with fair [counterexample](../../../../../counterexample.md) $C_1$. In fact every fair initial [path in a transition system](../../../../../path-in-a-transition-system.md) reaches $s_1$ or $s_4$, so none satisfies $Ga$.

For $\varphi_4=b\mathbin{\mathrm U}G\neg b$, [strong until](../../../../../strong-until.md) requires an eventual position satisfying $G\neg b$, together with $b$ at every earlier position. On $A$, $b$ is true forever, so $G\neg b$ never holds. Thus **the fourth specification fails**, with fair [counterexample](../../../../../counterexample.md) $A$. On each $B_n$, $b$ holds until entry into $s_2$, after which $\neg b$ holds forever. On each $C_m$, $b$ holds until entry into $s_5$, after which $\neg b$ holds forever. These latter [paths in a transition system](../../../../../path-in-a-transition-system.md) satisfy the [strong until](../../../../../strong-until.md) requirement.

For $\varphi_5=b\mathbin{\mathrm W}G\neg b$, [weak until](../../../../../weak-until.md) permits either the preceding [strong until](../../../../../strong-until.md) behavior or $Gb$. Every $B_n$ and $C_m$ satisfies the [strong until](../../../../../strong-until.md) behavior, and $A$ satisfies $Gb$. These exhaust the fair initial [paths in a transition system](../../../../../path-in-a-transition-system.md). Therefore **the fifth specification holds on every fair initial path**. Allowing the left operand to continue forever is exactly what distinguishes this answer from the previous one.

For $\varphi_6=(XXb)\mathbin{\mathrm U}G\neg b$, the two [next-time operators](../../../../../next-time-operator.md) belong to the left operand of [strong until](../../../../../strong-until.md). The fair [path in a transition system](../../../../../path-in-a-transition-system.md) $C_1$ has $b$ true at positions zero and one, then false at every position from two onwards. Therefore $G\neg b$ first holds at position two. But $XXb$ is false already at position zero, since $b$ is false at position two. A witness for [strong until](../../../../../strong-until.md) cannot occur at zero or one, where its right operand is false, or at two or later, where its left operand has already failed. Thus **the sixth specification fails**, with fair [counterexample](../../../../../counterexample.md) $C_1$.

Indeed, every fair initial [path in a transition system](../../../../../path-in-a-transition-system.md) fails the sixth specification. On $A$, the right operand never holds. On $B_n$ and $C_m$, let $j\geq2$ be the first position of the permanent $\neg b$ tail. The left operand $XXb$ is false at $j-2$, strictly before any possible right-operand witness. This also checks that the two [next-time operators](../../../../../next-time-operator.md) cannot be ignored or shifted onto the whole [strong until](../../../../../strong-until.md) formula.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
