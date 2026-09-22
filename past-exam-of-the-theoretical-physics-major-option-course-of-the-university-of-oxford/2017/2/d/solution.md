<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the [unitary discrete Fourier transform](../../../../discrete-fourier-transform-split.md)

$$
a_j=\frac1{\sqrt L}\sum_ke^{ikj}a_k,\qquad k=\frac{2\pi n}{L},\quad n=0,\ldots,L-1.
$$

The transformed [operators](../../../../linear-operator.md) obey $[a_k,a_q^\dagger]=\delta_{kq}$. The hopping terms contribute $2A\cos k$ to the number coefficient. In the pairing sum, the odd sine part cancels between $k$ and $-k$. Thus

$$
H_{\mathrm{LSW}}=\sum_k\left[\alpha_k a_k^\dagger a_k+\frac{\Delta_k}{2}(a_ka_{-k}+a_k^\dagger a_{-k}^\dagger)\right],
$$

where

$$
\alpha_k=S(H_f+2J-J\cos k),\qquad \Delta_k=JS\cos k.
$$

The factor one half in the full [momentum sum](../../../../sum.md) avoids counting an [anomalous pair](../../../../bosonic-bogoliubov-diagonalization.md) twice. For $H_f>0$, $\alpha_k>|\Delta_k|$ for every allowed [momentum](../../../../momentum-split.md). Set

$$
a_k=\cosh\theta_k\,b_k-\sinh\theta_k\,b_{-k}^\dagger,\qquad
\tanh2\theta_k=\frac{\Delta_k}{\alpha_k}.
$$

Real even [angles](../../../../angle.md) ensure consistency between opposite [momenta](../../../../momentum-split.md), and $\cosh^2\theta_k-\sinh^2\theta_k=1$ preserves the [canonical commutation relations](../../../../canonical-commutation-relation.md). The anomalous coefficient becomes $\Delta_k\cosh2\theta_k-\alpha_k\sinh2\theta_k=0$. [Normal ordering](../../../../normal-ordering.md) then gives

$$
\boxed{H_{\mathrm{LSW}}=\sum_k\epsilon(k)b_k^\dagger b_k+\frac12\sum_k[\epsilon(k)-\alpha_k],}
$$

with

$$
\boxed{\epsilon(k)=\sqrt{\alpha_k^2-\Delta_k^2}=S\sqrt{(H_f+2J)[H_f+2J(1-\cos k)]}.}
$$

The [field-polarized planar ferromagnetic spin wave](../../../../field-polarized-planar-ferromagnetic-spin-wave.md) has [energy gap](../../../../energy-gap.md) $\epsilon(0)=S\sqrt{H_f(H_f+2J)}$. The [momenta](../../../../momentum-split.md) run over the whole [Brillouin zone](../../../../brillouin-zone.md) once, including the self-inverse [momenta](../../../../momentum-split.md) $0$ and, for even $L$, $\pi$; these use [single-mode squeezing](../../../../single-mode-squeeze-operator.md) rather than introducing an extra independent partner.

**The zero-field case has a [zero-mode obstruction to bosonic Bogoliubov diagonalization](../../../../zero-mode-obstruction-to-bosonic-bogoliubov-diagonalization.md).** Its nonzero-momentum modes have $\epsilon(k)=2\sqrt2JS|\sin(k/2)|$, but $\alpha_0=\Delta_0=JS$, so no finite [squeezing angle](../../../../bogoliubov-transformation.md) exists for the uniform mode. With $Q_0=(a_0+a_0^\dagger)/\sqrt2$, its [Hamiltonian](../../../../hamiltonian.md) is $JSQ_0^2-JS/2$, not an identically zero oscillator. For example, its [matrix element](../../../../matrix-element.md) between the [vacuum](../../../../fock-vacuum.md) and the two-boson [number state](../../../../fock-state.md) is $JS/\sqrt2$, whereas $\epsilon(0)b_0^\dagger b_0$ would vanish. Consequently the requested oscillator diagonalization is literal for nonzero [field](../../../../magnetic-field-split.md); at zero [field](../../../../magnetic-field-split.md) treat the collective orientation separately or introduce a [field](../../../../magnetic-field-split.md) regulator before taking a limit.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
