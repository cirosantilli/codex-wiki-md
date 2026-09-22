<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the Euclidean [quartic scalar field theory](../../../../../../quartic-interaction.md), expansion of $e^{-S}$ gives the momentum-space rules

- an internal scalar line of momentum $p$ contributes $(p^2+m^2)^{-1}$;
- a four-scalar vertex contributes $-\lambda$ and a momentum-conserving delta function;
- each independent [loop momentum](../../../../../../loop-momentum.md) is integrated with $\int d^4k/(2\pi)^4$;
- each graph is divided by its [Feynman-diagram symmetry factor](../../../../../../feynman-diagram-symmetry-factor.md).

At one loop, the [four-point one-particle-irreducible correlation function](../../../../../../four-point-one-particle-irreducible-correlation-function.md) receives the three bubble diagrams in the $s$, $t$, and $u$ channels. If $P$ is the momentum through one channel, its contribution is

$$
\frac{\lambda_a^2}{2}I(P;m,\Lambda),
\qquad
I(P;m,\Lambda)=\int_{|k|<\Lambda}\frac{d^4k}{(2\pi)^4}
\frac1{(k^2+m^2)((k+P)^2+m^2)}.
$$

Using a [Feynman parameter](../../../../../../feynman-parameter.md), shifting the loop momentum, and writing $\Delta_x=m^2+x(1-x)P^2$ gives, up to terms caused by shifting the boundary of a hard cutoff,

$$
I(P;m,\Lambda)=\frac1{16\pi^2}\int_0^1dx
\left[
\log\frac{\Lambda^2+\Delta_x}{\Delta_x}
+\frac{\Delta_x}{\Lambda^2+\Delta_x}-1
\right].
$$

Thus every channel has the logarithmic ultraviolet divergence

$$
I(P;m,\Lambda)=\frac1{16\pi^2}\log\Lambda^2+O(1).
$$

The complete one-loop vertex is

$$
V_a^{(4)}=-\lambda_a+\frac{\lambda_a^2}{2}
\bigl[I(p_1+p_2;m,\Lambda)+I(p_1+p_3;m,\Lambda)+I(p_1+p_4;m,\Lambda)\bigr]
+O(\lambda_a^3).
$$

Let $I_{m,\mathrm{os}}$ denote the bracket evaluated at the chosen on-shell kinematic point. The [on-shell renormalization scheme](../../../../../../on-shell-renormalization-scheme.md) requires $V_a^{(4)}|_{\mathrm{os}}=-\lambda_{\mathrm{phys}}$, hence the perturbative solution is

$$
\boxed{\lambda_a=\lambda_{\mathrm{phys}}
+\frac{\lambda_{\mathrm{phys}}^2}{2}I_{m,\mathrm{os}}
+O(\lambda_{\mathrm{phys}}^3)}.
$$

The cutoff dependence of $\lambda_a$ is the coupling [counterterm](../../../../../../counterterm.md) needed to hold the measured coupling fixed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
