<h1 id="16b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the physical [Coulomb bound state](../../../../../../coulomb-bound-state.md) boundary condition: the spherically symmetric wavefunction is regular at the origin and square integrable with measure $4\pi r^2dr$. For $E<0$, set

$$
\boxed{K=\frac{\sqrt{-2mE}}{\hbar}>0.}
$$

At large $r$, the decaying branch behaves exponentially as $e^{-Kr}$. Substituting $\psi=f e^{-Kr}$ into the radial [Schrödinger equation](../../../../../../schrodinger-equation.md) gives

$$
rf''+(2-2Kr)f'+2(\lambda-K)f=0.
$$

The regular solution has a [power series](../../../../../../power-series.md) $f(r)=\sum_{j\geq0}a_jr^j$, with recurrence

$$
\boxed{a_{j+1}=\frac{2[K(j+1)-\lambda]}{(j+1)(j+2)}a_j.}
$$

A nonzero regular solution has $a_0\ne0$. If the series does not terminate, its coefficients eventually have one sign after choosing an overall real phase. For any fixed $0<\delta<1/2$ and sufficiently large $j$, the ratio of consecutive magnitudes is at least $2K(1-\delta)/(j+2)$. The tail therefore grows at least as a positive constant times $e^{2K(1-\delta)r}$ divided by a power of $r$; a finite polynomial of earlier terms cannot cancel it. Multiplication by $e^{-Kr}$ leaves exponential growth, contradicting normalizability.

Thus the series must terminate at degree $N-1$, where $KN=\lambda$ and $N$ is a positive integer. Conversely, termination gives a regular polynomial times $e^{-\lambda r/N}$, which is normalizable. Therefore

$$
\boxed{E_N=-\frac{\hbar^2\lambda^2}{2mN^2}
=-\frac{me^4}{32\pi^2\epsilon_0^2\hbar^2N^2},\qquad N=1,2,\ldots.}
$$

These are the $\ell=0$ members of the hydrogen spectrum. Regularity at the origin is essential: square integrability alone on the punctured radial interval would also admit a singular $1/r$ branch. Such a branch is not a physical eigenfunction of the ordinary three-dimensional Coulomb Hamiltonian; its singularity introduces an inadmissible point-source contribution. In the reduced radial variable $u=r\psi$, the physical condition is $u(0)=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16B](../../16b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
