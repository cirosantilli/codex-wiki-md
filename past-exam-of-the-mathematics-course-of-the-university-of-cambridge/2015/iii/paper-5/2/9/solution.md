<h1 id="2/9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

For the subsequent [essential spectrum](../../../../../../essential-spectrum-of-a-closed-operator.md) arguments, the discrete-spectrum definition must use $\operatorname{ran}(L-\lambda I)$ closed, rather than the printed unshifted range. With that correction, $0\notin\Sigma_{\mathrm e}(L)$ means exactly that $N=\ker L$ is finite-dimensional and $\operatorname{ran}L$ is closed; this includes the case $0$ is in the [resolvent set](../../../../../../resolvent-set-of-an-operator.md).

A [closed-range bound on the kernel complement](../../../../../../closed-range-bound-on-the-kernel-complement.md) supplies the useful equivalence

$$
\operatorname{ran}L\text{ closed}\iff\exists b>0:\ \|Lv\|\ge b\|v\|\quad(v\in N^\perp).
$$

For the forward implication, $L:N^\perp\to\operatorname{ran}L$ is a bounded bijection between [Banach spaces](../../../../../../banach-space-split.md), so the [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md) applies. For the reverse implication, any [Cauchy sequence](../../../../../../cauchy-sequence.md) of image points has a [Cauchy sequence](../../../../../../cauchy-sequence.md) of preimages in $N^\perp$, and completeness gives a preimage of its limit.

Now decompose a bounded sequence as $f_n=p_n+v_n$ with $p_n\in N$, $v_n\in N^\perp$. If $Lf_n$ converges, the lower bound makes $(v_n)$ a [Cauchy sequence](../../../../../../cauchy-sequence.md). The [finite-dimensional vector space](../../../../../../finite-dimensional-vector-space.md) $N$ makes the bounded $p_n$ have a convergent subsequence. Their sum has a norm-convergent subsequence.

Conversely, if every bounded sequence with convergent images has a norm-convergent subsequence, the kernel cannot be infinite-dimensional: an [orthonormal sequence](../../../../../../orthonormal-sequence.md) in it would have zero images and no convergent subsequence. If the range were not closed, the lower-bound equivalence would provide unit vectors $v_n\in N^\perp$ with $Lv_n\to0$. Any norm limit would lie in both $N$ and $N^\perp$, hence be zero, contradicting its unit norm. This proves **the required [sequential properness for a self-adjoint operator](../../../../../../sequential-properness-for-a-self-adjoint-operator.md) equivalence**.

The spectral-shift repair is essential for later parts. On $\ell^2$, take $L=\operatorname{diag}(2,1,1/2,1/3,\ldots)$. Its range is not closed, but $2$ is an isolated eigenvalue with one-dimensional eigenspace and closed shifted range. The printed definition would incorrectly place $2$ in the [essential spectrum](../../../../../../essential-spectrum-of-a-closed-operator.md), although no [singular Weyl sequence](../../../../../../singular-weyl-sequence.md) exists there: on the complement of that eigenspace, $\|(L-2I)v\|\ge\|v\|$.

## ↑ Ancestors (11)

1. [9](../9.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
