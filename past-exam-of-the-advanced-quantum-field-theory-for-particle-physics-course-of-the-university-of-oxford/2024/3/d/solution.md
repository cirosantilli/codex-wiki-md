<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the outgoing massless [gauge bosons](../../../../gauge-boson.md), take $k_1^2=k_2^2=0$. Work away from internal poles, with the [Feynman i-epsilon prescription](../../../../feynman-i-epsilon-prescription.md) understood. The [Dirac equations](../../../../dirac-equation.md) and [four-momentum conservation](../../../../four-momentum-conservation.md) give

$$
\begin{aligned}
\bar v\not k_2&=\bar v(\not r_t-m),\\
\not k_2u&=-(\not r_u-m)u.
\end{aligned}
$$

Multiplying by the neighboring [Dirac propagator](../../../../dirac-propagator.md) numerator cancels its denominator. The two fermion-exchange diagrams therefore yield the [matrix commutator](../../../../commutator.md)

$$
\begin{aligned}
k_{2\nu}(\mathcal M_t+\mathcal M_u)^{ab\mu\nu}
&=g^2\bar v\gamma^\mu(t^at^b-t^bt^a)u\\
&=ig^2\epsilon^{abc}J_c^\mu,\qquad
J_c^\lambda=\bar v(p_2)\gamma^\lambda t^cu(p_1).
\end{aligned}
$$

The annihilation [vector current](../../../../vector-current.md) obeys $q_\lambda J_c^\lambda=\bar v(\not p_1+\not p_2)t^cu=0$. Direct contraction of the three-boson tensor gives

$$
k_{2\nu}V^{\lambda\mu\nu}
=s g^{\lambda\mu}-q^\lambda k_2^\mu-k_2^\lambda k_1^\mu.
$$

Thus

$$
k_{2\nu}\mathcal M_s^{ab\mu\nu}
=-ig^2\epsilon^{abc}\left(J_c^\mu-\frac{J_c\cdot k_2}{s}k_1^\mu\right).
$$

The terms proportional to $J_c^\mu$ cancel, leaving the [non-Abelian Ward identity for fermion annihilation](../../../../non-abelian-ward-identity-for-fermion-annihilation.md)

$$
\boxed{k_{2\nu}\mathcal M^{ab\mu\nu}
=ig^2\epsilon^{abc}\frac{J_c\cdot k_2}{s}\,k_1^\mu.}
$$

The open-index tensor is generally nonzero: neither $\epsilon^{abc}$ nor $J_c\cdot k_2$ is constrained to vanish. For a concrete nonzero configuration, take [centre-of-momentum frame](../../../../center-of-momentum-frame.md) kinematics $p_1=(E,0,0,p)$, $p_2=(E,0,0,-p)$, $p=\sqrt{E^2-m^2}$, $k_1=(E,E,0,0)$, $k_2=(E,-E,0,0)$. Standard [Dirac spinors](../../../../dirac-spinor.md) with two-component spin labels $\chi=(1,0)^T$ for $u$ and $\eta=(0,1)^T$ for $v$ give the spinor current $(0,2E,2iE,0)$ and its contraction with $k_2$ is $2E^2$. Choosing both colour spinors $(1,0)^T$ and $(a,b,c)=(1,2,3)$ multiplies this by $1/2$, still nonzero. This explicitly rules out an unconditional tensor identity $k_{2\nu}\mathcal M^{ab\mu\nu}=0$.

For a physical [polarization vector](../../../../polarization-vector.md) $\varepsilon_{1\mu}^*$, however, $k_1\cdot\varepsilon_1^*=0$, and therefore

$$
\boxed{\varepsilon_{1\mu}^*\,k_{2\nu}\mathcal M^{ab\mu\nu}=0.}
$$

This is the required decoupling of a pure-gauge [polarization vector](../../../../polarization-vector.md) on leg 2 when the other leg is physical. Interchanging the legs gives the corresponding identity for leg 1. The role of the three-boson diagram is explicit: it cancels the noncommuting colour-current term left by the two fermion exchanges.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
