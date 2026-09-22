<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $X_1,X_2,Y$ be independent, with $X_1,X_2$ distributed as $X$. Apply part (b) to $X_1,-Y,X_2$:

$$
H(X_1+X_2-Y)+H(Y)\leq2H(X-Y).
$$

Adding an [independent random variable](../../../../../../independent-random-variables.md) cannot decrease [information entropy](../../../../../../information-entropy.md), so

$$
H(X_1+X_2)+H(Y)\leq2H(X-Y).
$$

In terms of [Entropic Ruzsa distance](../../../../../../entropic-ruzsa-distance.md), this is $d_R(X,-X)\leq2d_R(X,Y)$. The [Entropic Ruzsa triangle inequality](../../../../../../entropic-ruzsa-triangle-inequality.md) and invariance under simultaneous negation now give

$$
d_R(X,-Y)
\leq d_R(X,-X)+d_R(-X,-Y)
\leq2d_R(X,Y)+d_R(X,Y),
$$

which is the [Entropic Ruzsa sum-difference inequality](../../../../../../entropic-ruzsa-sum-difference-inequality.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
