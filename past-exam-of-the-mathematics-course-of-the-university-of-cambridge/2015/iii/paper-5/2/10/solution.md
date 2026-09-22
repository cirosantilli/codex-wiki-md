<h1 id="2/10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Use the corrected [essential spectrum of a bounded self-adjoint operator](../../../../../../essential-spectrum-of-a-bounded-self-adjoint-operator.md) and put $A=L-\lambda I$. Essential spectral points are real. If $\ker A$ is infinite-dimensional, choose an [orthonormal sequence](../../../../../../orthonormal-sequence.md) in the kernel. It converges weakly to zero by the [Bessel inequality](../../../../../../bessel-s-inequality.md), and its residuals vanish.

If $\ker A$ is finite-dimensional, membership in the [essential spectrum](../../../../../../essential-spectrum-of-a-closed-operator.md) means the range is not closed. Choose unit $v_n\in(\ker A)^\perp$ with $Av_n\to0$, using the [closed-range bound on the kernel complement](../../../../../../closed-range-bound-on-the-kernel-complement.md). A bounded [Hilbert space](../../../../../../hilbert-space-split.md) sequence has a weakly convergent subsequence. Its weak limit $v$ satisfies $Av=0$ because bounded operators preserve [weak convergence](../../../../../../weak-convergence.md), and $v\in(\ker A)^\perp$; hence $v=0$. This subsequence is a [singular Weyl sequence](../../../../../../singular-weyl-sequence.md).

Conversely a [singular Weyl sequence](../../../../../../singular-weyl-sequence.md) first places $\lambda$ in the [spectrum of a bounded operator](../../../../../../spectrum-of-a-bounded-operator.md). If it were not essential, the [sequential properness for a self-adjoint operator](../../../../../../sequential-properness-for-a-self-adjoint-operator.md) equivalence for $A$ would yield a norm-convergent subsequence. Its weak limit is zero, whereas norm convergence of unit vectors gives a unit norm limit, a contradiction. Therefore

$$
\boxed{\lambda\in\Sigma_{\mathrm e}(L)\iff\exists(f_n):\ \|f_n\|=1,\ f_n\rightharpoonup0,\ (L-\lambda I)f_n\to0.}
$$

For nonreal $\lambda$, the resolvent lower bound excludes such a sequence, so the equivalence covers all $\lambda\in\mathbb C$.

## ↑ Ancestors (11)

1. [10](../10.md)
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
