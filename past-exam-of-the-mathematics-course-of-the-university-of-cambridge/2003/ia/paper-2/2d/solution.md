<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

With $h=\delta t>0$, the [central finite difference](../../../../../central-finite-difference.md) converts the decay equation to

$$
\boxed{x_{n+1}+2Khx_n-x_{n-1}=0.}
$$

The continuous [ordinary differential equation](../../../../../ordinary-differential-equation.md) has the [general solution](../../../../../general-solution.md) $x(t)=Ce^{-Kt}$. The discrete [linear recurrence](../../../../../linear-recurrence-relation.md) is second order and requires two initial values, such as $x_0,x_1$. Trying $x_n=\rho^n$ gives the [characteristic equation of a linear recurrence](../../../../../characteristic-equation-of-a-linear-recurrence.md) $\rho^2+2Kh\rho-1=0$. Its roots are

$$
\rho_+=-Kh+\sqrt{1+K^2h^2},\qquad
\rho_-=-Kh-\sqrt{1+K^2h^2},
$$

so

$$
\boxed{x_n=A\rho_+^n+B\rho_-^n,\quad
A=\frac{x_1-\rho_-x_0}{\rho_+-\rho_-},\quad
B=\frac{\rho_+x_0-x_1}{\rho_+-\rho_-}.}
$$

There are no repeated roots, and the same formula extends to negative integer $n$ if required.

To demonstrate the continuum limit, put $a_h=\operatorname{arsinh}(Kh)$. Then $\rho_+=e^{-a_h}$ and $\rho_-=-e^{a_h}$, with $a_h/h\to K$. For $t_n=nh\in[0,T]$,

$$
\rho_+^n=e^{-(a_h/h)t_n}\longrightarrow e^{-Kt_n}
$$

uniformly, since $0\le t_n\le T$. More precisely $a_h/h=K-K^3h^2/6+O(h^4)$, giving an $O(h^2)$ error on a fixed interval. Thus $B=0$, $A=C$ selects the physical discrete mode and corresponds to $x_1=\rho_+x_0$.

The other root is a [parasitic amplification root](../../../../../parasitic-amplification-root.md):

$$
B\rho_-^n=B(-1)^n e^{(a_h/h)t_n}.
$$

For fixed $B\ne0$, even and odd mesh points approach values differing by $2Be^{Kt}$. Equivalently successive mesh values have a nonvanishing alternating jump despite their time separation tending to zero. This mode cannot converge uniformly to a continuous ODE solution; its limiting envelope also grows rather than decays.

For step-dependent initial data the precise result is the [centered two-step discretization of exponential decay](../../../../../centered-two-step-discretization-of-exponential-decay.md) criterion:

$$
\boxed{x_n\to Ce^{-Kt_n}\text{ uniformly on }[0,T]
\quad\Longleftrightarrow\quad A_h\to C\text{ and }B_h\to0.}
$$

Sufficiency follows from the two uniformly bounded exponential envelopes on a fixed interval. Necessity follows from convergence at the adjacent points $0,h$: $x_0\to C$, $x_1-x_0\to0$, and the coefficient formulas force $B_h\to0$, $A_h\to C$. In particular a nonzero but vanishing starting error is not excluded. Starting with the exact value $x_1=Ce^{-Kh}$ gives $B_h=CK^3h^3/12+O(h^4)$ and still converges on each fixed interval. The assertion about “remaining” solutions therefore concerns a fixed nonzero parasitic amplitude, not every nonzero step-dependent amplitude. The method is nevertheless not damping-stable for arbitrarily long times because $|\rho_-|>1$.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
