<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $\sigma^2>0$; otherwise the scaled sum is deterministic and no nontrivial [rate function](../../../../../../rate-function.md) is possible. The sum has [normal distribution](../../../../../../normal-distribution.md) $B_N\sim N(N\mu,N\sigma^2)$. For $X_N=B_N/N^{1+\varepsilon}$, use the faster [large-deviation speed](../../../../../../large-deviation-speed.md) $b_N=N^{1+2\varepsilon}$. The [moment-generating function of a normal distribution](../../../../../../moment-generating-function-of-a-normal-distribution.md) yields

$$
\frac1{b_N}\log\mathbb E e^{b_N\theta X_N}
=\mu\theta N^{-\varepsilon}+\frac{\sigma^2\theta^2}{2}
\longrightarrow \Lambda(\theta)=\frac{\sigma^2\theta^2}{2}.
$$

The limiting [cumulant-generating function](../../../../../../cumulant-generating-function.md) is finite and differentiable on all of $\mathbb R$, hence satisfies the [Gärtner–Ellis theorem](../../../../../../gartner-ellis-theorem.md). Its [Legendre-Fenchel transform](../../../../../../convex-conjugate.md) is obtained by maximizing $\theta x-\sigma^2\theta^2/2$, whose maximizer is $\theta=x/\sigma^2$. Thus

$$
\boxed{\text{speed }N^{1+2\varepsilon},\qquad I_B(x)=\frac{x^2}{2\sigma^2}\quad(x\in\mathbb R).}
$$

The drift disappears because the scaled [mean](../../../../../../expected-value.md) is $\mu/N^\varepsilon\to0$. The [rate function](../../../../../../rate-function.md) is nontrivial and good. The corrected scaled [cumulant-generating function](../../../../../../cumulant-generating-function.md) used here contains an [expectation](../../../../../../expected-value.md); the corresponding formula in the paper's reference material omits it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
