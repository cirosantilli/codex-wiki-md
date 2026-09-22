<h1 id="18h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [likelihood ratio](../../../../../../../likelihood-ratio.md) of the simple alternative to the simple null is

$$
\frac{f(x\mid1)}{f(x\mid0)}
=e^{-1}\left(\frac{1+e^x}{1+e^{x-1}}\right)^2.
$$

This is a strictly increasing function of $x$. By the [Neyman-Pearson lemma](../../../../../../../neyman-pearson-lemma.md), the most powerful test therefore rejects for $X>c$. The [logistic distribution](../../../../../../../logistic-distribution.md) has

$$
F_0(c)=\frac{e^c}{1+e^c}.
$$

The size condition $\mathbb P_0(X>c)=\alpha$ gives

$$
\frac{e^c}{1+e^c}=1-\alpha,
\qquad
c=\log\frac{1-\alpha}{\alpha}.
$$

Because the distribution is continuous, no boundary randomization is needed. The most powerful size-$\alpha$ test is therefore

$$
\boxed{\text{reject }H_0\quad\Longleftrightarrow\quad
X>\log\frac{1-\alpha}{\alpha}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [18H](../../../18h.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
