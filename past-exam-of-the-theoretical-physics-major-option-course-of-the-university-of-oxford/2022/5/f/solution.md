<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write $d\Pi_p=d^3p/[(2\pi)^3 2\omega_p]$, $p^\mu=(\omega_p,\mathbf p)$ and $\omega_p=\sqrt{\mathbf p^2+m^2}$. The [Fourier expansion](../../../../fourier-series-split.md) in the source is compatible with the oscillator [canonical commutation relations](../../../../canonical-commutation-relation.md)

$$
[a_{\mathbf p},a_{\mathbf q}^\dagger]=(2\pi)^3 2\omega_p\delta^{(3)}(\mathbf p-\mathbf q),\qquad[a,a]=[a^\dagger,a^\dagger]=0.
$$

For the free real [scalar field](../../../../scalar-field.md), $\pi=\dot\phi$ and

$$
P_0=\frac12\int d^3x\,[\pi^2+(\nabla\phi)^2+m^2\phi^2],\qquad P_i=\int d^3x\,\pi\partial_i\phi.
$$

Substitution of the [Fourier expansion](../../../../fourier-series-split.md) produces spatial [Dirac delta functions](../../../../dirac-delta-function.md). Terms with two [annihilation operators](../../../../annihilation-operator.md) or two [creation operators](../../../../creation-operator.md) cancel: in $P_0$ their coefficient is $-\omega_p^2+\mathbf p^2+m^2=0$, and in $P_i$ their integral is odd under $\mathbf p\mapsto-\mathbf p$. The two mixed terms combine, with [normal ordering](../../../../normal-ordering.md) removing the vacuum constant, to give

$$
\boxed{\hat P_\mu=\int d\Pi_p\,p_\mu a_{\mathbf p}^\dagger a_{\mathbf p}.}
$$

In particular, $P_i$ contains the lower component $p_i=-\mathbf p_i$ in this [Minkowski metric](../../../../minkowski-metric.md) convention.

To check commutativity without manipulating a square of a [Dirac delta function](../../../../dirac-delta-function.md), define $N_f=\int d\Pi_p f(p)a_p^\dagger a_p$. The oscillator algebra gives $[N_f,a_q]=-f(q)a_q$ and $[N_f,a_q^\dagger]=f(q)a_q^\dagger$. Thus $[N_f,a_q^\dagger a_q]=0$ and $[N_f,N_g]=0$. Taking $f=p_\mu$, $g=p_\nu$ proves

$$
\boxed{[\hat P_\mu,\hat P_\nu]=0.}
$$

These identities hold on the usual dense domain of finite-particle states, or can first be proved in a finite box and then continued to the continuum.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [5](../../5.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
