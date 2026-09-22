<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix the channel matrix $W$. The mixed input induces the mixed output $q_3=\lambda q_1+(1-\lambda)q_2$. The [concavity of information entropy](../../../../concavity-of-information-entropy.md) implies

$$
H(q_3)\geq\lambda H(q_1)+(1-\lambda)H(q_2).
$$

For completeness, the difference is $\lambda D(q_1\Vert q_3)+(1-\lambda)D(q_2\Vert q_3)\geq0$ by [Gibbs inequality](../../../../gibbs-inequality.md), including zero coordinates with the usual conventions.

On the other hand, conditional output [entropy](../../../../information-entropy-split.md) is linear in the input law:

$$
H(Y_3\mid X_3)=\sum_xp_3(x)H(W(\cdot\mid x))
=\lambda H(Y_1\mid X_1)+(1-\lambda)H(Y_2\mid X_2).
$$

Subtracting gives the [concavity of mutual information in the input distribution](../../../../concavity-of-mutual-information-in-the-input-distribution.md):

$$
\boxed{I(X_3;Y_3)\geq\lambda I(X_1;Y_1)+(1-\lambda)I(X_2;Y_2).}
$$

This makes maximizing [mutual information](../../../../mutual-information.md) over the input [probability simplex](../../../../probability-simplex.md) a concave optimization problem: a local maximum is global. It also justifies averaging input distributions over channel symmetries when searching for an optimum, since symmetry averaging cannot lower the achieved [mutual information](../../../../mutual-information.md). The channel itself is held fixed throughout.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
