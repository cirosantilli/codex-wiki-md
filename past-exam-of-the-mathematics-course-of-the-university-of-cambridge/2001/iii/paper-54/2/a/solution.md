<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The spatial mean is conserved: averaging every term in the [partial differential equation](../../../../../../partial-differential-equation-split.md) over the periodic cell gives $\partial_t\langle T\rangle=0$. Adding a constant to $T$ also preserves the equation. We therefore fix the mean, conveniently at zero. This qualification is essential: without it the constant [Fourier mode](../../../../../../fourier-mode.md) contributes an additional neutral direction, so the centre subspace would have five real dimensions rather than four.

On a [Fourier mode](../../../../../../fourier-mode.md) $e^{i(mx+ny)}$, the linearized [linear operator](../../../../../../linear-operator.md) has [eigenvalue](../../../../../../eigenvalue.md)

$$
\lambda_{m,n}=\mu(m^2+n^2)-(m^2+n^2)^2.
$$

On the fixed-mean subspace, the first [eigenvalues](../../../../../../eigenvalue.md) to reach zero are those with $m^2+n^2=1$. At $\mu=1$ these are the modes $e^{\pm ix},e^{\pm iy}$; every other nonconstant [Fourier mode](../../../../../../fourier-mode.md) is strictly damped. The reality condition leaves two complex [amplitudes](../../../../../../wave-amplitude.md), hence a **four-real-dimensional centre manifold on the fixed-mean subspace**. The trivial state loses [linear stability](../../../../../../linear-stability.md) as $\mu$ increases through one.

Use slow time $\tau=\varepsilon^2t$, and write $T=\varepsilon W+\varepsilon^3T_3+\cdots$, where

$$
W=A(\tau)e^{ix}+\overline A(\tau)e^{-ix}+B(\tau)e^{iy}+\overline B(\tau)e^{-iy}.
$$

There is no quadratic nonlinearity, so no forced second-order correction is needed. At order $\varepsilon^3$, with $\mu=1+\varepsilon^2\nu$, projection onto the critical [Fourier modes](../../../../../../fourier-mode.md) gives

$$
W_\tau=-\nu\Delta W+(-\Delta-\Delta^2)T_3+\nabla\cdot(|\nabla W|^2\nabla W).
$$

The correction $T_3$ does not contribute to the critical projection because the linear operator vanishes on those modes. To find the nonlinear [coefficient](../../../../../../coefficient.md) of $e^{ix}$, split the [divergence](../../../../../../divergence.md) term into

$$
\partial_x(W_x^3)+\partial_x(W_y^2W_x)+\partial_y(W_x^2W_y)+\partial_y(W_y^3).
$$

The first term contributes $-3|A|^2A$. In the second, only the zero-$y$ [Fourier coefficient](../../../../../../fourier-coefficient.md) of $W_y^2$ contributes; it is $2|B|^2$, and differentiating $W_x$ once more gives $-2|B|^2A$. The third term has zero $y$-average, and the fourth has no $x$-dependent critical component. Interchanging $x,y$ gives the other [amplitude equation](../../../../../../amplitude-equation.md). Thus the [conserved-mean convection amplitude equations](../../../../../../conserved-mean-convection-amplitude-equations.md) are

$$
\boxed{A_\tau=\nu A-3|A|^2A-2|B|^2A,\qquad B_\tau=\nu B-3|B|^2B-2|A|^2B,\quad\alpha=3,\ \beta=2.}
$$

To establish the selected [planform](../../../../../../planform.md), put $A=re^{i\theta}$, $B=se^{i\psi}$. The [phases](../../../../../../phase-waves.md) are constant and the magnitudes obey

$$
\dot r=r(\nu-3r^2-2s^2),\qquad \dot s=s(\nu-3s^2-2r^2).
$$

For $\nu>0$, the square state has $r=s=\sqrt{\nu/5}$. Its magnitude [Jacobian matrix](../../../../../../jacobian-matrix.md) is $-(2\nu/5)\begin{pmatrix}3&2\\2&3\end{pmatrix}$, with [eigenvalues](../../../../../../eigenvalue.md) $-2\nu$ and $-2\nu/5$. Its two neutral [phases](../../../../../../phase-waves.md) correspond to [translation symmetry](../../../../../../translational-symmetry.md). The pure roll has $r^2=\nu/3,s=0$; an infinitesimal $B$ disturbance grows at rate $\nu-2\nu/3=\nu/3>0$. The other pure roll is equivalent, while the trivial state is unstable for $\nu>0$. Consequently **squares, with $|A|^2=|B|^2=\nu/5$, are the stable small-amplitude planform, modulo translations**. For $\nu<0$ the trivial state is stable.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
