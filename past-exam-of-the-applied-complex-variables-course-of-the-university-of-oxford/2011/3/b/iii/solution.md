<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The constant-coefficient equations and decay imply that only the modes $e^{iax}$ on the positive half-line and $e^{-ibx}$ on the negative half-line can occur; the opposite modes grow. [Continuity](../../../../../continuous-function.md) and the nonzero [derivative](../../../../../derivative.md) jump then imply nonzero amplitudes, so any common decay exponent satisfies $0<\gamma\leq\operatorname{Im}a<\operatorname{Im}b$. In particular $-b$ lies below the plus [holomorphic](../../../../../holomorphic-function-split.md) half-plane, and $a$ lies outside the minus half-plane. This locates the [poles](../../../../../pole.md) needed for the transform calculation, without yet computing the amplitudes.

Rearrange the equation from part (i) as

$$
\frac{k+a}{k+b}Y_+-\frac1{(a+b)(k+b)}
=-\left(\frac{k-b}{k-a}Y_-+\frac1{(a+b)(k-a)}\right).
$$

The left side is [holomorphic](../../../../../holomorphic-function-split.md) in the plus half-plane, and the right side in the minus half-plane. Their equality on the overlap glues them into one [entire function](../../../../../entire-function.md). The assumed decay of $Y_\pm$, together with the rational factors tending to one and the subtracted fractions tending to zero, makes this [entire function](../../../../../entire-function.md) tend to zero at [infinity](../../../../../infinity.md). It is therefore identically zero by [Liouville's theorem](../../../../../liouville-theorem.md). This is the additive splitting step of the [Wiener-Hopf method](../../../../../wiener-hopf-method.md). Solving the two zero identities gives

$$
\boxed{Y_+(k)=\frac1{(a+b)(k+a)},\qquad Y_-(k)=-\frac1{(a+b)(k-b)}.}
$$

Their apparent cancellation formulas extend holomorphically wherever a cancelled factor vanishes; the only actual [poles](../../../../../pole.md) are at $-a$ and $b$.

With the Fourier convention in use, inversion has factor $e^{-ikx}$ and normalization $1/(2\pi)$. For $x>0$, close the [contour](../../../../../complex-integration-contour.md) in the [lower half-plane](../../../../../lower-half-plane.md) clockwise, collecting the [pole](../../../../../pole.md) at $-a$. For $x<0$, close in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) counterclockwise, collecting the [pole](../../../../../pole.md) at $b$. The [residue theorem](../../../../../residue-theorem.md) gives

$$
\boxed{y(x)=\begin{cases}\dfrac{e^{iax}}{i(a+b)},&x>0,\\[6pt]\dfrac{e^{-ibx}}{i(a+b)},&x<0.\end{cases}}
$$

Equivalently, each displayed transform follows immediately by integrating the corresponding decaying exponential on its half-line, so Fourier uniqueness gives the same inversion without a [contour](../../../../../complex-integration-contour.md) estimate. Both values at zero are $1/(i(a+b))$, and the [derivative](../../../../../derivative.md) jump is $(a+b)/(a+b)=1$, directly checking the interface conditions.

The moduli are a nonzero constant times $e^{-\operatorname{Im}a\,x}$ for $x>0$ and $e^{-\operatorname{Im}b\,|x|}$ for $x<0$. Hence the largest common exponential decay rate is

$$
\boxed{\gamma_{\max}=\operatorname{Im}a.}
$$

Strictly, the stated big-$O$ bound is also true for every smaller positive $\gamma$; it does not specify a unique exponent unless the sharp rate is intended. The two transform convergence half-planes are exactly the sharper domains stated in part (ii), and the [poles](../../../../../pole.md) on their boundaries prevent extending either half-line [integral](../../../../../integral-split.md) domain any farther.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the applied complex variables course of the University of Oxford](../../../../split.md)
6. [Applied complex variables course of the University of Oxford](../../../../../applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
