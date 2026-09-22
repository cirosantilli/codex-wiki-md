<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**[Absolute values](../../../../../../absolute-value.md) are missing in the printed formula.** For signed real blocks, the intended [block mixed norm](../../../../../../block-mixed-norm.md) must be

$$
\|v\|_{q,1}=\sum_{i,j}\left(\sum_{r=1}^d|v^r_{i,j}|^q\right)^{1/q},\qquad q\ge1.
$$

Without them, at $q=1$ a block $(-1,1)$ has value zero although it is nonzero, and a negative [scalar](../../../../../../scalar.md) has negative value. For nonintegral $q$, a negative component may not even have a real power. The literal expression therefore is not a [norm](../../../../../../norm.md) and does not define the claimed general [convex](../../../../../../convex-function.md) problem. Even [integer](../../../../../../integer.md) exponents do not fix all other $q$ in the stated range.

With the corrected [norm](../../../../../../norm.md), let $q'$ be the [Holder conjugate exponent](../../../../../../conjugate-exponents.md): $q'=q/(q-1)$ for $q>1$ and $q'=\infty$ for $q=1$. Blockwise [Holder inequality](../../../../../../holder-inequality.md), with equality from a norming block, gives

$$
\lambda\|Au\|_{q,1}=\sup_{p\in P_{\lambda,q'}}\langle Au,p\rangle,\qquad P_{\lambda,q'}=\{p\in X^d:\|p_{i,j}\|_{q'}\le\lambda\text{ for all }i,j\}.
$$

The [duality of block mixed norms](../../../../../../duality-of-block-mixed-norms.md) identifies the closed [compact](../../../../../../compact-space.md) [convex set](../../../../../../convex-set.md) and the projection residual from the [Moreau decomposition](../../../../../../moreau-decomposition.md)

$$
\boxed{C= A^*P_{\lambda,q'},\qquad u=g-P_Cg.}
$$

For $q=2$, the dual blocks are [Euclidean balls](../../../../../../euclidean-ball.md); for $q=1$, they are cubes given by componentwise bounds $|p^r_{i,j}|\le\lambda$. No injectivity or surjectivity of $A$ is required: [compactness](../../../../../../compact-space.md) of the block product makes its [linear](../../../../../../linearity.md) image [compact](../../../../../../compact-space.md), and the [strictly convex](../../../../../../strictly-convex-function.md) fidelity still gives a unique primal minimizer. For general $q'$, the Euclidean projection onto a dual block ball is not generally obtained by radial scaling, so the special clipping formula from the isotropic case should not be reused without further analysis.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
