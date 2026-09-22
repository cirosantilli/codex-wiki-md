<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a probability [measure-preserving system](../../../../../measure-preserving-system.md), **[weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md) is the vanishing of averaged absolute correlation discrepancies**:

$$
\boxed{\frac1N\sum_{n=0}^{N-1}
\left|\mu(T^{-n}A\cap B)-\mu(A)\mu(B)\right|
\longrightarrow0
\quad(A,B\in\mathcal B).}
$$

By approximation with simple functions and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), this is equivalent to

$$
\frac1N\sum_{n=0}^{N-1}
\left|\langle U^nf,g\rangle-\left(\int f\,d\mu\right)
\overline{\left(\int g\,d\mu\right)}\right|\longrightarrow0
\qquad(f,g\in L^2).
$$

Here $\langle f,g\rangle=\int f\overline g\,d\mu$, and $U=U_T$. Absolute values are part of the definition: signed [Cesaro convergence of a sequence](../../../../../cesaro-convergence-of-a-sequence.md) of these correlations alone expresses [ergodicity](../../../../../ergodicity.md), not [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md).

Suppose the product system is [ergodic](../../../../../ergodicity.md). Fix a mean-zero $f\in L^2(\mu)$ and any $g\in L^2(\mu)$. On the product take

$$
F(x,y)=f(x)\overline{f(y)},\qquad
G(x,y)=g(x)\overline{g(y)}.
$$

These belong to $L^2(\mu\otimes\mu)$, and $\int F=|\int f|^2=0$. The [mean ergodic theorem](../../../../../von-neumann-mean-ergodic-theorem.md) on the product, followed by pairing with $G$, gives

$$
\frac1N\sum_{n=0}^{N-1}|\langle U^nf,g\rangle|^2
=\left\langle\frac1N\sum_{n=0}^{N-1}(U\otimes U)^nF,G\right\rangle
\longrightarrow0.
$$

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) in $n$ bounds the averaged absolute correlation by the square root of this quantity. Subtract the mean from a general $f$ to obtain the definition above. This proves **product [ergodicity](../../../../../ergodicity.md) implies [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md)**, through the [square-correlation proof of weak mixing from product ergodicity](../../../../../square-correlation-proof-of-weak-mixing-from-product-ergodicity.md).

For the multiple averages, write $m(f)=\int f\,d\mu$ and use the following [Van der Corput lemma](../../../../../van-der-corput-lemma-hilbert-space-sequences.md). If $(v_n)$ is bounded in a [Hilbert space](../../../../../hilbert-space-split.md), every correlation average

$$
L_h=\lim_{N\to\infty}\frac1N\sum_{n=0}^{N-1}
\langle v_{n+h},v_n\rangle
$$

exists, and $H^{-1}\sum_{h=1}^H|L_h|\to0$, then $N^{-1}\sum_{n<N}v_n\to0$ in norm. One way to see the estimate is to replace $v_n$ by $H^{-1}\sum_{j=0}^{H-1}v_{n+j}$; for fixed $H$ the change in its long average tends to zero. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and expansion of the squared block norm give

$$
\limsup_{N\to\infty}\left\|\frac1N\sum_{n<N}v_n\right\|^2
\leq\frac{M^2}{H}
+\frac2H\sum_{h=1}^{H-1}\left(1-\frac hH\right)|L_h|,
\qquad M=\sup_n\|v_n\|.
$$

Let $H\to\infty$. This proves the auxiliary implication needed here.

A [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md) system is [ergodic](../../../../../ergodicity.md): a mean-zero invariant $f$ would have the nonvanishing correlation $\langle U^nf,f\rangle=\|f\|_2^2$. Every positive power $T^r$ is also [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md), since for nonnegative correlation discrepancies $b_n$,

$$
\frac1H\sum_{h=0}^{H-1}b_{rh}
\leq\frac r{rH}\sum_{n=0}^{rH-1}b_n\longrightarrow0.
$$

This part of the [stability of weak mixing under powers and products](../../../../../stability-of-weak-mixing-under-powers-and-products.md) will control the induction.

In fact the stronger [arithmetic-progression multiple averages under weak mixing](../../../../../arithmetic-progression-multiple-averages-under-weak-mixing.md) holds:

$$
\boxed{\frac1N\sum_{n=0}^{N-1}
\prod_{j=1}^k U^{jn}f_j
\longrightarrow\prod_{j=1}^k m(f_j)
\quad\text{in }L^2,\qquad f_j\in L^\infty.}
$$

For $k=1$ this is the [mean ergodic theorem](../../../../../von-neumann-mean-ergodic-theorem.md) and [ergodicity](../../../../../ergodicity.md). Suppose it is known for $k-1$ and first assume $m(f_k)=0$. Put $v_n=\prod_{j=1}^kU^{jn}f_j$. For fixed $h$, set

$$
g_{j,h}=(U^{jh}f_j)\overline{f_j}.
$$

Using invariance of the integral to remove the common $U^n$ gives

$$
\langle v_{n+h},v_n\rangle
=\int g_{1,h}\prod_{j=2}^k U^{(j-1)n}g_{j,h}\,d\mu.
$$

This identity does not require an inverse of $T$. Apply the induction hypothesis to the $k-1$ factors and pair their $L^2$ limit with $g_{1,h}$. It follows that

$$
L_h=\prod_{j=1}^k m(g_{j,h}),\qquad
|L_h|\leq
\left(\prod_{j=1}^{k-1}\|f_j\|_\infty^2\right)
|\langle U^{kh}f_k,f_k\rangle|.
$$

The average in $h$ of the right side tends to zero because $T^k$ is [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md) and $m(f_k)=0$. The [Van der Corput lemma](../../../../../van-der-corput-lemma-hilbert-space-sequences.md) proves the zero $L^2$ limit. For general $f_k$, split it into $f_k-m(f_k)$ and its constant mean; the first term has the zero limit just proved, and the other term is $m(f_k)$ times the induction average for $k-1$. This completes the induction.

Pair this result with the real bounded $f_0$. For

$$
a_n=\int f_0\prod_{j=1}^kU^{jn}f_j\,d\mu,\qquad
\ell=\prod_{j=0}^km(f_j),
$$

**the requested [Cesaro limit](../../../../../cesaro-convergence-of-a-sequence.md) is**

$$
\boxed{\operatorname{C-lim}_{n\to\infty}a_n=\ell.}
$$

To obtain [convergence in density of a sequence](../../../../../convergence-in-density-of-a-sequence.md), we also need the product system to be [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md). For simple tensors, its correlations are products of single-system correlations. If $c_n\to c$ and $d_n\to d$ in averaged absolute discrepancy and both sequences are bounded, then

$$
|c_nd_n-cd|\leq |c_n-c|\,|d_n|+|c|\,|d_n-d|,
$$

so the product discrepancy has zero average. Finite sums of tensors are dense in $L^2(\mu\otimes\mu)$, and the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) extends the conclusion to arbitrary $L^2$ functions. Hence $T\times T$ is [weak mixing](../../../../../weakly-mixing-measure-preserving-transformation.md).

Apply the multiple-average result to $F_j=f_j\otimes f_j$ on that product. Because the original $f_j$ are real,

$$
\frac1N\sum_{n<N}a_n^2
\longrightarrow\prod_{j=0}^k\left(\int F_j\,d(\mu\otimes\mu)\right)
=\ell^2.
$$

Together with the first-moment limit this gives

$$
\frac1N\sum_{n<N}|a_n-\ell|^2\longrightarrow0.
$$

The [mean-square criterion for convergence in density](../../../../../mean-square-criterion-for-convergence-in-density.md) now yields, for every $\varepsilon>0$,

$$
\frac1N\#\{0\leq n<N:|a_n-\ell|\geq\varepsilon\}
\leq\frac1{\varepsilon^2N}\sum_{n<N}|a_n-\ell|^2\longrightarrow0.
$$

Therefore **the [density convergence of multiple weak-mixing correlations](../../../../../density-convergence-of-multiple-weak-mixing-correlations.md) gives the same answer**:

$$
\boxed{\operatorname{D-lim}_{n\to\infty}a_n
=\prod_{j=0}^k\int f_j\,d\mu.}
$$

The second-moment argument is essential; the signed [Cesaro limit](../../../../../cesaro-convergence-of-a-sequence.md) alone would not imply this conclusion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
