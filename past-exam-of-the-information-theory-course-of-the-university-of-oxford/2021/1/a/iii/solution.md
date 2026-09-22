<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [chain rule for information entropy](../../../../../chain-rule-for-information-entropy.md) converts the two differences into [conditional entropies](../../../../../conditional-entropy.md). Their gap, in the order right minus left, is

$$
\begin{aligned}
&\bigl[H(X,Z)-H(X)\bigr]-\bigl[H(X,Y,Z)-H(X,Y)\bigr]\\
&\qquad=H(Z\mid X)-H(Z\mid X,Y)=I(Y;Z\mid X)\geq0.
\end{aligned}
$$

This is [additional conditioning reduces entropy](../../../../../additional-conditioning-reduces-entropy.md). The [relative entropy](../../../../../kullback-leibler-divergence.md) representation of [conditional mutual information](../../../../../conditional-mutual-information.md) identifies exactly when that gap vanishes: **equality holds if and only if $Y$ and $Z$ have [conditional independence](../../../../../conditional-independence.md) given $X$.** Knowledge of $Y$ then changes no [conditional probability](../../../../../conditional-probability.md) of $Z$ after $X$ is known.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
