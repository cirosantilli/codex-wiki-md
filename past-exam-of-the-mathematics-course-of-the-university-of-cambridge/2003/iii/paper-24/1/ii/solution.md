<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The preceding [dimension of level-one modular forms](../../../../../../dimension-of-level-one-modular-forms.md) gives $\dim M_{16}=2$ and $\dim S_{16}=\dim M_4=1$. Thus $E_4\Delta$, which begins with $q$, spans $S_{16}$. A normalized weight-sixteen [Eisenstein series](../../../../../../eisenstein-series.md) and $E_4^4$ both have constant term one, so their difference is a multiple of $E_4\Delta$.

There is a normalization error in the printed auxiliary expansion: for the usual normalized $E_{16}$, the coefficient multiplier is $16320/3617$, rather than $255/(8\cdot3617)$. Indeed, the [Fourier expansion of a normalized Eisenstein series](../../../../../../fourier-expansion-of-a-normalized-eisenstein-series.md) gives $-32/B_{16}$, and the [Bernoulli number](../../../../../../bernoulli-number.md) $B_{16}=-3617/510$ gives $16320/3617$. The printed multiplier is smaller by a factor of $512$. With the correct normalization, the first [Fourier coefficients](../../../../../../fourier-coefficient.md) yield

$$
E_4^4=1+960q+O(q^2),\qquad E_{16}=E_4^4-\frac{3456000}{3617}E_4\Delta.
$$

Comparing all positive-index coefficients therefore gives the exact identity

$$
16320\,\sigma_{15}(n)=3617\,[q^n]E_4^4-3456000\,c_n.
$$

The [Fourier coefficients](../../../../../../fourier-coefficient.md) of $E_4^4$ are integers, as are those of $E_4\Delta$: $E_4$ has its integral divisor-sum expansion and the [modular discriminant](../../../../../../modular-discriminant.md) has the product $q\prod_{r\geq1}(1-q^r)^{24}$. Also $3456000+16320=960\cdot3617$, and $\gcd(16320,3617)=1$. Reducing the identity modulo $3617$ and cancelling the invertible multiplier proves the [weight-sixteen Eisenstein congruence](../../../../../../weight-sixteen-eisenstein-congruence.md)

$$
\boxed{c_n\equiv\sigma_{15}(n)\pmod{3617}\qquad(n\geq1).}
$$

The desired congruence is valid; it is the auxiliary normalization in the PDF that requires correction.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
