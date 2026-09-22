# Three-level laser rate equation

↑ **Parent:** [Three-level laser](three-level-laser.md)

Consider an original reduced model with a fixed number $N$ of active emitters. Let $u=N_2/N$ be the upper lasing-state fraction, $1-u=N_1/N$ the ground-state fraction, and $s=n/N$ the number of cavity [photons](photon.md) per emitter. Assume the pump state empties rapidly, so its population can be neglected. Measure time by $x=t/\tau$, where $\tau$ is the upper state's spontaneous lifetime. Let $r=W\tau$ be the effective pump rate, $C>0$ the dimensionless stimulated-coupling coefficient, $K>0$ the photon-loss rate in these units, and $0\leq\beta\leq1$ the fraction of spontaneous decays feeding this optical [normal mode](normal-mode.md). The [rate equations](rate-equation.md) are

$$
\frac{du}{dx}=r(1-u)-u-C(2u-1)s,
\qquad
\frac{ds}{dx}=\bigl[C(2u-1)-K\bigr]s+\beta u.
$$

Each term has a physical role. Pumping transfers emitters out of the ground state; [spontaneous emission](spontaneous-emission.md) removes upper-state population. The net stimulated term includes emission from fraction $u$ and absorption by fraction $1-u$, giving their difference $2u-1$. A stimulated transition removes one stored excitation and creates one cavity [photon](photon.md), or does the reverse. The factor $\beta$ accounts for spontaneous emission into the selected mode without pretending that all [spontaneous emission](spontaneous-emission.md) enters it.

For negligible cavity light, the upper-state equation is linear. A constant pump applied to $u(0)=0$ gives

$$
u(x)=\frac{r}{r+1}\left(1-e^{-(r+1)x}\right),\qquad
u_\infty=\frac{r}{r+1}.
$$

Thus this model first permits [population inversion](population-inversion.md) at $r>1$. Positive [optical gain](optical-gain.md) is still insufficient for an oscillator: the gain must exceed the complete [laser threshold](laser-threshold.md), including photon loss. The small-signal photon growth coefficient changes sign when

$$
C(2u-1)=K,\qquad
u_{\rm th}=\frac{1+K/C}{2},\qquad
\boxed{r_{\rm th}=\frac{C+K}{C-K}\quad(C>K).}
$$

If $C\leq K$, even complete inversion cannot exceed the assumed loss in this model. For chosen $C=100$ and $K=20$, the threshold population is $u_{\rm th}=0.6$ and the pump threshold is $r_{\rm th}=1.5$. At $r=2$, the unsaturated population first reaches $0.6$ at $x=(\log10)/3\simeq0.7675$. These numbers are stipulated examples, not ruby material parameters.

**Table of contents**

- [Laser gain clamping](laser-gain-clamping.md)
- [Stored excitation in a pulsed laser](stored-excitation-in-a-pulsed-laser.md)

## ↑ Ancestors (6)

1. [Three-level laser](three-level-laser.md)
2. [Laser](laser-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2012/paper-1/2/c/solution.md)
- [Ruby laser](ruby-laser.md)
- [Stored excitation in a pulsed laser](stored-excitation-in-a-pulsed-laser.md)
