<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The axioms for [information entropy](../../../../../../information-entropy.md) give the formula $H(X)=-\sum_xp(x)\log p(x)$ and hence the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md)

$$
H(X,Y)=H(X)+H(Y\mid X).
$$

Because [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md), $H(Y\mid X)\leq H(Y)$, and therefore

$$
H(X,Y)\leq H(X)+H(Y).
$$

This is [subadditivity of information entropy](../../../../../../subadditivity-of-information-entropy.md).

For the [entropy submodularity](../../../../../../entropy-submodularity.md) rule, apply the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) twice:

$$
\begin{aligned}
H(X,Y)+H(Y,Z)-H(Y)-H(X,Y,Z)
&=H(X\mid Y)-H(X\mid Y,Z)\\
&=I(X;Z\mid Y)\geq0.
\end{aligned}
$$

The last quantity is [conditional mutual information](../../../../../../conditional-mutual-information.md), whose nonnegativity again expresses that [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 164](../../../paper-164-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
