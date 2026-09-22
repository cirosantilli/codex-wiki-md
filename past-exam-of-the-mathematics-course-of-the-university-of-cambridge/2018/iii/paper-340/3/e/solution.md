<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use localized [tensor-product wavelets](../../../../../../tensor-product-wavelet.md) and finitely many bounded polynomial pieces, with the [boundary wavelets](../../../../../../boundary-wavelet.md) adapted as in part (b). A rectifiable smooth curve of length $\ell$ meets $O(1+\ell2^j)$ dyadic squares of side $2^{-j}$: subdividing an arclength parametrization into pieces of length at most $2^{-j}$ covers it by that many balls, each meeting only a bounded number of squares. Enlarging squares by the fixed support diameter preserves the count.

Each normalized two-dimensional [wavelet](../../../../../../wavelet.md) has $L^1$ [norm](../../../../../../norm.md) $O(2^{-j})$. A coefficient meeting the curve is therefore $O(2^{-j})$, and the total squared energy of these coefficients at level $j$ is $O(2^{-j})$. If $p<q$, all other coefficients vanish by the [vanishing moments](../../../../../../vanishing-moment.md). Keeping the curve coefficients through level $J$ costs $O(2^J)$ and leaves squared error $O(2^{-J})$.

The printed part (e) does not repeat $p<q$. The bound still holds for any fixed polynomial degree when $q\ge1$: on a smooth piece, a [Taylor polynomial](../../../../../../taylor-polynomial.md) in the variable carrying a [wavelet](../../../../../../wavelet.md) gives coefficient size $O(2^{-(q+1)j})$. There are $O(4^j)$ such coefficients, so their squared energy is $O(2^{-2qj})$. Retain all coefficients through $K=\lfloor J/2\rfloor$, and curve coefficients through $J$. The cost is $O(4^K+2^J)=O(2^J)$ and the omitted squared energy is

$$
O(2^{-2qK}+2^{-J})=O(2^{-J}).
$$

The [best N-term approximation](../../../../../../best-n-term-approximation.md) is at least as good as this selection, proving

$$
\boxed{\|f-f_N^n\|_2^2=O(N^{-1}).}
$$

This argument covers the unqualified finite-degree clause without adding an unnecessary restriction $p<q$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
