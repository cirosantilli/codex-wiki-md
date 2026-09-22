<h1 id="b/4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [countable fixed point of a normal ordinal function](../../../../../countable-fixed-point-of-a-normal-ordinal-function.md), first show that $\Phi$ maps every [countable ordinal](../../../../../countable-ordinal.md) to a [countable ordinal](../../../../../countable-ordinal.md). Use [transfinite induction](../../../../../transfinite-induction.md) below $\omega_1$. The zero case is assumed, and the successor case is the stated preservation property. If $\lambda$ is a [countable](../../../../../countable-set.md) limit, normality gives $\Phi(\lambda)=\bigcup_{\alpha<\lambda}\Phi(\alpha)$, a [countable union of countable sets](../../../../../countable-union-of-countable-sets.md), hence [countable](../../../../../countable-set.md). This countable-union step is where [axiom of countable choice](../../../../../axiom-of-countable-choice.md) is used; the assumed [axiom of choice](../../../../../axiom-of-choice.md) supplies it.

Now set $\alpha_0=0$, $\alpha_{n+1}=\Phi(\alpha_n)$. The preceding result makes every term [countable](../../../../../countable-set.md), and the domination proved earlier makes the [sequence](../../../../../sequence.md) nondecreasing. If it ever stabilizes, it already gives the required fixed point. Otherwise $\alpha=\sup_{n<\omega}\alpha_n$ is a [countable](../../../../../countable-set.md) nonzero limit, using [axiom of countable choice](../../../../../axiom-of-countable-choice.md) again for countability of the union. Its defining [sequence](../../../../../sequence.md) is cofinal, so monotonicity and continuity give

$$
\boxed{\Phi(\alpha)=\sup_n\Phi(\alpha_n)=\sup_n\alpha_{n+1}=\alpha.}
$$

Apply this to $\Phi(\alpha)=\omega^\alpha$. This is normal, begins at $1$, and $\omega^{\alpha+1}=\omega^\alpha\cdot\omega$ is [countable](../../../../../countable-set.md) whenever $\omega^\alpha$ is [countable](../../../../../countable-set.md). Thus a [countable](../../../../../countable-set.md) $\epsilon$ satisfies $\boxed{\epsilon=\omega^\epsilon}$. Starting at zero gives the familiar tower [sequence](../../../../../sequence.md) $0,1,\omega,\omega^\omega,\ldots$, whose [supremum](../../../../../supremum.md) is $\epsilon_0$. The finite recursion, [ordinal](../../../../../ordinal-split.md) identities and fixed-point continuity do not require choice; the uses of choice above concern [countable](../../../../../countable-set.md) unions of [countable ordinals](../../../../../countable-ordinal.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
