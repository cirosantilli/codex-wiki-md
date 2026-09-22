<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Fix $T>0$. The given [normal distribution](../../../../../../normal-distribution.md) and part (d) imply

$$
\mathbb E e^{-\lambda\langle X\rangle_T}=e^{-\lambda T}\qquad(\lambda\ge0).
$$

One can deduce determinism without any moment assumption on the bracket. Put $Z=e^{-\langle X\rangle_T}$. Taking $\lambda=1,2$ gives $\mathbb EZ=e^{-T}$ and $\mathbb EZ^2=e^{-2T}$, so $\operatorname{Var}(Z)=0$. Therefore $\langle X\rangle_T=T$ almost surely. Applying this at every rational time and using continuity of [quadratic variation](../../../../../../quadratic-variation.md) gives $\langle X\rangle_t=t$ simultaneously for all $t\ge0$ outside a single null set.

The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) states that a continuous local martingale starting at zero with this bracket is [Brownian motion](../../../../../../brownian-motion-split.md) in its filtration. To see the independent-increment conclusion directly, the [Itô formula](../../../../../../ito-s-lemma.md) shows that $e^{i\theta X_t+\theta^2t/2}$ is a martingale on any fixed bounded time interval: it is a local martingale with a deterministic bound on its modulus. Thus

$$
\mathbb E[e^{i\theta(X_t-X_s)}\mid\mathcal F_s]=e^{-\theta^2(t-s)/2}.
$$

The deterministic [conditional characteristic function](../../../../../../conditional-characteristic-function.md) identifies an $N(0,t-s)$ increment independent of $\mathcal F_s$. Together with the given path continuity and $X_0=0$, this proves **$X$ is Brownian motion**.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [5](../../5.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
