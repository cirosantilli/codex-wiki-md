<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a nonzero [Hecke eigenform](../../../../../../hecke-eigenform.md) that is a [cusp form](../../../../../../cusp-form.md), $c(1)\ne0$: otherwise part (b) would make all its positive [Fourier coefficients](../../../../../../fourier-coefficient.md) zero, and cuspidality already gives $c(0)=0$, forcing $f=0$. Since $T_w(1)=I$, $\lambda(1)=1$. Part (b) gives multiplicativity at coprime integers and the prime-power recurrence

$$
\lambda(p^{r+1})=\lambda(p)\lambda(p^r)-p^{w-1}\lambda(p^{r-1})\quad(r\geq1).
$$

Multiply its generating [series](../../../../../../series-mathematics.md) by the corresponding quadratic to obtain

$$
\sum_{r\geq0}\lambda(p^r)X^r
=\frac1{1-\lambda(p)X+p^{w-1}X^2}.
$$

Unique [prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md) and multiplicativity give

$$
\boxed{L(f,s)=\sum_{n\geq1}\frac{c(n)}{n^s}
=c(1)\prod_p\left(1-\lambda(p)p^{-s}+p^{w-1-2s}\right)^{-1}.}
$$

For a normalized eigenform $c(1)=1$, the prefactor disappears. It must be retained for an arbitrary scalar multiple of that eigenform.

This product identity holds analytically in an absolute-convergence half-plane. The invariant [norm](../../../../../../norm.md) of a positive-weight [cusp form](../../../../../../cusp-form.md) is bounded, as proved in Question 6. For a period-one [Fourier expansion of a modular form](../../../../../../fourier-expansion-of-a-modular-form.md),

$$
|c(n)|\leq e^{2\pi ny}\int_0^1|f(x+iy)|\,dx\leq C e^{2\pi ny}y^{-w/2}.
$$

Choosing $y=1/n$ gives $c(n)=O(n^{w/2})$, so $\operatorname{Re}s>w/2+1$ suffices. [Absolute convergence](../../../../../../absolute-convergence.md) then justifies expansion and rearrangement of the [Euler product of a Hecke eigenform](../../../../../../euler-product-of-a-hecke-eigenform.md); no sharper coefficient estimate is needed here.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
