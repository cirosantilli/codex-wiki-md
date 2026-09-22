<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $M$ bound the piecewise [Hölder norms](../../../../../../holder-norm.md), and let $B=\|f\|_\infty$. At scale $j$, classify a [wavelet](../../../../../../wavelet.md) as bad when its localized [support of a function](../../../../../../support.md) meets a discontinuity, and as good otherwise. [Compact support](../../../../../../compact-support.md) and bounded overlap imply at most $C_0K$ bad [wavelets](../../../../../../wavelet.md) per scale and at most $C_12^j$ total [wavelets](../../../../../../wavelet.md). A good support lies in a single [smooth](../../../../../../smooth-function.md) piece, so the preceding [wavelet coefficient decay for Hölder functions](../../../../../../wavelet-coefficient-decay-for-holder-functions.md) gives $|c_{j,n}|\le C M2^{-j(\alpha+1/2)}$. The permitted bounded-function estimate gives $|c_{j,n}|\le C B2^{-j/2}$ for bad coefficients.

Consider a specific [N-term approximation](../../../../../../n-term-approximation.md): retain all coarse [scaling functions](../../../../../../scaling-function.md) and all [wavelets](../../../../../../wavelet.md) through scale $J$, and also retain the bad coefficients at scales $J<j\le L$, where $L=\lceil2\alpha J\rceil$. Since $\alpha>1/2$, $L\ge J$ for large $J$. Its term count is bounded by

$$
N_J\le C_2 2^J+C_3K(L-J)+C_4=O(2^J+KJ).
$$

By the [Parseval identity](../../../../../../parseval-identity.md), its squared [L2 norm](../../../../../../l2-norm.md) error is the sum of omitted squared coefficients. The good tail satisfies

$$
\sum_{j>J}\sum_{n\ \mathrm{good}}|c_{j,n}|^2\le C M^2\sum_{j>J}2^j2^{-2j(\alpha+1/2)}\le C'M^22^{-2\alpha J},
$$

and the remaining bad tail satisfies

$$
\sum_{j>L}\sum_{n\ \mathrm{bad}}|c_{j,n}|^2\le C K B^2\sum_{j>L}2^{-j}\le C'KB^22^{-L}\le C'KB^22^{-2\alpha J}.
$$

Choose $J=\lfloor\log_2(N/(2C_2'))\rfloor$ with a fixed sufficiently large $C_2'$; then the $O(KJ)$ extra terms fit the remaining budget for all sufficiently large $N$, while $2^J$ is comparable to $N$. Padding to $N$ terms does not increase the error. The [best N-term approximation](../../../../../../best-n-term-approximation.md) is at least as accurate as this constructed selection, so

$$
\boxed{\epsilon_n(N,f)=\|f-f_N^{\mathrm{nonlin}}\|_2^2=O(N^{-2\alpha}).}
$$

The constant may depend on the finite number of jumps, the piecewise [Hölder norms](../../../../../../holder-norm.md), $B$ and the fixed [wavelet](../../../../../../wavelet.md) family. Values exactly at the jumps are immaterial in $L^2$. The improvement comes from retaining only a bounded number of jump-crossing coefficients at each finer scale, as in [best N-term wavelet approximation of piecewise Hölder functions](../../../../../../best-n-term-wavelet-approximation-of-piecewise-holder-functions.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
