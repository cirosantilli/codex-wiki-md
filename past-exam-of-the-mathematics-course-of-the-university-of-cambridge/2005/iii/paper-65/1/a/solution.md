<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Substitution into the [Newell–Whitehead–Segel equation](../../../../../../newell-whitehead-segel-equation.md) gives $0=(\mu-q^2-R_0^2)R_0$. Thus a nonzero roll has **$R_0^2=\mu-q^2>0$**; at equality the branch meets the zero solution. The two signs of $R_0$ differ by a constant [phase modulation](../../../../../../phase-modulation.md).

The sign of the transverse [zigzag instability](../../../../../../zigzag-instability.md) must be calculated from the differential operator. Put $D=\partial_X+i\partial_Y^2/2$ and $A=R_0e^{iqX+i\phi(Y)}$. The [chain rule](../../../../../../chain-rule.md) gives

$$
DA=\left[i\left(q-\frac12\phi_Y^2\right)-\frac12\phi_{YY}\right]A.
$$

Consequently the change in the printed functional density is

$$
\Delta V=R_0^2\left\langle q\phi_Y^2-\frac14\phi_Y^4-\frac14\phi_{YY}^2\right\rangle.
$$

For a [Lyapunov functional](../../../../../../lyapunov-functional.md) one integrates this density over the transverse coordinate too, or uses a transverse spatial average, with periodic or decaying boundary conditions. A fast-$x$ average alone leaves a density depending on $Y$ and is not itself a global monotonicity statement. Indeed $D^\dagger=-D$ under these boundary conditions, and the functional derivative of the resulting spatial integral is $\delta V/\delta\overline A=\mu A+D^2A-|A|^2A=A_T$. Hence $dV/dT=2\langle|A_T|^2\rangle\ge0$: stable rolls locally maximize this functional.

With the **plus sign actually printed in $D$**, $q<0$ makes both quadratic contributions to $\Delta V$ negative. These rolls are stable to long-wave transverse [phase modulation](../../../../../../phase-modulation.md). For $q>0$ a sufficiently long-wave displacement increases $V$ and is unstable. At $q=0$ the second-derivative stiffness vanishes, but the fourth-derivative and nonlinear tilt terms still decrease $V$. [Linearization](../../../../../../linearization.md) makes the conclusion explicit:

$$
\phi_T=-q\phi_{YY}-\frac14\phi_{YYYY},\qquad
\boxed{\sigma(k)=qk^2-\frac14k^4.}
$$

Thus for $q>0$ the unstable band is $0<k^2<4q$, with maximum growth at $k^2=2q$; in a finite periodic cell the band must contain an allowed [Fourier mode](../../../../../../fourier-mode.md). Replacing $D$ by $\partial_X-i\partial_Y^2/2$ reverses the sign of the detuning associated with the [zigzag instability](../../../../../../zigzag-instability.md). It would therefore be incorrect to import that opposite sign convention into the printed equation. Transverse stability does not exclude the distinct longitudinal [Eckhaus instability](../../../../../../eckhaus-instability.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
