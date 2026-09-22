<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**$\ell_2\succ\ell_1$.** The distinction is small but strict: their normalized [expected utilities](../../../../../expected-utility.md) are $18/25$ and $7/10$, respectively.

By the [Von Neumann-Morgenstern utility theorem](../../../../../von-neumann-morgenstern-utility-theorem.md), use a representing [utility function](../../../../../utility-function-split.md) and apply a positive [affine function](../../../../../affine-function.md) to set $u(\omega_1)=1$ and $u(\omega_4)=0$. This is possible because the given [strict preference](../../../../../strict-preference.md) implies $u(\omega_1)>u(\omega_4)$. The two specified [indifference relations](../../../../../indifference-relation.md) then give

$$
u(\omega_3)=\frac35,\qquad u(\omega_2)=\frac34+\frac14\frac35=\frac9{10}.
$$

Taking the [expected utility](../../../../../expected-utility.md) of each [lottery](../../../../../lottery.md) yields

$$
U(\ell_1)=\frac25+\frac15\frac9{10}+\frac15\frac35=\frac7{10},\qquad
U(\ell_2)=\frac25\frac9{10}+\frac35\frac35=\frac{18}{25}.
$$

Their difference is $1/50>0$, establishing the stated [strict preference](../../../../../strict-preference.md). These numbers measure [utility](../../../../../utility.md), not monetary reward or an assumed ordering of the subscripts.

Here is the underlying argument directly in terms of the axioms. The [independence axiom for lottery preferences](../../../../../independence-axiom-for-lottery-preferences.md) permits [substitution of indifferent lotteries](../../../../../substitution-of-indifferent-lotteries.md) inside a common mixture. Replacing $\omega_3$ by its given mixture of $\omega_1,\omega_4$, and then replacing $\omega_2$, followed by [reduction of compound lotteries](../../../../../reduction-of-compound-lotteries.md), gives

$$
\omega_2\sim\frac9{10}\omega_1+\frac1{10}\omega_4,
$$

and consequently

$$
\ell_1\sim\frac7{10}\omega_1+\frac3{10}\omega_4,
\qquad
\ell_2\sim\frac{18}{25}\omega_1+\frac7{25}\omega_4.
$$

The [transitive relation](../../../../../transitive-relation.md) axiom combines the successive substitutions. Finally, [mixture monotonicity](../../../../../mixture-monotonicity.md) says that among mixtures of a strictly better and a strictly worse outcome, the greater [probability](../../../../../probability.md) of the better outcome is strictly preferred; this follows from the [independence axiom for lottery preferences](../../../../../independence-axiom-for-lottery-preferences.md) and [transitivity](../../../../../transitive-relation.md). Since $18/25>7/10$ and $\omega_1\succ\omega_4$, the comparison follows. [Complete lottery preferences](../../../../../complete-lottery-preferences.md) and [continuity of lottery preferences](../../../../../continuity-of-lottery-preferences.md) are part of the representation theorem's hypotheses; the direct substitution calculation uses the already supplied indifferences and does not need to invoke [continuity of lottery preferences](../../../../../continuity-of-lottery-preferences.md) again.[“The Expected Utility Property” and the preceding preference axioms](../../../../../expected-utility-theory-by-econport.md)

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Computational game theory](../../../computational-game-theory-split.md)
4. [2021](../../../split.md)
5. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../split.md)
6. [MSc in advanced computer science course of the University of Oxford](../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
7. [Master's course of the University of Oxford](../../../../../master-s-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
