<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [linear independence](../../../../../../linear-independence.md) of the first $n$ elements of each [orthonormal system](../../../../../../orthonormal-sequence.md) shows that $T_n$ and $S_n$ have the same finite [dimension](../../../../../../dimension-vector-space.md) $n$ and are [closed subspaces of a Hilbert space](../../../../../../closed-subspace-of-a-hilbert-space.md). Apply part (b) with $U=T_n$ and $V=S_n^\perp$. Since $(S_n^\perp)^\perp=S_n$, the positive [directed subspace angle](../../../../../../directed-subspace-angle.md) cosine gives

$$
H=T_n\oplus S_n^\perp.
$$

Let $Q$ be the [oblique projection](../../../../../../oblique-projection.md) onto $T_n$ along $S_n^\perp$. Define $\widetilde f_n=Qf$. Its residual $f-Qf$ is orthogonal to every $\psi_j$ with $1\le j\le n$, so the required measurements agree. Conversely, if $g\in T_n$ has the same measurements, then $f-g\in S_n^\perp$; uniqueness of the [direct sum](../../../../../../direct-sum.md) decomposition gives $g=Qf$. Thus this is [finite-dimensional Hilbert sampling reconstruction](../../../../../../finite-dimensional-hilbert-sampling-reconstruction.md).

There is also an explicit coefficient description. Use the [inner product](../../../../../../inner-product.md) convention linear in its first entry and put

$$
C_{jk}=\langle\phi_k,\psi_j\rangle,\qquad b_j=\langle f,\psi_j\rangle,\qquad\widetilde f_n=\sum_{k=1}^n c_k\phi_k.
$$

Then $Cc=b$. The [orthonormal systems](../../../../../../orthonormal-sequence.md) show $\|P_{S_n}\sum_k c_k\phi_k\|=\|Cc\|_2$ and $\|\sum_k c_k\phi_k\|=\|c\|_2$, so the smallest [singular value](../../../../../../singular-value.md) of $C$ is $\cos\theta_{T_n,S_n}>0$. Hence $c=C^{-1}b$, another direct proof of existence and uniqueness.

For $n\ge1$, both summands of this [direct sum](../../../../../../direct-sum.md) are nonzero: the infinite [orthonormal system](../../../../../../orthonormal-sequence.md) $(\psi_j)$ contains $\psi_{n+1}\in S_n^\perp$. The permitted [oblique projection](../../../../../../oblique-projection.md) norm formula therefore applies without its degenerate exception, giving

$$
\|Q\|=\|I-Q\|=\sec\theta_{T_n,S_n}.
$$

The [operator norm](../../../../../../operator-norm.md) immediately yields the stability estimate $\|\widetilde f_n\|\le\sec\theta_{T_n,S_n}\|f\|$. For the approximation bounds, put $e=f-P_{T_n}f$. Because $Q$ fixes $T_n$, we have

$$
f-Qf=(I-Q)e,
$$

so the [operator norm](../../../../../../operator-norm.md) estimate gives $\|f-Qf\|\le\sec\theta_{T_n,S_n}\|e\|$. For the lower bound, $e\perp T_n$ while $P_{T_n}f-Qf\in T_n$. The [Pythagorean identity](../../../../../../pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|f-Qf\|^2=\|e\|^2+\|P_{T_n}f-Qf\|^2\ge\|e\|^2.
$$

**The unique measurement-matching reconstruction is stable and within the [secant function](../../../../../../secant-trigonometry.md) factor of the best [orthogonal projection](../../../../../../orthogonal-projection.md) approximation:**

$$
\boxed{\widetilde f_n=Qf,\quad\|\widetilde f_n\|\le\sec\theta_{T_n,S_n}\|f\|,\quad\|f-P_{T_n}f\|\le\|f-\widetilde f_n\|\le\sec\theta_{T_n,S_n}\|f-P_{T_n}f\|.}
$$

If a zero-dimensional reconstruction is admitted, it is simply $\widetilde f_0=0$ and its error equals the [norm](../../../../../../norm.md) of $f$; that case is best stated directly instead of using the angle of a zero space.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
