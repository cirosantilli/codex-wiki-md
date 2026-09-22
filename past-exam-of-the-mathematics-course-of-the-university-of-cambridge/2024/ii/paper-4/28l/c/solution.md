<h1 id="28l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $d_i=\bar X_{n-1,i}-\bar X_n=(\bar X_n-X_i)/(n-1)$. Taylor's theorem gives

$$
T_{n-1,i}-T_n=g'(\bar X_n)d_i+R_{n,i},
\qquad |R_{n,i}|\leq M d_i^2.
$$

Since $\sum_i d_i=0$, centering the leave-one-out values and expanding the square gives

$$
v_{\rm JACK}=\frac{n-1}{n}(A_n+B_n+2C_n),
$$

with the stated $A_n,B_n$ and the cross term satisfying $|C_n|\leq\sqrt{A_nB_n}$ by Cauchy--Schwarz.

Now

$$
A_n=\frac{g'(\bar X_n)^2}{(n-1)^2}
\sum_i(X_i-\bar X_n)^2
\sim\frac{g'(\mu)^2\sigma^2}{n}.
$$

The fourth-moment assumption gives

$$
B_n\leq\frac{M^2}{(n-1)^4}\sum_i(X_i-\bar X_n)^4=O(n^{-3}),
$$

and hence $C_n=O(n^{-2})$. Since $\sigma_n^2=g'(\mu)^2\sigma^2/n$, it follows that

$$
\boxed{\frac{v_{\rm JACK}}{\sigma_n^2}\to1.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28L](../../28l.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
