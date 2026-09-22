<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a first-order system, it is important to specify the frame in which its coefficients are written. In the simple-pole convention intended here, a [Fuchsian linear differential system](../../../../../fuchsian-linear-differential-system.md) has, at a finite singular point $a$,

$$
A(z)=\frac{R_a}{z-a}+H_a(z),\qquad H_a\text{ holomorphic near }a.
$$

The [residue](../../../../../residue.md) is the matrix $R_a=\lim_{z\to a}(z-a)A(z)$, computed entry by entry. Such a point is a [regular singular point](../../../../../regular-singular-point.md): on a sector, the coefficient bound $\|A(z)\|\le C/|z-a|$ and integration along rays give at most power growth of solutions. Intrinsically, a [regular singular point](../../../../../regular-singular-point.md) means moderate power growth of all solutions on sectors, allowing logarithmic factors. This intrinsic definition is more general than requiring a simple coefficient pole in an arbitrary meromorphic frame.

For $A(z)=R/z$, a [fundamental matrix](../../../../../fundamental-matrix-of-a-linear-differential-equation.md) on a chosen [complex logarithm](../../../../../complex-logarithm.md) branch is

$$
\Phi(z)=\exp(R\log z).
$$

Differentiating the [matrix exponential](../../../../../matrix-exponential.md) verifies $\Phi'=R\Phi/z$. A counterclockwise circuit replaces $\log z$ by $\log z+2\pi i$, so

$$
\Phi\longmapsto\Phi M,\qquad
\boxed{M=e^{2\pi iR},\quad \text{monodromy group }=\{M^n:n\in\mathbb Z\}.}
$$

This is the [residue and monodromy of a constant Fuchsian system](../../../../../residue-and-monodromy-of-a-constant-fuchsian-system.md). A change of solution basis conjugates $M$. Its [eigenvalues](../../../../../eigenvalue.md) are $e^{2\pi i\lambda}$ for the residue [eigenvalues](../../../../../eigenvalue.md) $\lambda$; a nontrivial [Jordan block](../../../../../jordan-block.md) supplies the corresponding logarithmic terms in $z^R$. The [monodromy](../../../../../monodromy.md) does not uniquely recover $R$, since integer shifts of residue [eigenvalues](../../../../../eigenvalue.md) can leave their exponentials unchanged.

The coordinate-independent coefficient is the matrix-valued one-form $A(z)\,dz$. With $t=1/z$, its coefficient is

$$
\widetilde A(t)=-t^{-2}A(1/t).
$$

Being Fuchsian at infinity means $A(z)=O(z^{-1})$, while being ordinary there means $A(z)=O(z^{-2})$. If the finite simple poles are $a_1,\ldots,a_s$, subtract their principal parts:

$$
H(z)=A(z)-\sum_{j=1}^s\frac{R_j}{z-a_j}.
$$

Each entry of $H$ is [entire](../../../../../entire-function.md) and tends to zero at infinity. [Liouville's theorem](../../../../../liouville-theorem.md) therefore gives $H=0$. Expanding this [partial fraction decomposition](../../../../../partial-fraction-decomposition.md) at infinity yields

$$
\boxed{A(z)=\sum_{j=1}^s\frac{R_j}{z-a_j},\qquad R_\infty=-\sum_{j=1}^sR_j.}
$$

Thus the sum of all [residues](../../../../../residue.md), including the [residue](../../../../../residue.md) at infinity of the one-form, is zero. If infinity is ordinary, $R_\infty=0$ and the finite [residues](../../../../../residue.md) alone sum to zero. Treating $A$ merely as a scalar function of $z$, without transforming $dz$, would give the wrong infinity convention.

Put $\omega=e^{2\pi i/3}$. The possible finite singular points of $(B+zC)/(1-z^3)$ are $1,\omega,\omega^2$, and

$$
R_\zeta=-\frac{B+\zeta C}{3\zeta^2}\qquad(\zeta^3=1).
$$

A point $\zeta$ is removable exactly when $B+\zeta C=0$ as a matrix. At infinity,

$$
\widetilde A(t)=\frac{C+tB}{1-t^3},
$$

which is [holomorphic](../../../../../complex-differentiability-at-a-point.md) at $t=0$. Consequently **the actual set is $S=\{\zeta:\zeta^3=1,\ B+\zeta C\ne0\}$**, with $\{1,\omega,\omega^2\}$ the generic set. The finite [residues](../../../../../residue.md) sum to zero, as follows also from $\sum_{\zeta^3=1}\zeta^{-1}=\sum_{\zeta^3=1}\zeta^{-2}=0$.

Conversely, suppose a [Fuchsian linear differential system](../../../../../fuchsian-linear-differential-system.md) has its finite singular points among these three roots and has no singularity at infinity. Then $Q(z)=(1-z^3)A(z)$ extends to an [entire](../../../../../entire-function.md) matrix function, and ordinariness at infinity gives $Q(z)=O(z)$. By the [Cauchy estimate](../../../../../cauchy-estimate.md), each entry has zero derivatives of order two or higher, so $Q(z)=B+zC$. The same argument applies to any subset $S$, with additional cancellations at the omitted roots. This proves the requested normal form.

There is a genuine convention limitation: the normal form is not true under intrinsic regular singularity alone in an unrestricted frame. For example, if $N\ne0$ and $N^2=0$, then $A(z)=N/(z-1)^2$ has [fundamental matrix](../../../../../fundamental-matrix-of-a-linear-differential-equation.md) $I-N/(z-1)$. Its solutions have only power growth, so $1$ is intrinsically a [regular singular point](../../../../../regular-singular-point.md), and infinity is ordinary. Nevertheless its coefficient has a double pole and cannot equal $(B+zC)/(1-z^3)$. The simple-pole convention makes the preceding residue and normal-form assertions correct.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
