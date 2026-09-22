<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $M>0$, integrate the vector action by parts, dropping the boundary term, and write it as a quadratic functional:

$$
S_0[A]=\frac12\int d^4x\,A_\mu K^{\mu\nu}A_\nu,\qquad
K^{\mu\nu}=(\Box-M^2)g^{\mu\nu}-\partial^\mu\partial^\nu.
$$

The explicit [mass](../../../../mass.md) makes this Proca [kernel](../../../../kernel-of-a-linear-map-split.md) invertible: the displayed action alone has no gauge redundancy left to fix. It is interpreted as [unitary gauge](../../../../unitary-gauge.md) when obtained from a Higgs or Stückelberg completion with its would-be Goldstone field removed.

Introduce a source $J_\mu$ and complete the square, $A=A'-K^{-1}J$. The normalized Gaussian [path integral](../../../../path-integral.md) is

$$
\boxed{\frac{Z[J]}{Z[0]}=\exp\left[-\frac i2\int d^4x\,d^4y\,
J_\mu(x)(K^{-1})^{\mu\nu}(x,y)J_\nu(y)\right],\qquad
\widetilde D_{\mu\nu}=i(\widetilde K^{-1})_{\mu\nu}.}
$$

The source-independent [functional determinant](../../../../functional-determinant.md) cancels in $Z[J]/Z[0]$. For Fourier [momentum](../../../../momentum-split.md) $k$, the mixed-index [kernel](../../../../kernel-of-a-linear-map-split.md) is $\widetilde K^\mu{}_{\nu}=-(k^2+M^2)\delta^\mu{}_{\nu}+k^\mu k_\nu$. For $k^2\ne0$, use the [projectors](../../../../projection-linear-algebra.md)

$$
P_L{}^\mu{}_{\nu}=\frac{k^\mu k_\nu}{k^2},\qquad P_T=I-P_L.
$$

Their orthogonality gives

$$
\widetilde K=-(k^2+M^2)P_T-M^2P_L,\qquad
\widetilde K^{-1}=-\frac{P_T}{k^2+M^2}-\frac{P_L}{M^2}.
$$

Combining the [projectors](../../../../projection-linear-algebra.md) removes their apparent massless denominator. Adding the Feynman prescription gives the unitary-gauge propagator

$$
\boxed{\widetilde D_{\mu\nu}(k)=\frac{-i}{k^2+M^2-i0}
\left(g_{\mu\nu}+\frac{k_\mu k_\nu}{M^2}\right).}
$$

Multiplication by $\widetilde K$ verifies that it inverts the quadratic operator. On the physical pole $k^2=-M^2$, the numerator is transverse to $k$, as required for the three physical massive-vector polarizations.

The drawback is its off-shell ultraviolet behaviour: at large spacelike [momentum](../../../../momentum-split.md) the transverse term falls as $1/k^2$, but the longitudinal tensor term remains of order $1/M^2$. Naive loop [power counting](../../../../power-counting-in-quantum-field-theory.md) therefore looks worse and [renormalizability](../../../../renormalizable-quantum-field-theory.md) is not manifest. In a finite $R_\xi$ gauge the corresponding expression is

$$
D_\xi=-i\left[\frac{P_T}{k^2+M^2-i0}+\frac{\xi P_L}{k^2+\xi M^2-i0}\right],
$$

which falls as $1/k^2$ at fixed finite $\xi$. Its $\xi\to\infty$ limit gives the unitary-gauge longitudinal term, so taking that limit before the ultraviolet limit changes [power counting](../../../../power-counting-in-quantum-field-theory.md).

This is not a claim that a renormalizable Higgs theory ceases to be physically renormalizable in this gauge. Nor does it mean that the free Proca [Gaussian integral](../../../../gaussian-integral.md) is inconsistent. For conserved external sources $k\cdot J=0$, the longitudinal numerator drops out of $J^\mu D_{\mu\nu}J^\nu$ and the tree exchange again falls as $1/k^2$. The difficulty concerns off-shell [Green functions](../../../../green-s-function-split.md) and manifest control of loop divergences, not the number of physical polarizations.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
