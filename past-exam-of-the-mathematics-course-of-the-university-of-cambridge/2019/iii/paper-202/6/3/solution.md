<h1 id="6/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [variation-of-constants formula](../../../../../../variation-of-constants-formula.md) gives, when $a\ne0$,

$$
X_t=e^{-at}x+\frac ba(1-e^{-at})
+\sigma\int_0^te^{-a(t-u)}dB_u.
$$

Therefore, with $m=\min(s,t)$,

$$
\begin{aligned}
\operatorname{cov}(X_t,X_s)
&=\sigma^2\int_0^me^{-a(t-u)}e^{-a(s-u)}du\\
&=\boxed{\frac{\sigma^2}{2a}
\left(e^{-a|t-s|}-e^{-a(t+s)}\right)}.
\end{aligned}
$$

If $a=0$, then $X_t=x+bt+\sigma B_t$ and

$$
\boxed{\operatorname{cov}(X_t,X_s)=\sigma^2\min(t,s).}
$$

## ↑ Ancestors (11)

1. [3](../3.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
