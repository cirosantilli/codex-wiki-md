<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Take $\lambda\ne0$ and use the [complex sine-Gordon theory](../../../../../complex-sine-gordon-theory.md) reduced density $\ell=\mathcal L/M^2$, with physical lengths and times $x/M,t/M$. Physical rest energy is $M\int dx\,\mathcal H_\ell$, and the dimensionless [Noether charge](../../../../../noether-charge.md) is obtained from the reduced action. Put $c=\cos\alpha$, $s=\sin\alpha$, $f(x)=c\operatorname{sech}(cx)/\lambda$, so $\psi=f e^{ist}$. Initially take $0<|\alpha|<\pi/2$, avoiding the singular target-space boundary.

The canonical [Hamiltonian density](../../../../../hamiltonian-density.md) is

$$
\mathcal H_\ell=\frac{|\dot\psi|^2+|\psi_x|^2}{1-\lambda^2|\psi|^2}+|\psi|^2.
$$

Here $|\dot\psi|^2=s^2f^2$, $|\psi_x|^2=c^2f^2\tanh^2(cx)$, and $D=1-c^2\operatorname{sech}^2(cx)$. Since $s^2+c^2\tanh^2(cx)=D$, the kinetic contribution is simply $f^2$. Consequently

$$
\boxed{\mathcal M(\alpha)=2M\int f^2dx=\frac{4M}{\lambda^2}\cos\alpha.}
$$

To fix the charge sign, take the [Noether current](../../../../../noether-current.md) directly from $\delta\psi=i\varepsilon\psi$, $\delta\psi^*=-i\varepsilon\psi^*$:

$$
j^\mu=\frac{i(\psi\partial^\mu\psi^*-\psi^*\partial^\mu\psi)}{1-\lambda^2|\psi|^2},\qquad j^0=\frac{2sf^2}{D}.
$$

Thus positive internal rotation has positive charge in this convention. With $X=cx$ and the supplied integral,

$$
Q=\frac{2sc}{\lambda^2}\int_{-\infty}^{\infty}\frac{dX}{\cosh^2X-c^2},\qquad
\boxed{Q(\alpha)=\frac4{\lambda^2}\left[\operatorname{sgn}(\alpha)\frac\pi2-\alpha\right].}
$$

Reversing the definition of the generator would reverse all charge labels but not any [mass](../../../../../mass.md). The limit $\alpha\to\pi/2$ is the vacuum with zero [mass](../../../../../mass.md) and charge. At $\alpha=0$ the field reaches $|\psi|=1/|\lambda|$ at its center and the current's coordinate expression becomes singular. The [mass](../../../../../mass.md) still has the finite limiting value $4M/\lambda^2$, but

$$
\boxed{\lim_{\alpha\to0^\pm}Q=\pm2\pi/\lambda^2.}
$$

The displayed local density does not assign a unique endpoint charge merely by substituting $\alpha=0$.

**The four collective parameters.** Translation, a [Lorentz boost](../../../../../lorentz-boost.md) of [rapidity](../../../../../rapidity.md) $b$, and the global phase symmetry produce

$$
\boxed{\psi(x,t)=\frac{c}{\lambda}\frac{e^{i\chi+i s\eta}}{\cosh(c\xi)},\quad \xi=\cosh b(x-X_0)-\sinh b\,t,\quad \eta=\cosh b\,t-\sinh b(x-X_0).}
$$

The independent real parameters are $\alpha,b,X_0,\chi$, with $\chi$ periodic modulo $2\pi$. A further time translation is absorbed into these parameters. The energy and momentum are $\mathcal M\cosh b$ and $\mathcal M\sinh b$, while $Q$ is invariant. The internal angle is the [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md) whose [canonical momentum](../../../../../canonical-momentum.md) is this [Noether charge](../../../../../noether-charge.md).

**Semiclassical quantization.** For one rest-frame internal rotation, the period in dimensionless time is $T=2\pi/|s|$. The action around the orbit is

$$
I=\int_0^Tdt\int dx(\pi_\psi\dot\psi+\pi_{\psi^*}\dot\psi^*)=\int_0^Tdt\int dx\frac{2|\dot\psi|^2}{D}=T sQ=2\pi|Q|.
$$

Equivalently this is $S+\mathcal E T$, where $\mathcal E$ is the reduced rest energy. [Bohr-Sommerfeld quantization](../../../../../bohr-sommerfeld-quantization.md) with $\hbar=1$ gives $I=2\pi n$. Because the internal orbit is a cyclic angle, not a one-dimensional oscillator between turning points, there is no half-integer [Maslov index](../../../../../maslov-index.md) shift. Hence

$$
\boxed{Q=\pm n,\quad n=1,2,\ldots,\qquad |\alpha|=\frac\pi2-\frac{\lambda^2n}{4},\qquad \mathcal M_n=\frac{4M}{\lambda^2}\sin\frac{\lambda^2n}{4}.}
$$

On the nonsingular branch $0<n<2\pi/\lambda^2$. The elementary charge-one [mass](../../../../../mass.md) approaches $M$ at weak coupling. For positive $a,b$ with $(a+b)\lambda^2/4\leq\pi/2$, $\sin a'+\sin b'>\sin(a'+b')$, where $a'=a\lambda^2/4$, $b'=b\lambda^2/4$. Thus $\mathcal M_{a+b}<\mathcal M_a+\mathcal M_b$: the charge-$n$ [soliton](../../../../../soliton.md) cannot fragment into smaller like-charge particles. For a general charge-conserving partition, a constituent with $|q_i|\geq n$ already has mass at least $\mathcal M_n$; if every $|q_i|<n$, the decreasing ratio $\mathcal M_q/q$ gives $\sum_i\mathcal M_{|q_i|}\geq(\mathcal M_n/n)\sum_i|q_i|\geq\mathcal M_n$, strictly for nontrivial fragmentation. Thus opposite-charge constituents cannot open a lower-energy decay either. This is charged rather than topological stability, and the semiclassical spectrum is reliable at weak coupling.

**Counting states and the endpoint.** Write $L=2\pi/\lambda^2$. If $L$ is not an integer, the regular branch gives

$$
\boxed{Q=\pm1,\ldots,\pm\lfloor L\rfloor,\qquad \text{number of charge states}=2\lfloor L\rfloor.}
$$

If $L$ is an integer, the local nonsingular calculation gives only $2(L-1)$ regular states. The formal closed-branch list has $2L$ charge labels, but its last two labels are limits of the same singular static solution. Counting them needs a global completion; it cannot be decided from a regular current integral at $\alpha=0$.

In the additional integer-level completion, $\lambda^2=4\pi/k$ at leading semiclassical order and charges are identified modulo integer $k>1$. There are then $k-1$ nonzero charge sectors. For odd $k$, positive and negative labels are distinct; for even $k$, the endpoint labels $\pm k/2$ describe one self-conjugate state. This supplies $2L-1$ states when $k=2L$, rather than $2L$ endpoint labels. This global interpretation, and the distinction between classical and renormalized couplings, are discussed in [Dorey and Hollowood, section 2](https://arxiv.org/pdf/hep-th/9410140). A generic classical $\lambda$ does not automatically define an integer $k$ or specify this quantum completion.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
