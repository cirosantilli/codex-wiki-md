<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

On each branch the [worm-like chain force-extension interpolation](../../../../worm-like-chain-force-extension-interpolation.md) relates [force](../../../../force-split.md) to the extension of the already released chain. Fitting a sufficiently long branch estimates its [polymer contour length](../../../../polymer-contour-length.md) $L$ and, if the data constrain it independently, its [persistence length](../../../../persistence-length.md) $L_p$. In practice $L_p$ may be fixed across branches so that the changes in $L$ are better identified. Consecutive fitted [polymer contour lengths](../../../../polymer-contour-length.md) reveal how much additional chain became available at an [protein denaturation](../../../../denaturation-biochemistry.md) event; using a justified [polymer contour length](../../../../polymer-contour-length.md) per residue can then estimate residue counts. A projected folded length and the pulling geometry must be included before assigning a structural boundary.

Writing $u=x/L$, expansion at small extension gives

$$
f=\frac{k_BT}{L_p}\left(\frac32u+\frac34u^2+\cdots\right),\qquad
k_{\rm eff}=\left.\frac{df}{dx}\right|_0=\frac{3k_BT}{2L_pL}.
$$

Near full extension, $f\sim k_BT/[4L_p(1-x/L)^2]$. Larger $L$ shifts a branch toward larger extension at fixed [force](../../../../force-split.md). The effective [flexural rigidity](../../../../bending-stiffness.md) is $\kappa=k_BT L_p$, with units of [force](../../../../force-split.md) times length squared. This is entropic straightening of a [worm-like chain](../../../../worm-like-chain.md); bond stretching and barrier rupture themselves are not included in the formula.

**The persistence-length wording requires care.** The three-dimensional model gives $\langle\mathbf t(s)\cdot\mathbf t(0)\rangle=e^{-s/L_p}$. At $s=L_p$, $\arccos\langle\cos\theta\rangle=\arccos(e^{-1})=68.4^\circ$. This is not a statement that $\langle\theta\rangle=68.4^\circ$. For example, angles zero and $90^\circ$ with equal [probabilities](../../../../probability.md) have mean angle $45^\circ$, but $\arccos\langle\cos\theta\rangle=60^\circ$. The distinction prevents a false literal interpretation of the printed definition.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
