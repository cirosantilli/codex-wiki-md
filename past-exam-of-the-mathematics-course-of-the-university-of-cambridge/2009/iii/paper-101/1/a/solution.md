<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [central limit theorem](../../../../../../central-limit-theorem.md), let $X_1,X_2,\ldots$ be [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with [expectation](../../../../../../expected-value.md) $\mu$ and finite positive [variance](../../../../../../variance-split.md) $\sigma^2$. Then

$$
\boxed{\frac{X_1+\cdots+X_n-n\mu}{\sigma\sqrt n}\xrightarrow{d}N(0,1).}
$$

Thus the centered, normalized sum has [convergence in distribution](../../../../../../convergence-in-distribution.md) to the standard [normal distribution](../../../../../../normal-distribution.md). The positive-[variance](../../../../../../variance-split.md) assumption is needed for this normalization; if $\sigma^2=0$, each summand equals $\mu$ [almost surely](../../../../../../almost-sure-convergence.md) and the centered sum is identically zero.

Here is a [characteristic function](../../../../../../characteristic-function.md) proof using only the finite second moment. Put $U=(X_1-\mu)/\sigma$, so $\mathbb EU=0$ and $\mathbb EU^2=1$. The elementary integral remainder identity gives $|e^{iz}-1-iz|\leq z^2/2$ for real $z$. Consequently

$$
\frac{e^{itU}-1-itU}{t^2}\longrightarrow-\frac{U^2}{2},\qquad
\left|\frac{e^{itU}-1-itU}{t^2}\right|\leq\frac{U^2}{2}.
$$

By the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), the [characteristic function](../../../../../../characteristic-function.md) satisfies $\varphi_U(t)=1-t^2/2+o(t^2)$ as $t\to0$. For a fixed real $t$, [independence](../../../../../../independent-random-variables.md) therefore gives

$$
\varphi_{(U_1+\cdots+U_n)/\sqrt n}(t)
=\varphi_U(t/\sqrt n)^n
=\left(1+\frac{c_n}{n}\right)^n,\qquad c_n\longrightarrow-t^2/2.
$$

The allowed complex-number limit makes this tend to $e^{-t^2/2}$, the [characteristic function](../../../../../../characteristic-function.md) of the standard [normal distribution](../../../../../../normal-distribution.md). It is continuous at zero, so the [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) proves the asserted [convergence in distribution](../../../../../../convergence-in-distribution.md). No third moment or boundedness of the summands was used.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 101](../../../paper-101-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
