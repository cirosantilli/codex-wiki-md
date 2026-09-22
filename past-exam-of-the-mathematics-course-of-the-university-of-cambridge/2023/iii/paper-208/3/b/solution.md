<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $Z_i=f_i(X^{(i)})$ and $\Delta_i=Z-Z_i$. The [weakly self-bounding function](../../../../../../weakly-self-bounding-function.md) assumptions give $\Delta_i\geq0$ and $\sum_i\Delta_i^2\leq Z$. For $0\leq\lambda<2$, the bound $\phi(-x)\leq x^2/2$ and the [modified logarithmic Sobolev inequality](../../../../../../modified-logarithmic-sobolev-inequality.md) imply

$$
\operatorname{Ent}(e^{\lambda Z})
\leq\frac{\lambda^2}{2}\mathbb E[Ze^{\lambda Z}].
$$

Let $H(\lambda)=\log\mathbb Ee^{\lambda Z}$. Dividing by $\mathbb Ee^{\lambda Z}$ turns this into

$$
\lambda H'(\lambda)-H(\lambda)
\leq\frac{\lambda^2}{2}H'(\lambda),
$$

and therefore

$$
\frac{H'(\lambda)}{H(\lambda)}
\leq\frac1{\lambda(1-\lambda/2)}.
$$

Since $H(\lambda)\sim\lambda\mathbb EZ$ as $\lambda\downarrow0$, integration gives

$$
H(\lambda)
\leq\frac{2\lambda\mathbb EZ}{2-\lambda}.
$$

Subtracting $\lambda\mathbb EZ$ from both sides yields

$$
\log\mathbb E e^{\lambda(Z-\mathbb EZ)}
\leq\frac{\lambda^2\mathbb EZ}{2-\lambda},
$$

as required. This is a [Herbst argument](../../../../../../herbst-argument.md) with a variance proxy controlled by $Z$ itself.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
