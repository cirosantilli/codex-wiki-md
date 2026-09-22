<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\alpha=A/A_0$ and $G=g\sin\theta>0$. The one-dimensional [mass conservation](../../../../../../mass-conservation.md) and axial [momentum](../../../../../../momentum.md) equations consistent with the stated resistance are

$$
A_t+(Au)_x=0,\qquad u_t+uu_x=-\frac1\rho p_x+G-R_0R(\alpha)Au.
$$

In a steady flow, $Au=c_0A_0q$ and $u=c_0q/\alpha$. Since $p_\alpha=\rho c_0^2\alpha$, the [momentum](../../../../../../momentum.md) equation becomes

$$
c_0^2\left(\alpha-\frac{q^2}{\alpha^3}\right)\alpha_x=G-c_0A_0R_0qR(\alpha).
$$

Thus a uniform inlet state continues as a uniform steady solution precisely when

$$
\boxed{qR(\alpha_1)=\beta,\qquad\beta=\frac{G}{c_0A_0R_0}}.
$$

To examine downstream spatial stability of this steady solution, put $\alpha=\alpha_1+z(x)$ and linearize. The numerator vanishes at equilibrium, so

$$
z_x=sz,\qquad s=-\frac{c_0A_0R_0qR'(\alpha_1)}{c_0^2(\alpha_1-q^2/\alpha_1^3)}.
$$

Since $R'<0$, the numerator of $s$ is positive. The [displacement](../../../../../../displacement.md) decays as $x$ increases exactly when $\alpha_1^4<q^2$, or

$$
\boxed{\alpha_1<\sqrt q}.
$$

This proves the [spatial attraction of a uniform downhill tube flow](../../../../../../spatial-attraction-of-a-uniform-downhill-tube-flow.md) appropriate to the steady inlet-value problem.

The [tube wave speed](../../../../../../tube-wave-speed.md) is $c^2=(A/\rho)dp/dA=c_0^2\alpha^2$, while $u=c_0q/\alpha$. The inequality is therefore $u>c$: the inlet lies on the [supercritical tube flow](../../../../../../supercritical-tube-flow.md) branch, with both inviscid [characteristic speeds](../../../../../../characteristic-speed.md) $u\pm c$ directed downstream. A subcritical state has a characteristic carrying downstream boundary information upstream; the critical state makes the steady area equation singular unless its forcing also vanishes.

Spatial attraction must not be confused with temporal stability. The stated hypotheses do not guarantee decay of all time-dependent perturbations. For example, take $R=\alpha^{-2}$ and a uniform supercritical state. The damping coefficient multiplying $u$ is $f=R_0A_0/\alpha$, and for perturbations $e^{i(kx-\omega t)}$ about area $\bar A$ and speed $\bar u$, set $s_t=-i(\omega-k\bar u)$. Linearizing the two evolution equations gives

$$
s_t(s_t+f)+k^2c^2+ik\bar u f=0.
$$

Its small-$k$ branch is $s_t=-ik\bar u+k^2(\bar u^2-c^2)/f+O(k^3)$, which grows when $\bar u>c$. This is a [friction-induced instability of a collapsible-tube flow](../../../../../../friction-induced-instability-of-a-collapsible-tube-flow.md). Consequently the advertised stability is valid as downstream stability of the steady solution; an unrestricted temporal-stability claim would require further assumptions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
