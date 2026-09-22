<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $R(\alpha)=\alpha^{-\gamma}$, the uniform upstream area satisfies

$$
\boxed{\alpha_1^\gamma=q/\beta}.
$$

The condition $\beta>q^{1-\gamma/2}$ is equivalent to $\alpha_1<\sqrt q$, so this is a [supercritical tube flow](../../../../../../supercritical-tube-flow.md). The downstream prescribed area is subcritical. The steady equation cannot pass smoothly through $\alpha=\sqrt q$: its numerator there is positive under this strict inequality, while its denominator vanishes. A localized, dissipative [elastic jump in a quadratic pressure-area tube](../../../../../../elastic-jump-in-a-quadratic-pressure-area-tube.md) permits the transition.

Neglect gravity and distributed resistance within the short jump. Area conservation gives equal flux on both sides. Multiply the inviscid [momentum](../../../../../../momentum.md) equation by $A$ and use the steady flux to put it in conservative form:

$$
\frac{d}{dx}\left(Au^2+\frac{c_0^2A_0}{3}\alpha^3\right)=0.
$$

The elastic contribution follows from $\rho^{-1}A p_x=c_0^2A_0\alpha^2\alpha_x$. Thus the dimensionless [momentum](../../../../../../momentum.md) flux $q^2/\alpha+\alpha^3/3$ is equal on both sides. If $\alpha_2$ is the post-jump area, subtraction and division by $\alpha_2-\alpha_1\ne0$ give

$$
\boxed{\alpha_2^3+\alpha_1\alpha_2^2+\alpha_1^2\alpha_2-\frac{3q^2}{\alpha_1}=0}.
$$

The momentum-flux function decreases up to $\sqrt q$ and increases thereafter, so the upstream state has exactly one conjugate state with $\alpha_2>\sqrt q$. The physically admissible direction is narrow, fast flow into wide, slow flow. The jump conserves [momentum](../../../../../../momentum.md) and mass, while losing mechanical energy. Indeed the steady [Bernoulli equation](../../../../../../bernoulli-equation.md) away from a jump has $B=c_0^2(q^2/\alpha^2+\alpha^2)/2$. Using the [momentum](../../../../../../momentum.md) relation to eliminate $q^2$ gives $B_1-B_2=c_0^2(\alpha_2^2-\alpha_1^2)(\alpha_2-\alpha_1)^2/(6\alpha_1\alpha_2)>0$. Imposing conservation of $B$ across the jump would therefore give the wrong relation.

Downstream of the jump the steady equation becomes

$$
\frac{G}{c_0^2}\,dx=\frac{\alpha^4-q^2}{\alpha^3-(q/\beta)\alpha^{3-\gamma}}\,d\alpha.
$$

For $\alpha>\sqrt q>\alpha_1$, both numerator and denominator are positive. Thus area grows downstream, and a solution of this type requires $\alpha_3\geq\alpha_2$. Integration from the jump to the exit gives

$$
\boxed{\int_{\alpha_2}^{\alpha_3}\frac{\alpha^4-q^2}{\alpha^3-(q/\beta)\alpha^{3-\gamma}}\,d\alpha=\frac{G}{c_0^2}(L-x_s)}.
$$

The first equation determines $\alpha_1$, the cubic determines its subcritical conjugate $\alpha_2$, and the integral determines $x_s$. The integral must lie between zero and $GL/c_0^2$ for a jump inside the tube. If $\alpha_3<\alpha_2$, or the required downstream length exceeds $L$, these boundary data do not admit the described single-jump branch. For admissible data the uniform upstream section can extend to the selected jump location because it is an exact equilibrium of the steady area equation.

## ↑ Ancestors (11)

1. [B](../b.md)
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
