<h1 id="21f/solution">Solution</h1>

↑ **Parent:** [21F](../21f.md)

By the [argument principle](../../../../../argument-principle.md), the number of zeros minus poles, counted with multiplicity, in the fundamental parallelogram is $(2\pi i)^{-1}\oint f'/f\,dz$. The logarithmic [derivative](../../../../../derivative.md) is periodic with the same lattice, so the [integrals](../../../../../integral.md) over opposite sides cancel. Thus **the numbers of zeros and poles are equal**.

The [Weierstrass elliptic function](../../../../../weierstrass-elliptic-function.md) gives a degree-two map $\wp:\mathbb C/\Lambda\to\mathbb P^1$ whose fibers identify $z$ and $-z$. An even [elliptic function](../../../../../elliptic-function.md) is constant on these fibers, so it descends to a single-valued function $Q$ on the [sphere](../../../../../sphere.md). This is meromorphic even at a branch value: near a half-period the involution is $t\mapsto-t$, the [Laurent series](../../../../../laurent-series.md) of $f$ has only even powers, and $\wp-\wp_0$ has a double zero and provides a local coordinate in $t^2$. At the image of $0$, $\wp\sim t^{-2}$ gives the same conclusion at infinity. A [meromorphic function](../../../../../meromorphic-function.md) on the [Riemann sphere](../../../../../riemann-sphere.md) is a [rational function](../../../../../rational-function.md), so $\boxed{f=Q(\wp)}$.

**A meromorphic antiderivative need not be elliptic.** Take $f=\wp$. Its double poles have zero [residue](../../../../../residue.md), so integrating on the punctured plane gives a single-valued primitive, since every closed-contour [integral](../../../../../integral.md) is a sum of zero [residues](../../../../../residue.md). The primitive extends meromorphically over each pole, with local principal part $-1/z$. If $F$ were elliptic, it would have precisely one pole modulo the lattice, with [residue](../../../../../residue.md) $-1$, contradicting the zero sum of [residues](../../../../../residue.md) in a fundamental parallelogram. This is a nonconstant counterexample satisfying the stated premise; the preceding descent proves that [even elliptic functions are rational in the Weierstrass function](../../../../../even-elliptic-functions-are-rational-in-the-weierstrass-function.md).

## ↑ Ancestors (10)

1. [21F](../21f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
