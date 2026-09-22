<h1 id="9/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $r>s$, $a>0$. When $0<a\le1/4$, the roots of $\mu^2-\mu+a$ are real and lie strictly between zero and one. When $a>1/4$, they are a complex-conjugate pair of modulus $\sqrt a$. Thus the positive [steady state](../../../../../steady-state.md) is linearly asymptotically stable exactly when $0<a<1$, and unstable when $a>1$. Since $a=2s-2s^2/r$ increases strictly with $r$, the crossing occurs at

$$
\boxed{a=1,\qquad r_c=\frac{2s^2}{2s-1}=\frac{2(\delta+1)^2}{2\delta+1}.}
$$

At the crossing,

$$
\mu_\pm=\frac{1\pm i\sqrt3}{2}=e^{\pm i\pi/3},\qquad \boxed{n_t=A\cos(\pi t/3)+B\sin(\pi t/3).}
$$

Every nonzero real linearized perturbation has period six. This establishes the intended **linear stability threshold and linearized period six**.

**The nonlinear period-six claim in the printed paper does not follow, and is false as a local bifurcating-branch claim for this map.** One can check this directly rather than infer a nonlinear period from the [eigenvalues](../../../../../eigenvalue.md). At $r=r_c$ normalize $N_t=N^*(1+u)$, $N_{t-1}=N^*(1+v)$. The exact planar map is

$$
F(u,v)=\left((1+u)\left[\frac{2s^2}{2s-1+(1+v)^2}-(s-1)\right]-1,\ u\right).
$$

Its cubic [Taylor expansion](../../../../../taylor-expansion.md) is

$$
F(u,v)=\left(u-v-uv+\frac{2-s}{2s}v^2+\frac{2-s}{2s}uv^2+\frac{s-1}{s^2}v^3,\ u\right)+O(\|(u,v)\|^4).
$$

Here is a concrete check of the sixfold return. Put $z=(u,v)^T$, $Q=u^2-uv+v^2$, and

$$
K=\begin{pmatrix}1&-2\\2&-1\end{pmatrix},\qquad K^2=-3I,\qquad \alpha=-\frac{3s^2-3s+1}{s^2},\qquad\beta=-\frac{5s^2-6s+2}{2s^2}.
$$

Composing the displayed cubic expansion six times cancels all quadratic terms and gives

$$
F^6(z)-z=Q(\alpha I+\beta K)z+O(\|z\|^4).
$$

In particular

$$
\boxed{Q(F^6(z))-Q(z)=-\frac{2(3s^2-3s+1)}{s^2}Q(z)^2+O(\|z\|^5).}
$$

The quartic coefficient is strictly negative. Hence, sufficiently near the equilibrium, every nonzero point has smaller $Q$ after six iterations: the critical nonlinear map has no nearby nontrivial period-six orbit, and the equilibrium itself is locally attracting despite its neutral [linearization](../../../../../linearization.md).

One can also rule out a branch of small period-six orbits on either side of the crossing. Normalize about the positive equilibrium at each nearby $r$, and put $\eta=a-1$. The derivative of the sixth power of $\begin{pmatrix}1&-a\\1&0\end{pmatrix}$ at $a=1$ is $3I+K$. Smooth dependence on $r$ therefore gives

$$
F_\eta^6(z)-z=\big[(3\eta+\alpha Q)I+(\eta+\beta Q)K\big]z+o\big((|\eta|+\|z\|^2)\|z\|\big).
$$

The leading matrix has [determinant](../../../../../determinant.md) $(3\eta+\alpha Q)^2+3(\eta+\beta Q)^2$. Both terms could vanish with $Q>0$ only if $\alpha=3\beta$, but

$$
\alpha-3\beta=\frac{(3s-2)^2}{2s^2}>0.
$$

Thus its norm on nonzero $z$ is bounded below by a positive constant times $(|\eta|+\|z\|^2)\|z\|$, and the smaller remainder cannot cancel it. There is no nearby nonzero solution of $F_\eta^6(z)=z$. The [eigenvalues](../../../../../eigenvalue.md) satisfy the nonresonance conditions through order four, their moduli cross outward with increasing $r$, and the cubic radial coefficient is negative. The standard [Neimark–Sacker bifurcation](../../../../../neimark-sacker-bifurcation.md) theorem therefore gives a supercritical invariant closed curve. Its rotation is near the linear resonance $1/6$; it is not a local branch of exact period-six orbits.

Finally, the discrete population map does not preserve nonnegativity for arbitrary large lagged populations: $r/(1+bN_{t-1}^2)-\delta$ can be negative. The positive-equilibrium stability conclusions above are local and do not assume a global positivity property that the formula lacks.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
