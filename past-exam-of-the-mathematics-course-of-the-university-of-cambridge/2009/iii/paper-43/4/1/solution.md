<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Assume short-range ferromagnetic exchange $J>0$ and zero external field. In the one-dimensional [Ising model](../../../../../../ising-model.md), a [domain wall](../../../../../../domain-wall.md) costs only $2J$, independent of the lengths of the domains it separates. There are order-$N$ positions for one wall, so its positional entropy offsets any finite energy cost at nonzero temperature as the system grows. Domain walls consequently have a positive density at every $T>0$, destroying a uniform spontaneous [spin magnetization](../../../../../../spin-magnetization.md). Periodic boundaries require an even number of walls, but that constraint does not remove their nonzero thermodynamic-limit density.

The [One-dimensional Ising correlation function](../../../../../../one-dimensional-ising-correlation-function.md) makes this argument explicit. A bond is broken with probability $p_w=e^{-2\beta_{\rm th}J}/(1+e^{-2\beta_{\rm th}J})$, and the infinite-chain correlation is

$$
G(r)=(1-2p_w)^{r/a}=(\tanh\beta_{\rm th}J)^{r/a},\qquad
\xi=\frac{a}{-\log\tanh\beta_{\rm th}J}<\infty\quad(T>0).
$$

The dominant eigenvalue of the [transfer matrix for the one-dimensional Ising model](../../../../../../transfer-matrix-for-the-one-dimensional-ising-model.md) is $2\cosh\beta_{\rm th}J$, so the free energy per spin $-k_BT\log[2\cosh\beta_{\rm th}J]$ is analytic for $T>0$. **There is no finite-temperature transition in one dimension; only the zero-temperature limit orders.**

In two dimensions a reversed cluster is enclosed by a [Peierls contour](../../../../../../peierls-contour.md). A contour of length $\ell$ costs $2J\ell$, while the number of such contours surrounding a fixed site grows at most as a polynomial in $\ell$ times $3^\ell$: after the initial edge, a nonbacktracking square-lattice walk has at most three choices per step. With plus boundary conditions, flipping the interior of a specified contour yields the Boltzmann suppression $e^{-2\beta_{\rm th}J\ell}$. Therefore

$$
\Pr(\sigma_0=-1)\leq\sum_{\ell\geq4}C\ell^2\bigl(3e^{-2\beta_{\rm th}J}\bigr)^\ell.
$$

For sufficiently low temperature this bound is below $1/2$, giving a positive spontaneous magnetization. This is the energy-entropy mechanism of the [Peierls argument](../../../../../../peierls-argument.md).

At sufficiently high temperature, the graphical expansion bounds correlations by sums of connecting paths weighted by $(\tanh\beta_{\rm th}J)^\ell$. The same nonbacktracking count converges geometrically when $3\tanh\beta_{\rm th}J<1$, giving exponential decay and a disordered phase. Since an ordered low-temperature phase and a disordered high-temperature phase both occur, **the two-dimensional model has a finite-temperature phase transition.** The argument establishes its existence and the dimensional distinction, not the exact value of its critical temperature.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [4](../../4.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
