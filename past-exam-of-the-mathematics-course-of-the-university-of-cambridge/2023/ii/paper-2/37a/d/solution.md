<h1 id="37a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Substituting the [fixed-tension partition function of a one-dimensional chain](../../../../../../fixed-tension-partition-function-of-a-one-dimensional-chain.md) into the given free-energy definition gives

$$
\boxed{G=-k_BT\log Z=-nk_BT\log(2\cosh(\tau a)).}
$$

Differentiation with respect to the parameter conjugate to extension gives

$$
\frac{\partial G}{\partial\tau}
=-nk_BT\,a\tanh(\tau a).
$$

The same result follows directly from the [expected value](../../../../../../expected-value.md) under $p_i=e^{\tau l_i}/Z$:

$$
L=\sum_i p_i l_i
=\frac1Z\frac{\partial Z}{\partial\tau}
=\frac{\partial\log Z}{\partial\tau}.
$$

Consequently

$$
\boxed{L=-\frac1{k_BT}\frac{\partial G}{\partial\tau}},
\qquad
\boxed{\tanh(\tau a)=\frac{L}{na}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [37A](../../37a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
