<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the [second-harmonic feedback in a long-wave convection amplitude equation](../../../../../../second-harmonic-feedback-in-a-long-wave-convection-amplitude-equation.md), at $\mu=2$ the linear steady operator is $L_0=-(1+\partial_x^2)^2$. Its [eigenvalue](../../../../../../eigenvalue.md) on $e^{inx}$ is $-(1-n^2)^2$, so the critical [Fourier modes](../../../../../../fourier-mode.md) are $n=\pm1$. More generally the linear [dispersion relation](../../../../../../dispersion-relation.md) is $\lambda(k)=-1+\mu k^2-k^4$, giving first onset at $\mu=2,k=1$.

At order $\epsilon^2$, the [weakly nonlinear expansion](../../../../../../weakly-nonlinear-expansion.md) gives

$$
L_0\Theta_2=s(\Theta_{1x}^2)_x.
$$

With $\Theta_1=Ae^{ix}+\overline A e^{-ix}$,

$$
\Theta_{1x}^2=-A^2e^{2ix}-\overline A^{\,2}e^{-2ix}+2|A|^2.
$$

The constant part disappears under differentiation. Inverting $L_0$ on the second harmonic, whose [eigenvalue](../../../../../../eigenvalue.md) is $-9$, gives

$$
\boxed{\Theta_2=\frac{2is}{9}A^2e^{2ix}+\mathrm{c.c.}}
$$

up to a critical-harmonic correction absorbed into the definition of $A$. At order $\epsilon^3$,

$$
0=L_0\Theta_3-\mu_2\Theta_{1xx}
-2s(\Theta_{1x}\Theta_{2x})_x+(\Theta_{1x}^3)_x.
$$

The coefficient of $e^{ix}$ in the last three terms is respectively

$$
\mu_2A,\qquad \frac{8s^2}{9}|A|^2A,\qquad -3|A|^2A.
$$

The [Fredholm solvability condition](../../../../../../fredholm-solvability-condition.md) requires their sum to vanish, because $L_0$ annihilates the critical [Fourier mode](../../../../../../fourier-mode.md). For a nonzero amplitude,

$$
\boxed{|A|^2=p(s)\mu_2,\qquad p(s)=\frac9{27-8s^2}.}
$$

This requires $\mu_2/(3-8s^2/9)>0$. The cubic amplitude coefficient is positive for $s^2<27/8$, yielding a small-amplitude branch in a [supercritical bifurcation](../../../../../../supercritical-bifurcation.md); it is negative for $s^2>27/8$, yielding a [subcritical bifurcation](../../../../../../subcritical-bifurcation.md) branch in this leading approximation. At **$s^2=27/8$**, the cubic coefficient vanishes and the quoted relation is singular: higher-order nonlinear terms and a different detuning balance are needed. One must not assert a finite $p$ there.

If a term $\epsilon\mu_1$ were included in $\mu$, order $\epsilon^2$ would also contain $-\mu_1\Theta_{1xx}=\mu_1\Theta_1$. The quadratic nonlinearity produces only the zeroth and second harmonics, with the zeroth differentiated away, so it cannot balance a first-harmonic contribution at that order. Solvability would give $\mu_1A=0$. Hence **a nontrivial critical-mode expansion forces $\mu_1=0$** and first balances detuning against cubic amplitude effects at order $\epsilon^3$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
