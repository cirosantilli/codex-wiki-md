<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Group the nonzero modes into independent pairs $p>0$. For one pair set $\varepsilon=\epsilon(p)=p^2/(2m)+\mu$, and introduce the [Nambu spinor](../../../../nambu-spinor.md) $\Psi_p=(c_p,c_{-p}^\dagger)^{\mathsf T}$. [Normal ordering](../../../../normal-ordering.md) using $c_{-p}c_{-p}^\dagger=1-c_{-p}^\dagger c_{-p}$ gives

$$
H_p=\Psi_p^\dagger\begin{pmatrix}\varepsilon&i\Delta\\-i\Delta&-\varepsilon\end{pmatrix}\Psi_p+\varepsilon.
$$

This exactly contains both [kinetic terms](../../../../kinetic-term.md) and the pairing terms once; there is no additional factor of one half because only $p>0$ is summed.

Insert $\Psi_p=U_p\mathcal A_p$, where $\mathcal A_p=(\alpha_p,\alpha_{-p}^\dagger)^{\mathsf T}$ and $U_p$ is the [Bogoliubov transformation](../../../../bogoliubov-transformation.md) [matrix](../../../../matrix.md). Direct [matrix multiplication](../../../../matrix-multiplication.md) yields

$$
U_p^\dagger h_pU_p=\begin{pmatrix}
\varepsilon\cos2\theta_p-\Delta\sin2\theta_p&i(\varepsilon\sin2\theta_p+\Delta\cos2\theta_p)\\
-i(\varepsilon\sin2\theta_p+\Delta\cos2\theta_p)&-\varepsilon\cos2\theta_p+\Delta\sin2\theta_p
\end{pmatrix}.
$$

Choose the diagonalizing branch

$$
\boxed{\cos2\theta_p=\frac{\varepsilon}{E_p},\qquad \sin2\theta_p=-\frac\Delta{E_p},\qquad E_p=\sqrt{\varepsilon^2+\Delta^2},\quad p>0.}
$$

Then the off-diagonal terms vanish and the upper diagonal entry is $E_p>0$. Extend the angle to negative [momenta](../../../../momentum-split.md) as in part b; the sine relation just written applies to the positive representative of each pair. The [BCS coherence factors](../../../../bcs-coherence-factors.md) can be chosen as

$$
u_p=\sqrt{\frac{E_p+\varepsilon}{2E_p}},\qquad
v_p=-\frac{\Delta}{\sqrt{2E_p(E_p+\varepsilon)}}.
$$

Here $u_p$ denotes $\cos\theta_p$, and $v_p$ denotes $\sin\theta_p$; these expressions are nonsingular because $\mu>0$ and $m>0$. The minus sign of $v_p$ for positive $\Delta$ is fixed by the pairing [phase](../../../../phase-waves.md) in this [Hamiltonian](../../../../hamiltonian.md).

A second use of the [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) gives

$$
H_p=E_p\left(\alpha_p^\dagger\alpha_p-\alpha_{-p}\alpha_{-p}^\dagger\right)+\varepsilon
=E_p\left(\alpha_p^\dagger\alpha_p+\alpha_{-p}^\dagger\alpha_{-p}\right)+\varepsilon-E_p.
$$

The zero-momentum term was never paired and is simply $\mu\alpha_0^\dagger\alpha_0$. Hence

$$
\boxed{H=\sum_pE(p)\alpha_p^\dagger\alpha_p+C,\qquad
C=\sum_{p>0}\bigl[\epsilon(p)-\sqrt{\epsilon(p)^2+\Delta^2}\bigr],}
$$

with

$$
\boxed{E(0)=\mu,\qquad E(p)=\sqrt{\epsilon(p)^2+\Delta^2}\quad(p\ne0).}
$$

The constant is the [ground-state energy](../../../../ground-state-energy.md). At fixed $L$, its ultraviolet tail converges: $\epsilon(p)-E(p)=-\Delta^2/[\epsilon(p)+E(p)]\sim-m\Delta^2/p^2$ in one dimension. Replacing $E(0)$ by $\sqrt{\mu^2+\Delta^2}$ would incorrectly pair a spinless mode with itself.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
