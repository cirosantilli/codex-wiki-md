<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The first of the [Gaussian drift primitives](../../../../../../gaussian-drift-primitives.md), $E_0$, is an [even function](../../../../../../even-function.md); the second, $E_1$, is an [odd function](../../../../../../odd-function.md). Their derivatives follow by the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md). In particular $E_0'$ is the [Dawson function](../../../../../../dawson-function.md), which behaves as $1/(2z)+O(z^{-3})$. Since the [error function](../../../../../../error-function.md) tends to $\pm1$, the derivative of $E_1$ behaves as $1/(2|z|)+O(|z|^{-3})$ at either end. Integration therefore gives

$$
E_0(z)=\frac12\log|z|+C_1+o(1),
\qquad E_1(z)=\operatorname{sgn}z\left[\frac12\log|z|+C_2+o(1)\right].
$$

Also $F\sim z+\sqrt\pi/4$ on the left and $F\sim\sqrt\pi/4$ on the right. The two inner overlaps are consequently

$$
Y_0+\varepsilon Y_1\sim
\begin{cases}
A+\varepsilon\left[z+A\log|z|+\sqrt\pi/4+2cC_1-2dC_2+\alpha-\beta\right],&z\to-\infty,\\
B+\varepsilon\left[B\log z+\sqrt\pi/4+2cC_1+2dC_2+\alpha+\beta\right],&z\to+\infty.
\end{cases}
$$

Expressing the [outer expansions](../../../../../../outer-expansion.md) in $r=\varepsilon z$ requires the left constant $1+A\log\varepsilon$ and the right constant $B\log\varepsilon$. Equating those constants gives the stated $\alpha,\beta$. This is exactly how a [logarithmic overlap creates a switchback term](../../../../../../logarithmic-overlap-creates-a-switchback-term.md): $\log|r|=\log\varepsilon+\log|z|$. Adding the outer solutions and removing these overlaps leaves the displayed [additive composite expansion](../../../../../../additive-composite-expansion.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
