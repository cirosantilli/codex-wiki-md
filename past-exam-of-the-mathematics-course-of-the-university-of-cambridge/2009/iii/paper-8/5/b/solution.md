<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [Fredholm](../../../../../../fredholm-operator.md) convention, define

$$
\boxed{\sigma_{\mathrm{ess}}(T)=\{\lambda\in\mathbb C:T-\lambda I\text{ is not Fredholm}\}
=\sigma_{\mathcal Q(H)}([T]).}
$$

The equality follows from the [Atkinson theorem](../../../../../../atkinson-theorem.md). The quotient is a unital complex [Banach algebra](../../../../../../banach-algebra-split.md) when $H$ is infinite-dimensional. Its invertible set is open by the [Neumann series](../../../../../../neumann-series.md), so the spectrum is closed, and it lies in the disk $|\lambda|\leq\|[T]\|$.

For nonemptiness, suppose the quotient resolvent $R(\lambda)=(\lambda1-[T])^{-1}$ existed for every complex $\lambda$. It is analytic everywhere, and outside a sufficiently large disk its Neumann expansion gives $\|R(\lambda)\|\leq1/(|\lambda|-\|[T]\|)$. Continuity bounds it on the remaining compact disk. Every continuous linear functional applied to $R$ is therefore a bounded entire scalar function, constant by Liouville's theorem and zero because it tends to zero at infinity. The Hahn-Banach theorem, or separation by the dual, forces $R(\lambda)=0$, contradicting its inverse identity. **The essential spectrum is nonempty and closed.**

Infinite dimension is necessary: every operator on a finite-dimensional [Hilbert space](../../../../../../hilbert-space-split.md) is [Fredholm](../../../../../../fredholm-operator.md), so its essential spectrum in this convention is empty. The proof works on nonseparable infinite-dimensional spaces as well; it needs neither self-adjointness nor a sequence basis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
