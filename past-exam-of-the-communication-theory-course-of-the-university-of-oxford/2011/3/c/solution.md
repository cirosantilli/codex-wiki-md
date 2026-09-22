<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For any chosen input distribution, the chain rule and nonnegativity of [conditional mutual information](../../../../conditional-mutual-information.md) give

$$
I(U;V,W)=I(U;V)+I(U;W\mid V)\geq I(U;V),
$$

and likewise $I(U;V,W)\geq I(U;W)$. Choosing an input distribution attaining either marginal [capacity](../../../../channel-capacity.md) proves $K\geq\max\{K_1,K_2\}$.

For the upper bound, [conditional independence](../../../../conditional-independence.md) implies $H(V,W\mid U)=H(V\mid U)+H(W\mid U)$, while [entropy](../../../../information-entropy-split.md) subadditivity gives $H(V,W)\leq H(V)+H(W)$. Therefore

$$
\begin{aligned}
I(U;V,W)&=H(V,W)-H(V,W\mid U)\\
&\leq H(V)+H(W)-H(V\mid U)-H(W\mid U)\\
&=I(U;V)+I(U;W)\leq K_1+K_2.
\end{aligned}
$$

Maximizing over the input law gives

$$
\boxed{\max\{K_1,K_2\}\leq K\leq K_1+K_2.}
$$

More precisely, under the conditional-independence assumption,

$$
I(U;V,W)=I(U;V)+I(U;W)-I(V;W).
$$

The outputs may be dependent through the common input, and this final term measures the information they share rather than add independently.

This is [information from two conditionally independent observations](../../../../information-from-two-conditionally-independent-observations.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
