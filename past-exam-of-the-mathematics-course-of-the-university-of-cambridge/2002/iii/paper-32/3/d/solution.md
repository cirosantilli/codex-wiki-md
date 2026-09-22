<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The two binary terminal payoffs are complementary:

$$
\mathbf1_{\{S_T\ge X\}}+\mathbf1_{\{S_T<X\}}=1
$$

in every state, including $S_T=X$. Long one of each is therefore exactly a unit [zero-coupon bond](../../../../../../zero-coupon-bond.md). The [law of one price](../../../../../../law-of-one-price.md) gives [digital put-call parity](../../../../../../digital-put-call-parity.md):

$$
\boxed{C_t^{\rm bin}+P_t^{\rm bin}=B(t,T).}
$$

With deterministic interest, the two separate values are $B(t,T)Q(S_T\ge X\mid\mathcal F_t)$ and $B(t,T)Q(S_T<X\mid\mathcal F_t)$. There is no need to assume a continuous terminal price distribution: the strict inequality for the put and weak inequality for the call allocate any atom at the strike exactly once.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
