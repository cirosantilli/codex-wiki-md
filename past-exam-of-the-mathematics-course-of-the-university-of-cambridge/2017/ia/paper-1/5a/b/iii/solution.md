<h1 id="5a/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $d_n=x_{n+1}-x_n$ be the direction vector of the segment $X_nX_{n+1}$. Consecutive vectors $x_n,x_{n+1}$ are perpendicular and $|x_{n+1}|=\lambda|x_n|$. Using $x_{n+2}=-\lambda^2x_n$,

$$
d_n\mathbin{\cdot}d_{n+1}
=(x_{n+1}-x_n)\mathbin{\cdot}(x_{n+2}-x_{n+1})
=-|x_{n+1}|^2+\lambda^2|x_n|^2=0.
$$

Thus adjacent segments are perpendicular. Also

$$
d_{n+2}=x_{n+3}-x_{n+2}=-\lambda^2(x_{n+1}-x_n)=-\lambda^2d_n,
$$

so

$$
\boxed{X_nX_{n+1}\parallel X_{n+2}X_{n+3}}.
$$

If $0<\lambda<1$, the norm formula in part (i) gives $x_n\to0$. If $\lambda=1$, then $x_{n+2}=-x_n$: the points $X_1,X_2,-X_1,-X_2$ repeat cyclically and form a square centered at the origin.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [5A](../../../5a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ia](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
