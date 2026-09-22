<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**No additional hypothesis on $F$ is needed here for scalar interior $C^{1,\beta}$ regularity.** In the elliptic sense of uniform convexity, the assumptions already give constants $0<\lambda\leq M<\infty$ with $\lambda I\leq D^2F(p)\leq MI$ for all $p$. The following argument gives [interior gradient regularity for uniformly convex autonomous energies](../../../../../../interior-gradient-regularity-for-uniformly-convex-autonomous-energies.md).

The [first variation](../../../../../../first-variation.md) at the minimizer exists because $|DF(p)|\leq C(1+|p|)$, and its weak [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is

$$
\int_\Omega DF(Du)\cdot D\varphi=0\qquad(\varphi\in C_c^\infty(\Omega)).
$$

For a coordinate difference quotient $\delta_hu$, subtract the translated equation and the original equation. The [averaged linearization of a nonlinear divergence-form equation](../../../../../../averaged-linearization-of-a-nonlinear-divergence-form-equation.md) gives

$$
\operatorname{div}(A_hD\delta_hu)=0,\qquad A_h(x)=\int_0^1D^2F\bigl((1-t)Du(x)+tDu(x+he_k)\bigr)\,dt.
$$

These measurable symmetric matrices satisfy $\lambda I\leq A_h\leq MI$ independently of $h$. The [Caccioppoli inequality](../../../../../../caccioppoli-inequality.md) and the standard bound $\|\delta_hu\|_2\leq\|D_ku\|_2$ bound $D\delta_hu$ on every smaller interior set. Quoting the [Sobolev characterization by bounded difference quotients](../../../../../../sobolev-characterization-by-bounded-difference-quotients.md) yields $u\in H^2_{\mathrm{loc}}$.

Now $DF$ is globally [Lipschitz continuous](../../../../../../lipschitz-continuity.md), so the [Sobolev chain rule](../../../../../../sobolev-chain-rule.md) and commutation of distributional derivatives allow differentiation of the weak equation. Each $v_k=D_ku\in H^1_{\mathrm{loc}}$ satisfies

$$
\operatorname{div}(A Dv_k)=0,\qquad A(x)=D^2F(Du(x)),\qquad\lambda I\leq A(x)\leq MI.
$$

The [De Giorgi-Nash-Moser theorem](../../../../../../de-giorgi-nash-moser-theorem.md) states that [weak solutions](../../../../../../weak-solution.md) of this scalar divergence-form equation with bounded measurable [uniformly elliptic](../../../../../../uniformly-elliptic-operator.md) coefficients are locally [Hölder continuous](../../../../../../holder-condition.md). It gives a common $\beta\in(0,1)$ depending only on $n$ and the ellipticity ratio $M/\lambda$, with $D_ku\in C^{0,\beta}_{\mathrm{loc}}$ for every $k$. A Sobolev function whose [weak gradient](../../../../../../weak-gradient.md) is continuous has a $C^1$ representative, as follows by local [mollification](../../../../../../mollification.md) and integration of its [gradient](../../../../../../gradient.md). Hence

$$
\boxed{u\in C^{1,\beta}_{\mathrm{loc}}(\Omega).}
$$

The higher-regularity conclusion comes from differentiating an autonomous scalar equation; it does not rely on boundary regularity or a higher derivative such as $D^3F$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
