<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiate the [Helmholtz free energy](../../../../helmholtz-free-energy.md) at fixed couplings. With $\lambda=\lambda_+$ from [solution](../b/solution.md), the [entropy](../../../../entropy-split.md) per [spin](../../../../spin.md) is

$$
s=-\frac{\partial f}{\partial T}=\frac{k_B}{2}\left(\log\lambda-\beta\frac{\partial\log\lambda}{\partial\beta}\right).
$$

It is particularly useful to write

$$
\lambda=e^{\beta(2\bar J-J)}+e^{-\beta(2\bar J+J)}+2e^{\beta J}.
$$

At $\bar J=J$, this is $3e^{\beta J}+e^{-3\beta J}$, so $f=-J/2-(\log3)/(2\beta)+o(\beta^{-1})$. For fixed $\bar J>J$, the first exponential dominates alone, giving $f=(J-2\bar J)/2+o(\beta^{-1})$. Hence the [residual entropy](../../../../residual-entropy.md) is

$$
\boxed{\lim_{T\to0}s=\begin{cases}(k_B/2)\log3,&\bar J=J,\\0,&\bar J>J.\end{cases}}
$$

The finite positive difference $\bar J-J$ must be kept fixed in the second limit; taking it to zero first gives the other answer.

At high [temperature](../../../../temperature-split.md), $\lambda\to4$ and $\beta\partial_\beta\log\lambda\to0$, whence

$$
\boxed{\lim_{T\to\infty}s=k_B\log2.}
$$

All $2^{2L}$ configurations become equally probable because their [Boltzmann factors](../../../../boltzmann-factor.md) tend to one. The two available states per [spin](../../../../spin.md), rather than the coupling values, determine this [entropy](../../../../entropy-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
