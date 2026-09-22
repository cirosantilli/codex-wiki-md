<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In elastic diagonal [factorized scattering](../../../../../factorized-scattering.md), the [Faddeev-Zamolodchikov algebra](../../../../../faddeev-zamolodchikov-algebra.md) describes an exchange of two particle operators. Exchanging the pair twice must restore the original state. This is analytic [unitarity](../../../../../unitary-operator.md):

$$
S_{AA}(\theta)S_{AA}(-\theta)=1,\qquad S_{A\bar A}(\theta)S_{\bar A A}(-\theta)=1.
$$

Keeping the reversed species in this identity avoids an unstated parity assumption. For the particular amplitudes derived below, crossing and analytic [unitarity](../../../../../unitary-operator.md) also imply $S_{\bar A A}=S_{A\bar A}$. [Hermitian analyticity of a two-particle S-matrix](../../../../../hermitian-analyticity-of-a-two-particle-s-matrix.md) states $S_{ab}(\theta)^*=S_{ba}(-\theta^*)$ and, together with analytic [unitarity](../../../../../unitary-operator.md), gives $|S_{ab}(\theta)|=1$ for real [rapidity](../../../../../rapidity.md) differences. [Crossing symmetry](../../../../../crossing-symmetry.md) analytically turns an incoming particle into an outgoing [antiparticle](../../../../../antiparticle.md), relating the two channels by $S_{A\bar A}(\theta)=S_{AA}(i\pi-\theta)$, with the reverse relation obtained by crossing again. The shift $i\pi$ follows from the sign reversal of the two-momentum $p(\theta)=(m\cosh\theta,m\sinh\theta)$.

Put $u=\lambda/2$. The given amplitude is the [unit-modulus hyperbolic scattering block](../../../../../unit-modulus-hyperbolic-scattering-block.md) $S_u(\theta)=\sinh[(\theta+iu)/2]/\sinh[(\theta-iu)/2]$. Its numerator and denominator interchange under $\theta\mapsto-\theta$, proving analytic [unitarity](../../../../../unitary-operator.md). For real $u$ it also obeys [Hermitian analyticity of a two-particle S-matrix](../../../../../hermitian-analyticity-of-a-two-particle-s-matrix.md). Applying [crossing symmetry](../../../../../crossing-symmetry.md) gives

$$
\boxed{S_{A\bar A}(\theta)=\frac{\cosh[(\theta-iu)/2]}{\cosh[(\theta+iu)/2]}.}
$$

This crossed amplitude also has unit modulus on the real axis. Thus both requested channel constraints hold.

The bound-state conclusion needs a coupling range. In the fundamental attractive range $0<u<\pi$, equivalently $0<\lambda<2\pi$, the denominator has a simple [pole](../../../../../pole.md) at $\theta=iu$ inside the [physical rapidity strip](../../../../../physical-rapidity-strip.md). Its [residue](../../../../../residue.md) is

$$
\operatorname*{Res}_{\theta=iu}S_{AA}(\theta)=2i\sin u,
$$

with positive imaginary coefficient. Under the usual one-particle interpretation of this direct-channel [bound-state pole](../../../../../bound-state-pole-of-the-scattering-amplitude.md), it couples two charge-$+1$ particles to a new charge-$+2$ particle $B$. In the center-of-mass frame its constituents have analytically continued [rapidities](../../../../../rapidity.md) $\pm iu/2$, and their total two-momentum is $(2m\cos(u/2),0)$. Thus the [relativistic bound-state mass from a rapidity pole](../../../../../relativistic-bound-state-mass-from-a-rapidity-pole.md) gives

$$
\boxed{Q_B=+2,\qquad m_B=2m\cos\frac u2=2m\cos\frac\lambda4.}
$$

It is positive and less than the two-particle threshold $2m$. Without the coupling qualification the requested deduction is false: at $\lambda=0$ the amplitude is identically one after removing the apparent $0/0$ at the origin. A free massive complex [scalar field](../../../../../scalar-field.md) has this diagonal amplitude, charge-$\pm1$ particles and no isolated charge-$+2$ [bound state](../../../../../bound-state.md). At $u=\pi$ the amplitude similarly becomes constant $-1$ and the apparent boundary pole cancels. Neither endpoint supplies the claimed particle.

For [bound-state fusion of factorized S-matrices](../../../../../bound-state-fusion-of-factorized-s-matrices.md), represent $B$ as the residue of $A(\theta_B+iu/2)A(\theta_B-iu/2)$ at its bound-state separation. Move a third $A(\theta_A)$ through both constituents using the [Faddeev-Zamolodchikov algebra](../../../../../faddeev-zamolodchikov-algebra.md), then take the same residue. The bound-state normalization occurs on both sides and cancels. Consequently [bootstrap fusion](../../../../../bound-state-fusion-of-factorized-s-matrices.md) gives

$$
S_{BA}(\theta)=S_{AA}(\theta+iu/2)S_{AA}(\theta-iu/2)=\boxed{\frac{\sinh(\theta/2+3iu/4)\sinh(\theta/2+iu/4)}{\sinh(\theta/2-iu/4)\sinh(\theta/2-3iu/4)}},
$$

where $\theta=\theta_B-\theta_A$. This has analytic [unitarity](../../../../../unitary-operator.md) as a product of two shifted blocks. Its [poles](../../../../../pole.md) occur at $\theta=iu/2$ and $\theta=3iu/2$, modulo $2\pi i$; numerator zeroes occur at the corresponding negative positions, subject to cancellations at special couplings.

The nearer [pole](../../../../../pole.md), $\theta=iu/2$, has [residue](../../../../../residue.md) $-2i\sin u$. It is a [crossed-channel pole in diagonal factorized scattering](../../../../../crossed-channel-pole-in-diagonal-factorized-scattering.md), not a new direct-channel charge-$+3$ state. Indeed, the exchanged momentum has invariant

$$
t=m_B^2+m^2-2m_Bm\cos\frac u2=m^2,
$$

using $m_B=2m\cos(u/2)$. The exchanged particle is therefore the already present $A$, with the appropriate charge flow at the crossed vertex. Equivalently, [crossing symmetry](../../../../../crossing-symmetry.md) puts a positive-residue direct pole of $S_{B\bar A}$ at $i(\pi-u/2)$, corresponding to $B+\bar A\longrightarrow A$. This distinction avoids assigning an extra mass by applying the direct-channel formula to every [pole](../../../../../pole.md).

The farther [pole](../../../../../pole.md), $\theta=3iu/2$, lies in the [physical rapidity strip](../../../../../physical-rapidity-strip.md) only for $0<u<2\pi/3$, equivalently $0<\lambda<4\pi/3$. Its [residue](../../../../../residue.md) is

$$
2i\sin u\,\frac{\sin(3u/2)}{\sin(u/2)},
$$

which has positive imaginary coefficient in that range. It gives a charge-$+3$ [bound state](../../../../../bound-state.md) $C$. The [relativistic bound-state mass from a rapidity pole](../../../../../relativistic-bound-state-mass-from-a-rapidity-pole.md) now yields

$$
m_C^2=m_B^2+m^2+2m_Bm\cos\frac{3u}{2}=m^2(1+2\cos u)^2.
$$

The positive root in the admitted range is

$$
\boxed{Q_C=+3,\qquad m_C=m(1+2\cos u)=m\frac{\sin(3u/2)}{\sin(u/2)}=m(1+2\cos(\lambda/2)),\quad0<\lambda<\frac{4\pi}{3}.}
$$

This is the [three-particle bound state from equal-mass fusion](../../../../../three-particle-bound-state-from-equal-mass-fusion.md); in its own rest frame the constituent [rapidities](../../../../../rapidity.md) are $iu,0,-iu$. At $u=2\pi/3$ the farther apparent pole cancels because its numerator also vanishes; for $2\pi/3<u<\pi$ it lies outside the [physical rapidity strip](../../../../../physical-rapidity-strip.md) and does not require a new charge-$+3$ particle. Charge-conjugate partners carry charges $-2$ and $-3$ where the corresponding states exist. **Fusion distinguishes an existing crossed-channel particle from a genuinely new direct-channel [bound state](../../../../../bound-state.md), and the latter requires the stated smaller coupling range.**

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
