<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The statement necessarily treats $P_0,P_1$ as [probability measures](../../../../../probability-measure.md), as required by the sampling model $X\sim P_J$. The word "measures" in the introduction must be read with this normalization. Use the paper's convention $H^2(P,Q)=\tfrac12\int(\sqrt p-\sqrt q)^2\,d\mu$ for the [Squared Hellinger distance](../../../../../squared-hellinger-distance.md) throughout this question.

A measurable binary [hypothesis test](../../../../../statistical-hypothesis-test-split.md) $\psi$ is determined by the [measurable set](../../../../../measurable-set.md) $A=\{x:\psi(x)=1\}$. Under the uniform prior on the two hypotheses, its error probability is

$$
\mathbb P\{\psi(X)\neq J\}
=\frac12\bigl(P_0(A)+P_1(A^c)\bigr)
=\frac12\bigl(1-[P_1(A)-P_0(A)]\bigr).
$$

Since the two measures have equal total mass,

$$
\begin{aligned}
\sup_A[P_1(A)-P_0(A)]
&=\int(p_1-p_0)_+\,d\mu\\
&=\frac12\int|p_1-p_0|\,d\mu
=V(P_0,P_1).
\end{aligned}
$$

Indeed, the integral over any set is at most the integral of the positive part, and equality holds for $A=\{p_1>p_0\}$. This is also the [total variation distance](../../../../../total-variation-distance.md). The [likelihood ratio](../../../../../likelihood-ratio.md) rule choosing hypothesis $1$ precisely on that set therefore attains the [infimum](../../../../../infimum.md), proving

$$
\boxed{\inf_\psi\mathbb P\{\psi(X)\neq J\}=\frac12\bigl[1-V(P_0,P_1)\bigr].}
$$

Arbitrary choices on the tie set $\{p_1=p_0\}$ leave the error unchanged. This is the exact link between [total variation distance](../../../../../total-variation-distance.md) and optimal binary [statistical hypothesis testing](../../../../../statistical-hypothesis-test-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../../split.md)
6. [Algorithmic foundations of learning course of the University of Oxford](../../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
