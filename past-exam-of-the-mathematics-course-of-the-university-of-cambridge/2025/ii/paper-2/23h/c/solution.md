<h1 id="23h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix $R>0$ and choose $\chi_R\in C_c^\infty((-R-1,R+1))$ with $\chi_R=1$ on $[-R,R]$. The sequence $(\chi_Rf_n)$ is bounded in $H_0^1((-R-1,R+1))$. By part (a), each subsequence has a further subsequence converging strongly in $L^2$ on this bounded interval. The original weak convergence in $L^2(\mathbb R)$ forces every such strong limit to be zero. It follows that the whole sequence satisfies

$$
\|f_n\|_{L^2([-R,R])}\longrightarrow0;
$$

otherwise a subsequence bounded away from zero would contradict the preceding compactness argument.

The pointwise hypothesis gives a uniform tail estimate:

$$
\int_{|x|>R}|f_n(x)|^2\,dx
\leq C^2\int_{|x|>R}(1+x^2)^{-2}\,dx,
$$

whose right-hand side tends to zero as $R\to\infty$, independently of $n$. Given $\varepsilon>0$, first choose $R$ so that this tail is below $\varepsilon/2$, and then choose $n$ so that the integral on $[-R,R]$ is below $\varepsilon/2$. Therefore

$$
\boxed{\|f_n\|_{L^2(\mathbb R)}\longrightarrow0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [23H](../../23h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
