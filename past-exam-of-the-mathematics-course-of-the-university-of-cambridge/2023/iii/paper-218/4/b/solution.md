<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fitted classifier is

$$
\widehat C(x)=\operatorname*{argmax}_{k\in\{0,1\}}\widehat p_k(x),
$$

and training minimizes the empirical [categorical cross-entropy loss](../../../../../../categorical-cross-entropy-loss.md)

$$
-\sum_i\sum_{k=0}^1y_{ik}\log p_{ik}.
$$

The [softmax non-identifiability](../../../../../../softmax-non-identifiability.md) already proves that the coefficient vector is not unique. For any $a\in\mathbb R^2$ and $r\in\mathbb R$, replace both rows of $V$ by $V_{k\cdot}+a^T$ and both output biases by $c_k+r$. Every logit then gains the same value $a^Th+r$, so all softmax probabilities, classifications, and losses remain unchanged. Permuting the two hidden units supplies another non-uniqueness.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
