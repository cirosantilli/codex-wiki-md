<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because the [Entropic Ruzsa distance](../../../../../../entropic-ruzsa-distance.md) depends only on marginal distributions, take $X,Y,Z$ independent with the required marginals. Since $X-Z=(X-Y)+(Y-Z)$ is a function of $(X-Y,Y-Z)$, the [data processing inequality for mutual information](../../../../../../data-processing-inequality.md) yields

$$
I\bigl(X;(X-Y,Y-Z)\bigr)\geq I(X;X-Z).
$$

The map $(X,X-Y,Y-Z)\mapsto(X,Y,Z)$ is a [bijection](../../../../../../bijection.md). Using independence and the [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md), the left side is

$$
H(X-Y,Y-Z)-H(Y)-H(Z),
$$

whereas the right side is $H(X-Z)-H(Z)$. Hence

$$
H(X-Z)+H(Y)\leq H(X-Y,Y-Z)
\leq H(X-Y)+H(Y-Z),
$$

where the final step is [subadditivity of information entropy](../../../../../../subadditivity-of-information-entropy.md). Substituting this inequality into the definition of $d_R$ gives the [Entropic Ruzsa triangle inequality](../../../../../../entropic-ruzsa-triangle-inequality.md)

$$
\boxed{d_R(X,Z)\leq d_R(X,Y)+d_R(Y,Z).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
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
