<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $F(T)$ denote the right-hand side of the temperature [partial differential equation](../../../../../../partial-differential-equation-split.md). For a periodic variation $\eta$, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\begin{aligned}
DV[T]\eta&=\left\langle\mu\nabla T\cdot\nabla\eta-\Delta T\,\Delta\eta-|\nabla T|^2\nabla T\cdot\nabla\eta\right\rangle\\
&=\left\langle\left[-\mu\Delta T-\Delta^2T+\nabla\cdot(|\nabla T|^2\nabla T)\right]\eta\right\rangle
=\langle F(T)\eta\rangle.
\end{aligned}
$$

Along the evolution, $T_t=F(T)$, so this is a [gradient flow](../../../../../../gradient-flow.md) with increasing functional:

$$
\boxed{\frac{dV}{dt}=\langle T_t^2\rangle\geq0.}
$$

For $s=|\nabla T|^2$, completing the square gives

$$
\boxed{V[T]=\frac{\mu^2}{4}-\left\langle\frac{(s-\mu)^2}{4}+\frac{(\Delta T)^2}{2}\right\rangle\leq\frac{\mu^2}{4}.}
$$

Thus the [increasing-gradient functional for poorly conducting convection](../../../../../../increasing-gradient-functional-for-poorly-conducting-convection.md) converges to a finite limit along any globally smooth solution, and

$$
\int_0^\infty\langle T_t^2\rangle\,dt=V_\infty-V[T(0)]<\infty.
$$

In particular, there are arbitrarily late times at which $\|T_t\|_{L^2}$ is arbitrarily small. A nonstationary time-periodic solution is impossible: it would have a strictly positive increase of $V$ over a temporal period. More generally, if the orbit is precompact in a topology strong enough for the equation, its limiting states are stationary. With the conserved mean fixed, the displayed square completion bounds $\|\Delta T\|_{L^2}$, and periodic elliptic estimates give an $H^2$ bound; the usual smoothing and compactness for a globally regular parabolic solution support this limiting-state conclusion. The inequalities alone do not prove convergence to one uniquely specified equilibrium, and stationary families related by [translation symmetry](../../../../../../translational-symmetry.md) can remain.

Now take a smooth, nonconstant periodic roll $T_0(x)$. Multiplying its stationary [partial differential equation](../../../../../../partial-differential-equation-split.md) by $T_0$ and using periodic [integration by parts](../../../../../../integration-by-parts.md) yields

$$
\boxed{\mu\langle T_0'^2\rangle-\langle T_0''^2\rangle-\langle T_0'^4\rangle=0.}
$$

The primes here are essential: the first and fourth terms involve $T_0'$, not $T_0$. Write $a=T_0'$, $b=T_0''$, $M_2=\langle a^2\rangle$, $M_4=\langle a^4\rangle$, and $N_2=\langle b^2\rangle$. The orthogonal-roll perturbation has

$$
|\nabla(T_0(x)+\delta T_0(y))|^2=a(x)^2+\delta^2a(y)^2,\qquad
\Delta(T_0(x)+\delta T_0(y))=b(x)+\delta b(y).
$$

The cross term in the squared [Laplacian](../../../../../../laplacian.md) averages to zero since $\langle b\rangle=0$. Independence of the $x,y$ cell integrals then gives the exact [polynomial](../../../../../../polynomial-split.md) difference

$$
\begin{aligned}
V[T_0(x)+\delta T_0(y)]-V[T_0(x)]
&=\frac{\delta^2}{2}(\mu M_2-N_2-M_2^2)-\frac{\delta^4}{4}M_4\\
&=\boxed{\frac{\delta^2}{2}(M_4-M_2^2)-\frac{\delta^4}{4}M_4}.
\end{aligned}
$$

Its leading [coefficient](../../../../../../coefficient.md) is half the [variance](../../../../../../variance-split.md) of $a^2$ over the period. That [variance](../../../../../../variance-split.md) is strictly positive: a nonconstant smooth periodic function has a derivative which vanishes somewhere and is nonzero somewhere, so $a^2$ is not constant. Hence arbitrarily small transverse perturbations increase $V$ above the roll value.

One can turn this energy comparison into [linear instability](../../../../../../linear-instability.md). The linearized evolution at the roll is the self-adjoint operator

$$
L\eta=-\mu\Delta\eta-\Delta^2\eta+\nabla\cdot\left(|\nabla T_0|^2\nabla\eta+2(\nabla T_0\cdot\nabla\eta)\nabla T_0\right).
$$

Choose the fixed-mean perturbation $\eta=T_0(y)-\langle T_0\rangle$. Since $D^2V[T_0](\eta,\eta)=\langle\eta L\eta\rangle=M_4-M_2^2>0$, the [Rayleigh quotient](../../../../../../rayleigh-quotient.md) is positive. The periodic self-adjoint fourth-order operator therefore has a positive [eigenvalue](../../../../../../eigenvalue.md). This proves the [transverse energy instability of nonconstant temperature rolls](../../../../../../transverse-energy-instability-of-nonconstant-temperature-rolls.md): **every nonconstant roll is unstable wherever it exists**.

The existence qualification matters. Constants are also stationary and are stable on the fixed-mean subspace for $0<\mu<1$. Moreover, the periodic [Poincaré inequality](../../../../../../poincare-inequality.md) gives $N_2\geq M_2$, so the roll identity implies $\mu M_2=N_2+M_4>M_2$ for a nonconstant $2\pi$-periodic roll. Such rolls require $\mu>1$ on this specified cell; the conclusion for all positive $\mu$ is conditional on a nonconstant roll being available.

## ↑ Ancestors (11)

1. [B](../b.md)
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
