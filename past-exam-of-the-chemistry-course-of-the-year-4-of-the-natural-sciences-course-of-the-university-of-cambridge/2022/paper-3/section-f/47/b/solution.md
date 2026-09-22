<h1 id="section-f/47/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The printed PDF has a **plus sign before the second logarithm**. Differentiating that expression literally, with $h_i=\sigma(a_i)$ and $\partial h_i/\partial w_j=h_i(1-h_i)z_{ij}$, gives

$$
\frac{\partial E_i}{\partial h_i}=-\frac{y_i}{h_i}-\frac{1-y_i}{1-h_i},\qquad
\boxed{\frac{\partial E_i}{\partial w_j}=-[y_i(1-h_i)+(1-y_i)h_i]z_{ij}}.
$$

For example, at $y_i=0$ it is $-h_i z_{ij}$, so minimizing this printed objective pushes the predicted [probability](../../../../../../probability.md) of class one upwards rather than downwards; the objective is unbounded below as $h_i\to1$. It is therefore not the usual [binary cross-entropy](../../../../../../binary-cross-entropy.md).

If the second sign was intended to be negative, the standard negative log-likelihood is $-y_i\log h_i-(1-y_i)\log(1-h_i)$ and the derivative simplifies instead to **$(h_i-y_i)z_{ij}$**. Stating both cases preserves the actual question's algebra while identifying the apparent sign error. The logarithms here are natural; another base multiplies the [gradients](../../../../../../gradient.md) by its constant conversion factor.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [47](../../47.md)
3. [Section F](../../../section-f.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
