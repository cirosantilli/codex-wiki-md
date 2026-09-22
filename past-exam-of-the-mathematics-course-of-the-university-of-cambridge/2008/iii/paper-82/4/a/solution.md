<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Consider a nonreal [phase velocity](../../../../../../phase-velocity.md) $c$, so $U-c$ never vanishes. Substitute $\phi=(U-c)\psi$ into the [Rayleigh equation for inviscid shear flow](../../../../../../rayleigh-equation-for-inviscid-shear-flow.md). Differentiating cancels the two terms involving $U''$, leaving

$$
(U-c)\psi''+2U'\psi'-k^2(U-c)\psi=0,
\qquad
\boxed{\bigl[(U-c)^2\psi'\bigr]'-k^2(U-c)^2\psi=0.}
$$

For $k>0$, the wall condition on normal velocity gives $\phi=0$, hence $\psi=0$, at both walls. Multiply by $\overline\psi$ and use [integration by parts](../../../../../../integration-by-parts.md) to obtain the [weighted identity for Howard's semicircle theorem](../../../../../../weighted-identity-for-howard-s-semicircle-theorem.md):

$$
\int_{-y_0}^{y_0}(U-c)^2W\,dy=0,\qquad
W=|\psi'|^2+k^2|\psi|^2\ge0.
$$

For a nonzero [normal mode](../../../../../../normal-mode.md), $N=\int W\,dy>0$. The imaginary and real parts of this identity give, respectively,

$$
-2c_i\int(U-c_r)W\,dy=0,\qquad
\int[(U-c_r)^2-c_i^2]W\,dy=0.
$$

Since $c_i\ne0$, these imply

$$
\boxed{\int UW\,dy=c_rN,\qquad
\int U^2W\,dy=(c_r^2+c_i^2)N.}
$$

The first equation says that $c_r$ is a positive [weighted mean](../../../../../../weighted-arithmetic-mean.md) of $U$, and consequently $U_{\min}\le c_r\le U_{\max}$. The division by $c_i$ is essential: the weighted-mean assertion concerns nonreal modes. A neutral mode may have a [critical level](../../../../../../critical-level-of-a-shear-flow-wave.md) where $U=c$ and the substitution for $\psi$ is singular.

Pointwise, $(U-U_{\max})(U-U_{\min})\le0$. Integrating against the nonnegative weight $W$ and substituting both identities yields

$$
[c_r^2+c_i^2-(U_{\max}+U_{\min})c_r+U_{\max}U_{\min}]N\le0.
$$

Completing the square proves [Howard's semicircle theorem](../../../../../../howard-s-semicircle-theorem.md):

$$
\boxed{\left(c_r-\frac{U_{\max}+U_{\min}}2\right)^2+c_i^2
\le\left(\frac{U_{\max}-U_{\min}}2\right)^2.}
$$

Thus all nonreal [phase velocities](../../../../../../phase-velocity.md) lie in the closed disk with the real interval $[U_{\min},U_{\max}]$ as diameter. For the convention $e^{ik(x-ct)}$ and $k>0$, exponentially growing [normal modes](../../../../../../normal-mode.md) occupy its upper semicircle, while decaying modes occupy its lower semicircle.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 82](../../../paper-82-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
