<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use normalized [Fourier-Walsh transform](../../../../../../fourier-walsh-transform.md) coefficients $\widehat g(\xi)=2^{-n}\sum_x g(x)(-1)^{x\cdot\xi}$. The Hamming weight $|\xi|$ counts the nonzero coordinates. Norms on the input cube use uniform probability, and a frequency integral here is counting over $\xi\in\mathbb F_2^n$. A common alternative normalization multiplies both sides of the requested comparison by the same factor and does not change it.

[Beckner's inequality](../../../../../../beckner-s-inequality.md) states that for $1<p\leq q<\infty$ and $0\leq\rho\leq\sqrt{(p-1)/(q-1)}$, the [noise operator on the Boolean hypercube](../../../../../../noise-operator-on-the-boolean-hypercube.md), with coefficients $\widehat{T_\rho g}(\xi)=\rho^{|\xi|}\widehat g(\xi)$, satisfies $\|T_\rho g\|_q\leq\|g\|_p$. In particular choose $q=2$, $p=4/3$, $\rho=1/\sqrt3$.

Let $g=1_A$ and $\alpha=|A|/2^n$. Then $\|g\|_{4/3}^2=\alpha^{3/2}$. On frequencies of weight at most two, $\rho^{2|\xi|}\geq1/9$, so [Beckner's inequality](../../../../../../beckner-s-inequality.md) and [Parseval's identity](../../../../../../parseval-identity.md) give the [low-degree Fourier mass of a sparse Boolean set](../../../../../../low-degree-fourier-mass-of-a-sparse-boolean-set.md) estimate

$$
S_{\leq2}:=\sum_{|\xi|\leq2}\widehat g(\xi)^2\leq9\sum_\xi\rho^{2|\xi|}\widehat g(\xi)^2=9\|T_\rho g\|_2^2\leq9\alpha^{3/2}.
$$

The [indicator function](../../../../../../indicator-function.md) is real and the cube characters are real, so the displayed squares equal the squared [absolute values](../../../../../../absolute-value.md). Total [Fourier weight](../../../../../../fourier-weight.md) is $\sum\widehat g(\xi)^2=\|g\|_2^2=\alpha$. If $2^n>2003$, then $0<\alpha\leq1/2003$ and $9\sqrt\alpha\leq9/\sqrt{2003}<1/2$, since $2003>18^2$. Therefore

$$
\boxed{S_{\leq2}<\frac\alpha2<\alpha-S_{\leq2}=\sum_{|\xi|>2}\widehat g(\xi)^2.}
$$

This establishes the strict comparison for every power $N=2^n>2003$, not merely for an unspecified very large threshold. The original PDF supplies the density condition and Beckner request, both missing from the converted TeX.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
