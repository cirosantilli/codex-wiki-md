<h1 id="14h/solution">Solution</h1>

↑ **Parent:** [14H](../14h.md)

An [entire function](../../../../../entire-function.md) that is doubly [periodic](../../../../../periodic-function.md) is bounded: its absolute value has a finite maximum on the compact square $[0,1]+i[0,1]$, and periodic translations carry every point of $\mathbb C$ into that square. The [Liouville theorem](../../../../../liouville-theorem.md) therefore proves **every such analytic function is constant**.

For the zero-pole count, suppose the [meromorphic function](../../../../../meromorphic-function.md) is not identically zero; otherwise isolated zero multiplicities are not defined. It has only finitely many [zeros](../../../../../zero-of-a-function.md) and [poles](../../../../../pole.md) modulo the lattice $\Lambda=\mathbb Z+i\mathbb Z$, because a compact square can be covered by finitely many local meromorphic neighbourhoods. Choose a translated unit square with no [zeros](../../../../../zero-of-a-function.md) or [poles](../../../../../pole.md) on its boundary. The [logarithmic derivative](../../../../../logarithmic-derivative.md) $f'/f$ is doubly [periodic](../../../../../periodic-function.md), so integrals on opposite sides cancel, with their opposite orientations. The [argument principle](../../../../../argument-principle.md) gives

$$
\boxed{N-P=\frac1{2\pi i}\oint\frac{f'(z)}{f(z)}\,dz=0.}
$$

Both counts include multiplicities. Each half-open [fundamental parallelogram](../../../../../fundamental-parallelogram-of-a-period-lattice.md) contains exactly one representative of each lattice orbit, and translation by a lattice vector preserves the multiplicity of a [zero](../../../../../zero-of-a-function.md) or [pole](../../../../../pole.md). Consequently the counts agree in the prescribed half-open square too, even if that particular square has boundary [zeros](../../../../../zero-of-a-function.md) or [poles](../../../../../pole.md). Nonzero constants have both counts zero.

For the series, let $\Lambda=\mathbb Z+i\mathbb Z$ and write it as the [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) $\wp(z)$. On a compact set avoiding $\Lambda$, choose $R$ with $|z|\leq R$. For $|w|>2R$,

$$
\frac1{(z-w)^2}-\frac1{w^2}=\frac{2wz-z^2}{w^2(z-w)^2},\qquad \left|\frac1{(z-w)^2}-\frac1{w^2}\right|\leq\frac{C_R}{|w|^3}.
$$

There are $O(j)$ lattice points with $j\leq|w|<j+1$, hence $\sum_{w\ne0}|w|^{-3}$ converges by comparison with $\sum_jj^{-2}$. The [Weierstrass M-test](../../../../../weierstrass-m-test.md) proves absolute [locally uniform convergence](../../../../../locally-uniform-convergence.md) of the tail, and the finite remaining terms define [holomorphic functions](../../../../../holomorphic-function.md) off their [poles](../../../../../pole.md). It follows that $\wp$ is a [holomorphic function](../../../../../holomorphic-function.md) off $\Lambda$. Near each $w_0\in\Lambda$, separate the term $(z-w_0)^{-2}$; the remaining terms converge locally uniformly to a [holomorphic function](../../../../../holomorphic-function.md). Thus $\wp$ is [meromorphic](../../../../../meromorphic-function.md) on $\mathbb C$, with a double [pole](../../../../../pole.md) at each lattice point and no other [poles](../../../../../pole.md).

It remains to prove the required [periods](../../../../../period-of-a-function.md), rather than merely assert them from the lattice. Termwise [differentiation](../../../../../differentiation.md), justified by [locally uniform convergence](../../../../../locally-uniform-convergence.md) of these holomorphic series, gives

$$
\wp'(z)=-2\sum_{w\in\Lambda}\frac1{(z-w)^3}.
$$

This series is absolutely locally uniformly convergent off $\Lambda$. For either generator $\omega=1,i$, reindexing $w\mapsto w-\omega$ proves $\wp'(z+\omega)=\wp'(z)$. Therefore $\wp(z+\omega)-\wp(z)$ has zero [derivative](../../../../../derivative.md) off $\Lambda$. Its principal parts at lattice points cancel, so it extends to an entire constant $c_\omega$.

The original convergent series is even: reindexing $w\mapsto-w$ gives $\wp(-z)=\wp(z)$. At $z=-\omega/2$, which is not a lattice point for either generator, evenness gives

$$
c_\omega=\wp(\omega/2)-\wp(-\omega/2)=0.
$$

Hence **the series defines a meromorphic function with periods $1$ and $i$**. This [termwise derivative proof of Weierstrass periodicity](../../../../../termwise-derivative-proof-of-weierstrass-periodicity.md) uses an absolutely convergent derivative sum; splitting the original series into two separate inverse-square sums would not be justified.

## ↑ Ancestors (10)

1. [14H](../14h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
