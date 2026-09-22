<h1 id="3/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The original PDF assumes $u\ge0$ at the beginning of this question; the TeX conversion omits that hypothesis. First replace a smooth nonnegative solution by $v=u+\varepsilon>0$, which solves the same [homogeneous divergence-form elliptic equation](../../../../../../../homogeneous-divergence-form-elliptic-equation.md). For $w=v^{q/2}$, the [chain rule](../../../../../../../chain-rule.md) gives the favorable term

$$
\operatorname{div}(A\nabla w)=\frac q2\left(\frac q2-1\right)v^{q/2-2}A\nabla v\cdot\nabla v\ge0
$$

in the distributional sense. Thus $w$ is a [weak subsolution](../../../../../../../weak-subsolution-of-a-divergence-form-elliptic-equation.md). Testing its subsolution inequality with $\zeta^2w$ yields the same [Caccioppoli inequality](../../../../../../../caccioppoli-inequality.md) as before. More precisely, testing the equation for $v$ with $\zeta^2v^{q-1}$ gives

$$
\int\zeta^2|\nabla v^{q/2}|^2\le\frac{q^2}{(q-1)^2}R^2\int v^q|\nabla\zeta|^2\le4R^2\int v^q|\nabla\zeta|^2.
$$

Indeed the main term is at least $(q-1)\lambda\int\zeta^2v^{q-2}|\nabla v|^2$, and the cross term is bounded by twice $\Lambda$ times the square roots of this weighted gradient integral and $\int v^q|\nabla\zeta|^2$. Let $\varepsilon\downarrow0$ to obtain the stated power [energy estimate](../../../../../../../energy-estimate.md).

Apply the fixed-domain [Sobolev embedding theorem](../../../../../../../sobolev-embedding-theorem.md) to $\zeta u^{q/2}$. The crucial constant stays uniform before taking the $2/q$ power:

$$
\boxed{\|u\|_{L^{q\alpha}(B_{r_1})}\le\left[\frac{D_\ell R}{r_2-r_1}\right]^{2/q}\|u\|_{L^q(B_{r_2})}\quad(q\ge2),}
$$

where $D_\ell\ge1$ is independent of $q$. This is [uniform power gain for elliptic solutions](../../../../../../../uniform-power-gain-for-elliptic-solutions.md). The exponent is $q\alpha$, not the TeX conversion's $q^\alpha$. The PDF's weaker prefactor $C_\ell$ outside the $2/q$ power follows from this stronger estimate, but that weaker form alone cannot be iterated infinitely.

For completeness, the estimate also extends to nonnegative locally $H^1$ [weak solutions](../../../../../../../weak-solution.md) without assuming they are already bounded. For $s\ge0$ define $F_M(s)=s^{q/2}$ up to $M$ and continue it linearly with slope $(q/2)M^{q/2-1}$ above $M$; set $\Psi_M(s)=\int_0^sF_M'(r)^2\,dr$. Both have bounded derivatives for fixed $M$. Direct calculation gives $\Psi_M/F_M'\le F_M$ and $F_M(s)\le(q/2)s^{q/2}$. Test the weak equation with $\zeta^2\Psi_M(u)$, using smooth approximations to these [Sobolev chain rule](../../../../../../../sobolev-chain-rule.md) functions if needed. The resulting weighted energy bound is $\int\zeta^2|\nabla F_M(u)|^2\le4R^2\int F_M(u)^2|\nabla\zeta|^2$. If $u\in L^q(B_{r_2})$, dominated convergence on the right and the [Fatou lemma](../../../../../../../fatou-s-lemma.md) on the Sobolev left give the boxed gain as $M\to\infty$, with the same uniform constant. Starting with $q=2$, this justifies every subsequent iteration step.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
