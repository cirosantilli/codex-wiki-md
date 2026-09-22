<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Extend $u$ by zero to $\mathbb R^n$; its [compact support](../../../../../../compact-support.md) inside the ball makes the extension [smooth](../../../../../../smooth-function.md). The [Fourier transform of a derivative](../../../../../../fourier-transform-of-a-derivative.md) gives

$$
\widehat{L_0u}(\xi)=-(A\xi\mathbin\cdot\xi)\widehat u(\xi).
$$

The assumption says that $L_0$ is a [uniformly elliptic operator](../../../../../../uniformly-elliptic-operator.md), so

$$
|A\xi\mathbin\cdot\xi|^2\geq\theta^2|\xi|^4.
$$

Moreover,

$$
\sum_{i,j=1}^n|\xi_i\xi_j|^2
=\left(\sum_{i=1}^n\xi_i^2\right)^2
=|\xi|^4.
$$

The [Plancherel theorem](../../../../../../plancherel-theorem.md) therefore yields

$$
\|L_0u\|_2^2
=\int_{\mathbb R^n}|A\xi\mathbin\cdot\xi|^2|\widehat u|^2\,d\xi
\geq\theta^2\int_{\mathbb R^n}|\xi|^4|\widehat u|^2\,d\xi
=\theta^2\|D^2u\|_2^2.
$$

All integrands vanish outside the original support where appropriate, so

$$
\boxed{\theta\|D^2u\|_{L^2(B_r(x_0))}\leq\|L_0u\|_{L^2(B_r(x_0))}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
