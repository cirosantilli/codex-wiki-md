# Paul trap Mathieu parameters

↑ **Parent:** [Paul trap](paul-trap.md)

Specify the convention before quoting a stability parameter. Choose the ideal, rotationally symmetric [electric potential](electric-potential.md)

$$
\Phi(\mathbf r,t)=\frac{U-V\cos\Omega t}{2d^2}(x^2+y^2-2z^2),\qquad m>0,\quad d>0,\quad\Omega>0.
$$

Here $U$ is a static voltage coefficient, $V$ is a peak RF voltage coefficient, $d$ is the length entering this displayed normalization, $m$ is [mass](mass.md), $Q$ is signed [electric charge](electric-charge-split.md), and $\Omega$ is the drive [angular frequency](angular-frequency.md). The coefficient $V$ is neither a peak-to-peak voltage nor an RMS voltage. An apparatus's ring-to-cap voltage requires matching its electrode surfaces to this [electric potential](electric-potential.md); electrode radius alone does not define our $d$. The minus sign fixes the RF phase at $t=0$.

With $\tau=\Omega t/2$, [Newton's second law](newton-s-second-law.md) gives a [Mathieu equation](mathieu-equation.md) for each Cartesian coordinate $u_i$:

$$
\frac{d^2u_i}{d\tau^2}+(a_i-2q_i\cos2\tau)u_i=0,\qquad
(a_y,q_y)=(a_x,q_x),\qquad
(a_z,q_z)=(-2a_x,-2q_x).
$$

Thus a three-dimensional [Paul trap](paul-trap.md) needs simultaneous bounded solutions in all three directions. Changing the sign of $V$ reverses $q_i$ and shifts the RF phase by half a cycle; it does not change the ideal infinite-time stability regions. Rescaling the voltage or length convention changes the numerical parameters. [Floquet theory](floquet-theory.md) determines stability of the full [Mathieu equation](mathieu-equation.md); the small-parameter approximation below does not establish stability for arbitrary $q_i$. Bounded mathematical motion can still hit an electrode if its amplitude exceeds the available space.

## ↑ Ancestors (6)

1. [Paul trap](paul-trap.md)
2. [Ion trap](ion-trap.md)
3. [Atomic measurement methods](atomic-measurement-methods.md)
4. [Atomic physics](atomic-physics-split.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
