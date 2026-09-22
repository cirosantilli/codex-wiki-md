<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D=\overline U-c$ and $F=\widehat w/D^{1/2}$. For $c_i>0$, $D$ never vanishes, so an [analytic branch of a square root](../../../../../../analytic-branch-of-a-square-root.md) exists along the real flow domain. Take real smooth [velocity](../../../../../../velocity.md) and [buoyancy frequency](../../../../../../buoyancy-frequency.md) coefficients, nonzero $k$ (chosen positive for the growing-wave convention), a nontrivial regular [normal mode](../../../../../../normal-mode.md), and boundary decay strong enough to remove the integration-by-parts term.

Substitution into the [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md) gives the half-power case of the [power-transformed Taylor–Goldstein energy identity](../../../../../../power-transformed-taylor-goldstein-energy-identity.md):

$$
(D F')'-k^2DF-\frac12\overline U''F
+\frac{S}{D}F=0,\qquad
S=N^2-\frac14(\overline U')^2.
$$

For completeness, differentiating $\widehat w=D^{1/2}F$ yields $\widehat w''=D^{1/2}F''+\overline U'D^{-1/2}F'+[\tfrac12\overline U''D^{-1/2}-\tfrac14(\overline U')^2D^{-3/2}]F$, which explains the coefficient $1/4$.

Multiply by $F^*$ and integrate over $z$. The boundary term $[F^*DF']$ is zero for the given homogeneous endpoint conditions, or for sufficiently decaying finite-energy modes at infinity. Therefore

$$
\int\left[D(|F'|^2+k^2|F|^2)+\frac12\overline U''|F|^2
-\frac{S}{D}|F|^2\right]dz=0.
$$

Since $\operatorname{Im}D=-c_i$, $\operatorname{Im}(1/D)=c_i/|D|^2$, and $S,\overline U''$ are real, taking the [imaginary part](../../../../../../imaginary-part.md) and dividing by $-c_i$ gives

$$
\int\left[|F'|^2+k^2|F|^2+\frac{S}{|D|^2}|F|^2\right]dz=0.
$$

The first two terms have strictly positive [integral](../../../../../../integral.md) for a nonzero mode. Thus $S$ cannot be nonnegative everywhere:

$$
\boxed{N^2-\frac14(\overline U')^2<0\quad\text{somewhere}.}
$$

This proves the [Miles–Howard theorem](../../../../../../miles-howard-theorem.md) in contrapositive form. Where $\overline U'\ne0$, the corresponding [gradient Richardson number](../../../../../../gradient-richardson-number.md) must fall below $1/4$ somewhere. Failure of this sufficient-stability criterion does not prove instability. The derivation uses $c_i>0$; it cannot be applied unchanged to a neutral singular critical layer.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
