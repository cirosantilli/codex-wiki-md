<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**The [partial differential equation](../../../../../../partial-differential-equation-split.md).** Each term in $K_\alpha$ is a translated [heat kernel](../../../../../../heat-kernel.md) and satisfies $(\partial_t-\partial_x^2-\alpha\partial_x)K_\alpha=0$ for $t>0$. The same holds for $P_\alpha$, either by direct differentiation or because it is $-(2\partial_x+\alpha)H(x+\alpha t,t)$. For $x>0$, $P_\alpha(x,t)$ and its derivatives vanish faster than any power as $t\downarrow0$. Therefore differentiating the boundary [convolution](../../../../../../convolution.md) creates no extra upper-endpoint term. Gaussian domination justifies differentiating both integrals on compact subsets of $x,t>0$, proving the [advection-diffusion equation](../../../../../../advection-diffusion-equation.md).

**The [initial condition](../../../../../../initial-condition.md).** For fixed $x>0$, the first Gaussian in $K_\alpha$ is an [approximate identity](../../../../../../approximate-identity.md) centered at $y=x+\alpha t\to x$. Its integral tends to $u_0(x)$. The reflected Gaussian is exponentially small as $t\downarrow0$, because its center lies outside the half-line. The boundary [convolution](../../../../../../convolution.md) also tends to zero for $x>0$. Thus $u(x,t)\to u_0(x)$.

**The [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md).** The identity

$$
H(-y+\alpha t,t)=e^{\alpha y}H(y+\alpha t,t)
$$

shows that $K_\alpha(0,y,t)=0$, so the initial-data contribution vanishes at zero. The boundary contribution must be evaluated as a limit, not by substituting $x=0$ inside its singular integral. The positive kernel satisfies

$$
\int_0^\infty P_\alpha(x,s)\,ds=e^{-\alpha x}\longrightarrow1,
\qquad
\int_\epsilon^\infty P_\alpha(x,s)\,ds\longrightarrow0
\quad(x\downarrow0)
$$

for every $\epsilon>0$. Hence it is a one-sided [approximate identity](../../../../../../approximate-identity.md) at zero time, and continuity of $g_0$ gives

$$
\boxed{\lim_{x\downarrow0}u(x,t)=g_0(t),\qquad 0<t<T.}
$$

The mass formula follows from the Gaussian Laplace integral, or from the decaying solution of the corresponding constant-coefficient ordinary differential equation. Compatibility $u_0(0)=g_0(0)$ gives the continuous corner value. These arguments also verify the equivalent contour solution in (iii). In the decaying energy class the solution is unique: the difference $v$ of two solutions has zero data and $\frac d{dt}\int_0^\infty v^2dx=-2\int_0^\infty v_x^2dx$ for real solutions, with the analogous modulus identity for complex solutions.

**The unheaded [sine transform](../../../../../../fourier-sine-transform.md) question.** The direct classical [Fourier sine transform](../../../../../../fourier-sine-transform.md) does not close on $u$. If

$$
S(k,t)=\int_0^\infty\sin(kx)u(x,t)\,dx,\qquad
C(k,t)=\int_0^\infty\cos(kx)u(x,t)\,dx,
$$

then [integration by parts](../../../../../../integration-by-parts.md) gives

$$
S_t=-k^2S+kg_0-\alpha kC.
$$

The drift introduces an unknown cosine transform; the usual scalar sine-transform solution of the [heat equation](../../../../../../heat-equation.md) is therefore unavailable directly.

A [Dirichlet gauge transform for constant drift](../../../../../../dirichlet-gauge-transform-for-constant-drift.md) does provide a qualified alternative. Set $v=e^{\alpha x/2+\alpha^2t/4}u$. Then $v_t=v_{xx}$, with $v_0=e^{\alpha x/2}u_0$ and $v(0,t)=e^{\alpha^2t/4}g_0(t)$. If these weighted data have the decay needed for an ordinary [Fourier sine transform](../../../../../../fourier-sine-transform.md), it solves the transformed problem and produces exactly the kernel above. Mere decay of $u_0$ does not ensure this weighted integrability. Thus **not directly by the classical sine transform of $u$; yes after a gauge transformation when the required weighted-transform hypotheses hold**, or after a justified cutoff/limit argument.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
