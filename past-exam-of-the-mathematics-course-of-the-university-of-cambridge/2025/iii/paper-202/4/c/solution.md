<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $X$ and $Y$ be two solutions with the same initial value and Brownian motion, and put $Z=X-Y$. [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
dZ_t^2=\left(2Z_t(b(X_t)-b(Y_t))+
(\sigma(X_t)-\sigma(Y_t))^2\right)dt
+2Z_t(\sigma(X_t)-\sigma(Y_t))dW_t.
$$

Stop when either process or the stochastic integral becomes large. Taking expectations, using the assumed one-sided Lipschitz bound, and then removing the localization gives

$$
\mathbb EZ_t^2\leq K\int_0^t\mathbb EZ_s^2ds.
$$

The [Gronwall inequality](../../../../../../gronwall-inequality.md) yields $\mathbb EZ_t^2=0$. Thus $X_t=Y_t$ almost surely at every rational time, and path continuity makes the two processes indistinguishable. This proves pathwise uniqueness.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
