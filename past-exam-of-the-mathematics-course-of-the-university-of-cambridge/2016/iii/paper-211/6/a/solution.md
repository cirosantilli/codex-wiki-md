<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $\xi_t=V(t,S_t)$. The backward equation cancels its [drift](../../../../../../drift-coefficient.md), leaving

$$
d\xi_t=\left(V_t+\frac12a(S_t)^2V_{SS}\right)(t,S_t)dt
+a(S_t)V_S(t,S_t)dW_t
=a(S_t)V_S(t,S_t)dW_t.
$$

Bounded $a$ and $V_S$ make this [Itô integral](../../../../../../ito-integral.md) square-integrable on the finite horizon; in addition $V$ itself is bounded. Hence $\xi$ is a true [martingale](../../../../../../martingale-split.md), not just a [local martingale](../../../../../../local-martingale.md), and $\xi_T=g(S_T)$. **Taking conditional expectations gives**

$$
\boxed{\xi_t=\mathbb E[g(S_T)\mid\mathcal F_t].}
$$

The [stock](../../../../../../stock.md) is understood to be [adapted](../../../../../../adapted-process.md) to the stated [Brownian filtration](../../../../../../brownian-filtration.md), with its initial value fixed there. This is the [Feynman-Kac formula](../../../../../../feynman-kac-formula.md) in the zero-potential, zero-drift case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
