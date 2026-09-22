<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For finite-valued variables, [mutual information](../../../../mutual-information.md) is

$$
\boxed{I(X;Y)=\sum_{x,y}p(x,y)\log_2\frac{p(x,y)}{p_X(x)p_Y(y)}=H(Y)-H(Y\mid X)}.
$$

Terms of zero joint [probability](../../../../probability.md) are zero. A [discrete memoryless channel](../../../../discrete-memoryless-channel.md) has fixed transition probabilities $W(y\mid x)$ on finite alphabets, and conditional on an input sequence its outputs are independent with the product law $\prod_iW(y_i\mid x_i)$. Its [channel capacity](../../../../channel-capacity.md) is

$$
\boxed{C=\max_{P_X}I(X;Y)}
$$

bits per channel use. The maximum is over all input distributions, with the transition law held fixed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
