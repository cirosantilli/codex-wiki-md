<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $r=|\mathbf x|$, $\mathbf n=\mathbf x/r$, and take a [compactly supported](../../../../../../../compact-support.md) [Lighthill stress tensor](../../../../../../../lighthill-stress-tensor.md). The isotropic term in that [tensor](../../../../../../../tensor.md) is $(p-c_0^2\rho)\delta_{ij}$: the [Kronecker delta](../../../../../../../kronecker-delta.md) is implicit in the printed shorthand. Convolving the [Lighthill acoustic analogy](../../../../../../../lighthill-acoustic-analogy.md) with the [retarded acoustic Green function](../../../../../../../retarded-acoustic-green-function.md) and integrating twice by parts in the source coordinates gives

$$
\rho'(\mathbf x,t)=\partial_i\partial_j\int\frac{T_{ij}(\mathbf y,t-|\mathbf x-\mathbf y|/c_0)}{4\pi c_0^2|\mathbf x-\mathbf y|}\,d^3y.
$$

The boundary terms vanish because of [compact support](../../../../../../../compact-support.md). For source size $\ell$, the [acoustic compact-source approximation](../../../../../../../acoustic-compact-source-approximation.md) requires $\omega\ell/c_0\ll1$. At $r\gg\ell$, we may therefore replace the denominator by $r$ and the retarded argument by $t-r/c_0$ in the leading source integral. Define $S_{ij}(t)=\int T_{ij}(\mathbf y,t)d^3y$. In the radiation region $\omega r/c_0\gg1$, the leading two spatial derivatives act on the [retarded time](../../../../../../../retarded-time.md) rather than on $1/r$ or $\mathbf n$:

$$
\partial_i\partial_j\frac{S_{ij}(t-r/c_0)}r\sim\frac{n_in_j}{c_0^2r}\ddot S_{ij}(t-r/c_0).
$$

Thus the leading [acoustic quadrupole](../../../../../../../acoustic-quadrupole.md) density is

$$
\boxed{\rho'(\mathbf x,t)\sim\frac{x_ix_j}{4\pi c_0^4r^3}\ddot S_{ij}(t-r/c_0).}
$$

For the [compact acoustic quadrupole Mach-number scaling](../../../../../../../compact-acoustic-quadrupole-mach-number-scaling.md), let $U$ be the source fluctuation speed, $m=U/c_0\ll1$, and use the advective source time $\ell/U$. With $T_{ij}=O(\rho_0U^2)$, one has $S_{ij}=O(\rho_0U^2\ell^3)$ and $\ddot S_{ij}=O(\rho_0U^4\ell)$. Consequently

$$
\boxed{\frac{\rho'}{\rho_0}=O\!\left(m^4\frac\ell r\right).}
$$

The fourth power refers to the radiation coefficient with geometric spreading separated. It assumes that the source [frequency](../../../../../../../frequency.md) scales as $U/\ell$; an independently imposed frequency or an independently strong thermal source would change that [Mach number](../../../../../../../mach-number.md) estimate.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 82](../../../../paper-82-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
