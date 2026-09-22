<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Expansion of the two squares gives

$$
\boxed{|\xi^+|^2+|\xi^-|^2=\frac12(|\xi|^2+|\xi|^2|\sigma|^2)=|\xi|^2}.
$$

Let $D=d(f,g)$ be the [Fourier distance of order two](../../../../../../fourier-distance-of-order-two.md), with the supremum taken over $\xi\ne0$. Both [Fourier transforms](../../../../../../fourier-transform.md) have modulus at most one. Add and subtract $\widehat g(\xi^+)\widehat f(\xi^-)$, then use the [triangle inequality](../../../../../../triangle-inequality.md):

$$
|\widehat f(\xi^+)\widehat f(\xi^-)-\widehat g(\xi^+)\widehat g(\xi^-)|
\leq|\widehat f(\xi^+)-\widehat g(\xi^+)|+|\widehat f(\xi^-)-\widehat g(\xi^-)|
\leq D(|\xi^+|^2+|\xi^-|^2).
$$

Dividing by $|\xi|^2$ proves the bound by $D$, and splitting the last expression into its two weighted terms gives the requested intermediate inequality. If one of $\xi^\pm$ vanishes, its unweighted difference is zero by equal mass; its weighted term is interpreted as zero, avoiding a $0/0$ quotient.

Equal mass and first moment also explain finiteness of this distance: subtract the constant and linear Taylor terms in the Fourier [integral](../../../../../../integral.md) and use $|e^{-ia}-1+ia|\leq a^2/2$. This bounds the difference by $|\xi|^2\int|v|^2(f+g)/2$. No direction-independent extension of the quotient at zero is required.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
