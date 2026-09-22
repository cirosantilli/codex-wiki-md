<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the finite state space, $P_t=e^{tQ}$ and

$$
\mathbb E_xf(X_t)=(P_tf)(x).
$$

Therefore

$$
\lim_{t\downarrow0}\frac{\mathbb E_xf(X_t)-f(x)}t
=\left(\lim_{t\downarrow0}\frac{P_t-I}{t}f\right)(x)
=Qf(x).
$$

The [matrix](../../../../../../matrix.md) semigroup satisfies $\frac d{dt}P_tf=P_tQf$. Integrating from $0$ to $t$ gives the backward [integral](../../../../../../integral.md) equation

$$
\boxed{
\mathbb E_xf(X_t)=f(x)+\int_0^t\mathbb E_x[Qf(X_s)]\,ds.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
