<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite joint distribution, the [mutual information](../../../../mutual-information.md) is

$$
\boxed{I(X;Y)=\sum_{x,y}p(x,y)\log_2\frac{p(x,y)}{p_X(x)p_Y(y)}
=H(Y)-H(Y\mid X)=H(X)-H(X\mid Y).}
$$

Zero-[probability](../../../../probability.md) terms contribute zero. It measures the reduction in uncertainty about one variable upon observing the other.

A [discrete memoryless channel](../../../../discrete-memoryless-channel.md) has discrete input/output alphabets and a fixed [transition matrix](../../../../stochastic-matrix.md) $W(y\mid x)$. Over successive uses it obeys

$$
P(Y_1=y_1,\ldots,Y_n=y_n\mid X_1=x_1,\ldots,X_n=x_n)
=\prod_{j=1}^nW(y_j\mid x_j).
$$

Thus the output at a use depends on that input and no other channel history. Its [channel capacity](../../../../channel-capacity.md) is

$$
\boxed{C=\max_{p_X}I(X;Y),}
$$

in bits per use for base-two logarithms. On finite alphabets the maximum exists by [continuity](../../../../continuous-function.md) on the [probability simplex](../../../../probability-simplex.md); for more general discrete alphabets one uses a supremum.

## ↑ Ancestors (12)

1. [A](../a.md)
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
