<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For equal masses with positions $\mathbf r_1,\mathbf r_2$, the two-body [Schrödinger equation](../../../../../schrodinger-equation.md) is

$$
\boxed{i\hbar\frac{\partial\Psi}{\partial t}
=\left[-\frac{\hbar^2}{2m}(\nabla_1^2+\nabla_2^2)
-\frac{Gm^2}{|\mathbf r_1-\mathbf r_2|}\right]\Psi}.
$$

Neglecting wave-packet spreading and overlap, write $|a\rangle_i$ for the packet $\psi_{ai}$. The initial state and its branchwise gravitational evolution are

$$
|\Psi(0)\rangle=\frac1n\sum_{a,b=1}^n|a\rangle_1|b\rangle_2,
\qquad
|\Psi(t)\rangle\simeq\frac1n\sum_{a,b=1}^n
e^{iGm^2t/(\hbar d_{ab})}|a\rangle_1|b\rangle_2,
$$

up to local kinetic phases. The branch dependence of the [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md) is the source of [gravitationally induced entanglement](../../../../../gravitationally-induced-entanglement.md).

Under the approximation stated in the question, only the matching pairs $a=b$ acquire an appreciable common phase

$$
\phi=\frac{Gm^2t}{\hbar d}.
$$

The coefficient matrix of the resulting bipartite state is

$$
C=\frac1n[J+(e^{i\phi}-1)I],
$$

where $J$ is the all-ones matrix. Therefore

$$
\rho_1=CC^\dagger
=\frac1{n^2}\left(
[n+2(\cos\phi-1)]J+2(1-\cos\phi)I
\right).
$$

A [maximally entangled state](../../../../../maximally-entangled-state.md) would require $\rho_1=I/n$. This demands

$$
n+2(\cos\phi-1)=0,
\qquad\text{or}\qquad
\cos\phi=1-\frac n2.
$$

That equation has no solution for $n>4$. Thus the requested large-$n$ conclusion does not follow from the assumptions printed in the paper: within the stated approximation, the system never becomes maximally entangled in the large-$n$ limit. For completeness, maximal entanglement is possible for $n=3$ at $\phi=2\pi/3$ and for $n=4$ at $\phi=\pi$; for $n=2$ it occurs at $\phi=\pi/2$ or $3\pi/2$. The $n=4$ time would be

$$
t=\frac{\pi\hbar d}{Gm^2}=\frac{hd}{2Gm^2}
\simeq9.9\ \mathrm{s},
$$

but it is not a large-$n$ answer.

The system also does not remain entangled for every $t>0$. Whenever $\phi=2\pi k$, the phase matrix again factorizes and the state returns to its initial [product state](../../../../../product-state.md). The revival period is

$$
\boxed{T=\frac{2\pi\hbar d}{Gm^2}=\frac{hd}{Gm^2}\simeq19.7\ \mathrm{s}}.
$$

For $n>2$ it is entangled at all intervening times; for $n=2$ there is the additional product-state revival at $\phi=\pi$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
