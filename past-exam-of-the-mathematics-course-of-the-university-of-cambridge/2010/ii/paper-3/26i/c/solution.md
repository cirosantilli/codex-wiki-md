<h1 id="26i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $K$ count second-fork arrivals. Its independent increment over $(s,s+t]$ is Poisson$(rt)$, and

$$
\mathbb P(K(s)\text{ even})=\frac{1+e^{-2rs}}2,\qquad
\mathbb P(K(s)\text{ odd})=\frac{1-e^{-2rs}}2,
$$

obtained by evaluating $\mathbb E(-1)^{K(s)}=e^{-2rs}$. If $K(s)$ is even, the next second-fork arrival goes to B, so no B arrival requires zero new arrivals. If it is odd, the next goes to C, so up to one new arrival is allowed. Reverse these alternatives for C. Therefore

$$
\boxed{\begin{aligned}
\mathbb P(X_A(s+t)=X_A(s))&=e^{-\lambda t/3},\\
\mathbb P(X_B(s+t)=X_B(s))&=e^{-rt}\left[1+\frac{rt}2(1-e^{-2rs})\right],\\
\mathbb P(X_C(s+t)=X_C(s))&=e^{-rt}\left[1+\frac{rt}2(1+e^{-2rs})\right].
\end{aligned}}
$$

At $s=0$ these reduce to the distinct initial-delay survivors; as $s\to\infty$, both non-Poisson probabilities approach the equilibrium-delay survivor from part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26I](../../26i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
