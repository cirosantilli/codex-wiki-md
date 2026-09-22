<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the mode normalization given, the oscillator [canonical commutation relations](../../../../../../canonical-commutation-relation.md) are $[a_{\mathbf p},a_{\mathbf q}^\dagger]=(2\pi)^3\delta^3(\mathbf p-\mathbf q)$, with the other two [commutators](../../../../../../commutator.md) zero. Let $E_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$ and $p^0=E_{\mathbf p}$. The convention compatible with the requested numerator is

$$
\Delta_F(x-y)=\langle0|T\{\phi(x)\phi(y)\}|0\rangle,
$$

without an additional factor of $i$ outside the [vacuum expectation value](../../../../../../vacuum-expectation-value.md). Put $\tau=x^0-y^0$ and $\mathbf r=\mathbf x-\mathbf y$. The [Fock vacuum](../../../../../../fock-vacuum.md) is annihilated by $a_{\mathbf p}$, so only $aa^\dagger$ contributes to the two [Wightman functions](../../../../../../wightman-function.md). Consequently,

$$
\Delta_F(\tau,\mathbf r)=\int\frac{d^3p}{(2\pi)^3}\frac{e^{i\mathbf p\cdot\mathbf r}}{2E_{\mathbf p}}\left(\theta(\tau)e^{-iE_{\mathbf p}\tau}+\theta(-\tau)e^{iE_{\mathbf p}\tau}\right).
$$

In the second term we changed $\mathbf p\mapsto-\mathbf p$ to give the same spatial exponential.

Now perform the [energy](../../../../../../energy.md) [contour integral](../../../../../../contour-integral.md)

$$
g_E(\tau)=\lim_{\epsilon\downarrow0}\int\frac{dp^0}{2\pi}\frac{i\,e^{-ip^0\tau}}{(p^0)^2-E^2+i\epsilon}.
$$

Here the residue step uses $E>0$; the massless zero-momentum point is interpreted through the smeared [distribution](../../../../../../distribution-mathematical-analysis.md) limit, not as an isolated normalized oscillator. The [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) puts the positive-energy pole below the real axis and the negative-energy pole above it: $p^0=E-i0$ and $p^0=-E+i0$. For $\tau>0$, close in the lower half-plane, clockwise; the [residue theorem](../../../../../../residue-theorem.md) gives $-i$ times the residue $ie^{-iE\tau}/(2E)$, hence $e^{-iE\tau}/(2E)$. For $\tau<0$, close in the upper half-plane, counterclockwise; the negative-energy residue is $-ie^{iE\tau}/(2E)$, again giving a positive $e^{iE\tau}/(2E)$. These are exactly the two time-ordered terms. Restoring the spatial integral proves the [scalar Feynman propagator pole prescription](../../../../../../scalar-feynman-propagator-pole-prescription.md):

$$
\boxed{\Delta_F(x-y)=\lim_{\epsilon\downarrow0}\int\frac{d^4p}{(2\pi)^4}\frac{i\,e^{-ip\cdot(x-y)}}{p^2-m^2+i\epsilon}.}
$$

The prescription in this formula supplies the pole convention left unspecified in the printed display; an unprescribed ordinary real-axis integral would not be well-defined. It is a [distribution](../../../../../../distribution-mathematical-analysis.md) limit after smearing, not an absolutely convergent four-dimensional integral. With this normalization the [derivative jump of a free scalar time-ordered two-point function](../../../../../../derivative-jump-of-a-free-scalar-time-ordered-two-point-function.md) gives $(\Box+m^2)\Delta_F=-i\delta^4(x-y)$, an independent check of both the numerator and the sign.

<a id="4/c/image-feynman-propagator-integration-contours-and-displaced-poles"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-301-feynman-contours.png)

**[Figure 1](#4/c/image-feynman-propagator-integration-contours-and-displaced-poles). Feynman propagator integration contours and displaced poles**. Clockwise and counterclockwise [contour integrals](../../../../../../contour-integral.md) for the [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md).

The pole displacement is exaggerated in this original schematic. The contour orientation and selected pole reproduce the [time ordering](../../../../../../time-ordering.md) of the [Feynman propagator](../../../../../../feynman-propagator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
