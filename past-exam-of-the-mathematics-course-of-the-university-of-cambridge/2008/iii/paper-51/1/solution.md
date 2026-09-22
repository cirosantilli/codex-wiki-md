<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use units $\hbar=1$. The fluctuations about a [classical path](../../../../../classical-path.md) satisfy $f(0)=f(T)=0$. Expanding the [action functional](../../../../../action.md) and integrating the term $m\dot q_c\dot f$ by parts gives

$$
S[q_c+f]=S[q_c]+\int_0^T(-m\ddot q_c-V^{\prime}(q_c))f\,dt+\frac12\int_0^T\{m\dot f^2-V^{\prime\prime}(q_c)f^2\}\,dt+O(f^3).
$$

The linear term vanishes by the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) and the endpoint conditions. Integrating the quadratic [kinetic term](../../../../../kinetic-term.md) by parts yields the [Dirichlet fluctuation determinant of a semiclassical propagator](../../../../../dirichlet-fluctuation-determinant-of-a-semiclassical-propagator.md):

$$
\mathcal O_c=-m\frac{d^2}{dt^2}-V^{\prime\prime}(q_c(t)),\qquad K(q_1,q_0;T)\simeq e^{iS[q_c]}\int\mathcal Df\,\exp\left(\frac i2\int f\mathcal O_cf\,dt\right).
$$

A finite time-slicing first turns this into a product of ordinary [Gaussian integrals](../../../../../gaussian-integral.md), whose limit is proportional to $(\det\mathcal O_c)^{-1/2}$. A useful normalization relative to the free operator $\mathcal O_0=-m\,d^2/dt^2$ is

$$
D_c=\left(\frac{m}{2\pi iT}\right)^{1/2}\left(\frac{\det\mathcal O_c}{\det\mathcal O_0}\right)^{-1/2}.
$$

The oscillatory square root is fixed by the short-time limit and the [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md). Away from [zero modes](../../../../../zero-mode.md) this gives the [semiclassical propagator](../../../../../semiclassical-propagator.md); if several [classical paths](../../../../../classical-path.md) contribute, their saddle contributions are summed with their corresponding determinant phases.

**For a general potential the prefactor depends on the endpoints through $q_c$; writing only $D(T)$ suppresses that dependence.** If $V(q)=aq^2/2+bq+c$, the Taylor expansion has no terms beyond quadratic and $V^{\prime\prime}=a$ is independent of $q_c$. The [Gaussian functional integral](../../../../../gaussian-functional-integral.md) is then exact, and its prefactor genuinely depends only on $T$ and the potential parameters. Singular focusing times are understood by continuation of the kernel, rather than by assigning a finite value to a zero-mode determinant.

For the [free-particle propagator](../../../../../free-particle-propagator.md), $q_c(t)=q_0+(q_1-q_0)t/T$ and $S_c=m(q_1-q_0)^2/(2T)$. The free determinant supplies the factor $\sqrt{m/(2\pi iT)}$. Its normalization can also be checked by the momentum-space representation

$$
K_0=\int\frac{dp}{2\pi}\exp\left\{ip(q_1-q_0)-\frac{iTp^2}{2m}\right\}=\sqrt{\frac{m}{2\pi iT}}\exp\left\{\frac{im(q_1-q_0)^2}{2T}\right\},
$$

where completing the square evaluates the [Gaussian integral](../../../../../gaussian-integral.md) and the short-time limit gives the position-space delta function.

For the gravitational potential, the original PDF contains $-mgq$; the TeX aid drops the final $q$. The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) is $\ddot q_c=g$, and its endpoint solution is

$$
q_c(t)=q_0+\left(\frac{q_1-q_0}{T}-\frac{gT}{2}\right)t+\frac12gt^2.
$$

Substitution into the kinetic and potential terms gives

$$
S_c=\frac{m(q_1-q_0)^2}{2T}+\frac{mgT}{2}(q_1+q_0)-\frac{mg^2T^3}{24}.
$$

Since $V^{\prime\prime}=0$, the fluctuation operator is the free one. Thus the [quantum-mechanical propagator in a constant force](../../../../../quantum-mechanical-propagator-in-a-constant-force.md) is exactly

$$
\boxed{K_g(q_1,q_0;T)=\sqrt{\frac{m}{2\pi iT}}\exp\left[i\left\{\frac{m(q_1-q_0)^2}{2T}+\frac{mgT}{2}(q_1+q_0)-\frac{mg^2T^3}{24}\right\}\right].}
$$

The [quantum-mechanical propagator](../../../../../quantum-mechanical-propagator.md) is $\langle q_1|e^{-iHT}|q_0\rangle$, with [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) $H=-\partial_q^2/(2m)+V(q)$. For imaginary time $-i\tau$, insert an orthonormal complete set of [energy eigenstates](../../../../../energy-eigenstate.md) to obtain

$$
\boxed{K(q_1,q_0;-i\tau)=\sum_n e^{-\tau E_n}\psi_n(q_1)\psi_n(q_0)^*,\qquad\tau>0.}
$$

Here $\psi_n(q)=\langle q|n\rangle$. This discrete sum assumes a discrete complete spectrum; continuous spectral components require the corresponding spectral integral. The heat-semigroup expression is well defined for an appropriate [self-adjoint](../../../../../self-adjoint-operator.md) Hamiltonian bounded below. It is this spectral condition, not an unrestricted formal rotation for every conceivable potential, that justifies the imaginary-time kernel.

A path on the circle lifts to a path on the real line ending at $q_1+2\pi w$, where the integer $w$ is its [winding number](../../../../../winding-number.md). The periodic quantum theory sums all these winding sectors with equal weight, giving the [real-time winding representation of a quantum rotor kernel](../../../../../real-time-winding-representation-of-a-quantum-rotor-kernel.md). For imaginary time, put $x=q_1-q_0$ and $y=\tau/m$ in the supplied Gaussian summation identity:

$$
K_{S^1}(q_1,q_0;-i\tau)=\sqrt{\frac{m}{2\pi\tau}}\sum_{w\in\mathbb Z}e^{-m(x+2\pi w)^2/(2\tau)}=\frac1{2\pi}\sum_{n\in\mathbb Z}e^{-\tau n^2/(2m)+inx}.
$$

Comparison with the spectral expansion determines

$$
\boxed{E_n=\frac{n^2}{2m},\qquad\psi_n(q)=\frac{e^{inq}}{\sqrt{2\pi}},\qquad n\in\mathbb Z.}
$$

The normalization uses $0\le q<2\pi$. The ground state is nondegenerate; levels with $n\ne0$ have the degeneracy $n\leftrightarrow-n$. Returning to real time replaces $e^{-\tau E_n}$ by $e^{-iTE_n}$, with the usual limiting prescription. No twisted boundary condition or flux phase is present in the stated image sum.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
