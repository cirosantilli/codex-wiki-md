<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For one stage, first-order [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) gives $b_1=1$. The condition $b^TA^{-1}\mathbf1=1$ then gives $a_{11}=1$. Hence the scheme is **the [Backward Euler method](../../../../../../backward-euler-method.md)**:

$$
y_{n+1}=y_n+h f(t_n+h,y_{n+1}).
$$

It is a one-node [collocation Runge-Kutta method](../../../../../../collocation-runge-kutta-method.md) with $c_1=1$. Specifically, choose a linear [polynomial](../../../../../../polynomial-split.md) $p(t)$ on $[t_n,t_n+h]$ with $p(t_n)=y_n$ and impose $p'(t_n+h)=f(t_n+h,p(t_n+h))$. Its derivative is constant, so $p(t_n+h)-p(t_n)=hp'(t_n+h)$, exactly the [Backward Euler method](../../../../../../backward-euler-method.md) update.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
