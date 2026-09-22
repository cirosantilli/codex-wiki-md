<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under the given rank hypothesis, the necessary and sufficient local condition is

$$
\boxed{\{a_i,a_j\}=0\quad\text{for every }i,j\text{ on a neighbourhood of the point}.}
$$

Vanishing only at the single point would not suffice: an extension preserves the coordinate [Poisson brackets](../../../../../../poisson-bracket.md) throughout its domain. Necessity follows from the coordinate criterion just proved.

For sufficiency, put $Q_i=a_i$ and $Y_i=X_{Q_i}$. Because the [symplectic form](../../../../../../symplectic-form.md) is a [nondegenerate bilinear form](../../../../../../nondegenerate-bilinear-form.md) at every point, the independent [differentials](../../../../../../differential-of-a-smooth-map.md) $dQ_i$ give independent fields $Y_1,\ldots,Y_n$. They commute, since

$$
[X_{Q_i},X_{Q_j}]=X_{\{Q_j,Q_i\}}=0.
$$

Moreover $dQ_j(Y_i)=\{Q_j,Q_i\}=0$, so they span the tangent spaces of the $n$-dimensional fibres of the [submersion](../../../../../../submersion.md) $Q$. Choose a local section $s(Q)$ transverse to those fibres. Its joint local flow defines coordinates $(Q,t)$ by

$$
\Psi(Q,t)=\varphi_{Y_1}^{t_1}\circ\cdots\circ\varphi_{Y_n}^{t_n}(s(Q)).
$$

The [inverse function theorem](../../../../../../inverse-function-theorem.md) makes $\Psi$ a local [diffeomorphism](../../../../../../diffeomorphism.md), and commuting flows give $\Psi_*\partial_{t_i}=Y_i$.

In these coordinates $\iota_{\partial_{t_i}}\Psi^*\omega_0=dQ_i$. Each flow preserves the [symplectic form](../../../../../../symplectic-form.md), by [Cartan's magic formula](../../../../../../cartan-s-magic-formula.md). Thus its coefficients are independent of $t$, and

$$
\Psi^*\omega_0=\sum_i dt_i\wedge dQ_i+\beta(Q),
$$

where $\beta=s^*\omega_0$ is a closed [differential two-form](../../../../../../2-form.md) on the base. On a small ball, the [Poincaré lemma](../../../../../../poincare-lemma.md) gives $\beta=d\alpha$, with $\alpha=\sum_i\alpha_i(Q)dQ_i$. Define

$$
P_i=-t_i-\alpha_i(Q).
$$

Then

$$
\sum_i dQ_i\wedge dP_i
=\sum_i dt_i\wedge dQ_i+d\alpha
=\Psi^*\omega_0.
$$

Consequently the original coordinates are extended to the required [canonical transformation](../../../../../../canonical-transformation.md) $(Q,P)$, with the prescribed first half $Q=a$. Its [Jacobian matrix](../../../../../../jacobian-matrix.md) is invertible by construction. This is the [canonical completion of independent commuting functions](../../../../../../canonical-completion-of-independent-commuting-functions.md). For the printed $C^2$ data, the flows and resulting [canonical transformation](../../../../../../canonical-transformation.md) can be taken $C^1$, which is sufficient to preserve the [symplectic form](../../../../../../symplectic-form.md); smooth data give smooth coordinates.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
