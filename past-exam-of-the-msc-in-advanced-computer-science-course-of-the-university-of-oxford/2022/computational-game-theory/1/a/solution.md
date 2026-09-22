<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $X$ denote the monetary reward. Its [expected value](../../../../../expected-value-split.md) and [expected utility](../../../../../expected-utility.md) are different quantities:

$$
\mathbb E X=\frac{89}{100}+\frac{10}{10}=\boxed{1.89},\qquad
\mathbb E[u(X)]=\frac{89}{100}+\frac{100}{10}=\frac{1089}{100}=10.89.
$$

Thus indifference to a sure nonnegative reward requires $k^2=10.89$, giving **$k=3.30$ dollars**. This is the [certainty equivalent](../../../../../certainty-equivalent.md), hence the [lottery](../../../../../lottery.md)'s monetary value in the question's comparison with a sure reward. The [utility function](../../../../../utility-function-split.md) $u(x)=x^2$ is increasing and [strictly convex](../../../../../strictly-convex-function.md) on nonnegative monetary amounts. Its [certainty equivalent](../../../../../certainty-equivalent.md) exceeds its [expected value](../../../../../expected-value-split.md), $3.30>1.89$, demonstrating **[risk seeking](../../../../../risk-seeking.md)**; the same conclusion follows from the [Jensen inequality](../../../../../jensen-s-inequality.md).

The wording about paying an entry fee needs a qualification. A [certainty equivalent](../../../../../certainty-equivalent.md) compares a gross [lottery](../../../../../lottery.md) with a sure gross reward; a literal [utility indifference price](../../../../../indifference-price.md) also accounts for the fee's effect on wealth. If $u$ instead describes final wealth, with initial wealth $w$ and fee $c$, the comparison is $\mathbb E[(w-c+X)^2]=w^2$, on a domain where the [utility function](../../../../../utility-function-split.md) is increasing. Here $\operatorname{Var}(X)=7.3179$, so the nonnegative-wealth branch gives $c=w+1.89-\sqrt{w^2-7.3179}$ whenever that branch is admissible. An initial wealth and an admissible payment domain are not specified. Therefore **$3.30$ is the determined [certainty equivalent](../../../../../certainty-equivalent.md)**, while a literal wealth-dependent maximum fee is not uniquely determined. This is the distinction in [certainty equivalent and willingness to pay](../../../../../certainty-equivalent-and-willingness-to-pay.md). If negative rewards were allowed without requiring an increasing [utility function](../../../../../utility-function-split.md), the equation for $k$ also has the algebraic root $-3.30$; the usual nonnegative-reward interpretation selects the positive root.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2022](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
