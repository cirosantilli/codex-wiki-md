<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the two incoming initial arrows in the source figure: $I=\{s_0,s_3\}$. An [atomic proposition](../../../../../atomic-proposition.md) is true precisely at the [states](../../../../../state-computer-science.md) whose displayed labels contain it. In particular, $c$ is false at every [state](../../../../../state-computer-science.md). Hence $GF\neg c$ is true on every infinite [path in a transition system](../../../../../path-in-a-transition-system.md), and the first implication in the [fairness assumption](../../../../../fairness-assumption.md) imposes no restriction.

Write $p=a\land b$. The remaining implication is $FGp\to GF\neg b$. By the [linear temporal logic](../../../../../linear-temporal-logic.md) duality $\neg FGp=GF\neg p$, it is equivalent to

$$
GF\neg p\lor GF\neg b=GF\neg p,
$$

since $\neg b$ implies $\neg p$. Thus **a path is fair exactly when it visits states not labelled with both $a$ and $b$ infinitely often**. This condition also follows directly: if $p$ eventually holds forever, then $b$ eventually holds forever and the required $GF\neg b$ is impossible; if $p$ does not eventually hold forever, the implication has a false antecedent.

Every initial [path in a transition system](../../../../../path-in-a-transition-system.md) in the upper component either alternates forever between $s_0$ and $s_1$, or makes finitely many alternations and then stays at $s_2$. These are all fair: the first visits $s_1$ infinitely often, and the second visits $s_2$ infinitely often; neither [state](../../../../../state-computer-science.md) satisfies $a\land b$.

In the lower component, a [path in a transition system](../../../../../path-in-a-transition-system.md) can stay at $s_3$ forever, or leave it after finitely many visits and pass through $s_4$ to $s_5$. The constant [path in a transition system](../../../../../path-in-a-transition-system.md) $s_3^\omega$ is unfair because $a\land b$ holds forever while $\neg b$ never holds. Every departing [path in a transition system](../../../../../path-in-a-transition-system.md) is fair because $s_5$ satisfies neither $a$ nor $b$. Here $v^\omega$ means infinite repetition of the finite word $v$. Therefore

$$
\boxed{\begin{aligned}
\operatorname{FairPaths}(TS)={}&\{(s_0s_1)^\omega\}\\
&\cup\{(s_0s_1)^n s_2^\omega:n\geq1\}\\
&\cup\{s_3^m s_4s_5^\omega:m\geq1\}.
\end{aligned}}
$$

This notation lists initial [paths in a transition system](../../../../../path-in-a-transition-system.md). If one instead allows arbitrary starting [states](../../../../../state-computer-science.md), their suffixes starting at $s_1,s_2,s_4,s_5$ are fair as well; the fair [paths in a transition system](../../../../../path-in-a-transition-system.md) from each initial [state](../../../../../state-computer-science.md), and hence all verdicts below, are unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
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
