<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the canonically normalized Abelian coupling $g_1=-\sqrt{5/3}\,g'$, with $g_2=g$ and $g_3=g_s$, and write $\alpha_i=g_i^2/(4\pi)$. The sign in $g_1$ is a generator convention; its square is what enters running and matching. Let $\alpha_5=g_5^2/(4\pi)$ and $L_X=\log(M_X^2/\mu^2)$. To leading order,

$$
\frac{d}{d\log\mu^2}\frac1{\alpha_i}=\frac{b_i}{4\pi},\qquad\frac1{\alpha_i(\mu)}=\frac1{\alpha_5}-\frac{b_i}{4\pi}L_X.
$$

Use exactly the common-flavor coefficients stipulated for this model:

$$
b_3=11-\frac{2n_f}{3},\qquad b_2=\frac{22}{3}-\frac{2n_f}{3},\qquad b_1=-\frac{2n_f}{3}.
$$

The same $n_f$ cancels from their differences. In particular $b_3-b_2=11/3$ and $b_2-b_1=22/3$, so eliminating the unified coupling gives

$$
\frac1{\alpha_2}-\frac1{\alpha_s}=\frac{11}{12\pi}L_X,\qquad\frac1{\alpha_1}-\frac1{\alpha_2}=\frac{22}{12\pi}L_X=2\left(\frac1{\alpha_2}-\frac1{\alpha_s}\right).
$$

At the low reference scale, $e=g\sin\theta_W=g'\cos\theta_W$. With $w=\sin^2\theta_W$ this means

$$
\alpha_2^{-1}=\frac w\alpha,\qquad\alpha_1^{-1}=\frac{3(1-w)}{5\alpha}.
$$

The last difference equation becomes $3(1-w)/(5\alpha)-w/\alpha=2(w/\alpha-1/\alpha_s)$. Solving gives

$$
\boxed{\sin^2\theta_W=\frac16+\frac{5\alpha}{9\alpha_s}.}
$$

Substitute this into the first difference equation to obtain

$$
\boxed{\log\frac{M_X}{\mu}=\frac\pi{11}\left(\frac1\alpha-\frac{8}{3\alpha_s}\right),\qquad M_X=\mu\exp\!\left[\frac\pi{11}\left(\frac1\alpha-\frac{8}{3\alpha_s}\right)\right].}
$$

All low-scale couplings on the right must be evaluated at the same specified $\mu$. A dimensionful $M_X$ cannot be fixed by dimensionless coupling values without such a reference scale. The result is independent of the common $n_f$ in these differences, although $\alpha_5$ is not. An inferred $M_X>\mu$ requires $\alpha^{-1}>8/(3\alpha_s)$, and perturbative matching requires a positive small $\alpha_5$.

This is the [one-loop SU(5) prediction with common flavor coefficients](../../../../../../one-loop-su-5-prediction-with-common-flavor-coefficients.md). It is the prediction of the supplied simplified coefficient model, not the full matter-and-Higgs calculation for a realistic [SU(5) grand unified theory](../../../../../../su-5-grand-unified-theory.md). Actual [representations](../../../../../../group-representation.md), intermediate thresholds and higher-loop terms change the running and require the corresponding matching calculation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
