<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

The [parity operator](../../../../../parity-operator.md) acts by $(P\psi)(x)=\psi(-x)$. For an even potential, differentiating twice and using $V(-x)=V(x)$ proves $HP=PH$ on the parity-invariant domain of the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md). Therefore each [energy eigenspace](../../../../../energy-eigenspace.md) is invariant under $P$. The projectors $(I+P)/2$ and $(I-P)/2$ split it into even and odd subspaces, giving a basis of simultaneous [eigenstates](../../../../../eigenstate.md). An odd state obeys $\psi(0)=-\psi(0)$, hence **$\psi_{\rm odd}(0)=0$**.

The infinite walls impose **$\psi(-a)=\psi(a)=0$**, with the [wavefunction](../../../../../wave-function.md) zero outside. It is continuous at the central [delta potential](../../../../../delta-potential.md). Integrate the stationary [Schrödinger equation](../../../../../schrodinger-equation.md) over $[-\varepsilon,\varepsilon]$; the energy [integral](../../../../../integral.md) tends to zero and the [Dirac delta function](../../../../../dirac-delta-function.md) contributes $\kappa\psi(0)$. This gives

$$
\boxed{\frac{\hbar^2}{2m}\bigl(\psi'(0+)-\psi'(0-)\bigr)=\kappa\psi(0).}
$$

For the given piecewise positive-energy form, $E=\hbar^2\lambda^2/(2m)$. Replacing $x$ by $-x$ swaps the two pieces and leaves their values unchanged, proving $P\psi=\psi$. The value at zero is $A$, and the one-sided [derivatives](../../../../../derivative.md) are $-B\lambda$ and $B\lambda$. The jump condition gives $B=-m\kappa A/(\hbar^2\lambda)$. The wall at $a$ gives $A\cos(\lambda a)-B\sin(\lambda a)=0$, hence

$$
\boxed{\tan(\lambda a)=-\frac{\hbar^2\lambda}{m\kappa}.}
$$

For $\kappa=0$ the undivided wall equation instead gives the usual free even roots. For $\kappa>0$, set $c=m\kappa/\hbar^2>0$ and $k_n=(n+1/2)\pi/a$. In every interval $k_n<\lambda<(n+1)\pi/a$ there is exactly one root: writing $\delta=a(\lambda-k_n)\in(0,\pi/2)$ gives $\cot\delta=\lambda/c$, whose two sides are respectively strictly decreasing and increasing. These are all positive even roots; the quadratic form $\hbar^2\int|\psi'|^2/(2m)+\kappa|\psi(0)|^2$ is nonnegative, so there are no negative [eigenvalues](../../../../../eigenvalue.md). Thus $\lambda_n>k_n$ and **$\eta_n=\hbar^2(\lambda_n^2-k_n^2)/(2m)>0$**.

The printed limit of this absolute energy difference is false. The exact quantization equation gives $\delta_n=\arctan(c/\lambda_n)$, so $\delta_n\to0$ but $\lambda_n\delta_n\to c$. Consequently

$$
\lambda_n^2-k_n^2=\frac{2\lambda_n\delta_n}{a}-\frac{\delta_n^2}{a^2}\longrightarrow\frac{2c}{a},\qquad \boxed{\lim_{n\to\infty}\eta_n=\frac{\kappa}{a}.}
$$

Thus the [high-energy shift from a central delta barrier](../../../../../high-energy-shift-from-a-central-delta-barrier.md) is a finite positive constant, not zero. The corrected vanishing statement is the relative shift $\eta_n/E_n^{(0)}\to0$, or the wave-number difference $\lambda_n-k_n\to0$. Physically, highly energetic particles are weakly affected in relative terms by a fixed point barrier. The free even [wavefunction](../../../../../wave-function.md) normalized in $[-a,a]$ has density $1/a$ at the origin, so the barrier's first-order expectation is $\kappa/a$, matching the exact limit.

Odd states vanish at zero, so the delta term and the [derivative](../../../../../derivative.md) jump both vanish. Their normalized [wavefunctions](../../../../../wave-function.md) and energies are

$$
\boxed{\psi_j(x)=a^{-1/2}\sin(j\pi x/a)\quad(|x|<a),\qquad E_j^{\rm odd}=\frac{\hbar^2\pi^2j^2}{2ma^2},\quad j=1,2,\ldots,}
$$

with zero [wavefunction](../../../../../wave-function.md) outside. They do not depend on $\kappa$. These even and odd sectors describe the [central delta barrier in a symmetric infinite well](../../../../../central-delta-barrier-in-a-symmetric-infinite-well.md).

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
