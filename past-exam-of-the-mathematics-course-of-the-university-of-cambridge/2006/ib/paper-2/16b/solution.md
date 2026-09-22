<h1 id="16b/solution">Solution</h1>

↑ **Parent:** [16B](../16b.md)

For a [bound state](../../../../../bound-state.md) take $b>0$ and set $\psi(r)=e^{-br}v(r)$. Substitution into the radial equation and cancellation of the common exponential give

$$
r v''+(2-2br)v'+(a-2b)v=0.
$$

Seek a [power series](../../../../../power-series.md) $v(r)=\sum_{j\geq0}c_jr^j$ with $c_0\ne0$. Equating coefficients of $r^j$ yields the [polynomial construction of hydrogen S states](../../../../../polynomial-construction-of-hydrogen-s-states.md) recurrence

$$
\boxed{c_{j+1}=\frac{2b(j+1)-a}{(j+1)(j+2)}c_j,\qquad j\geq0.}
$$

For any [integer](../../../../../integer.md) $N\geq1$, choose $b=a/(2N)$. The numerator vanishes at $j=N-1$, while it is nonzero for $j<N-1$, so $v$ is a nonzero [polynomial](../../../../../polynomial-split.md) of degree $N-1$. Therefore $\psi$ is continuous at $r=0$ and decays exponentially as $r\to\infty$. The three-dimensional normalization [integral](../../../../../integral.md) is

$$
4\pi\int_0^\infty r^2|\psi(r)|^2dr.
$$

It is finite near zero because $\psi$ is bounded, and finite at infinity because an exponential dominates every [polynomial](../../../../../polynomial-split.md). Multiplying by its positive reciprocal square root gives a normalizable, nonzero [wavefunction](../../../../../wave-function.md). The recurrence ensures the [differential equation](../../../../../differential-equation-split.md) for $r>0$; at the singular endpoint the regular continuous extension has $2\psi'(0)+a\psi(0)=0$, so the potentially singular coefficient cancels. No nonexistent value of $1/r$ at zero is substituted.

Since $E=-\hbar^2b^2/(2m)$, the choice of $b$ gives

$$
\boxed{E_N=-\frac{\hbar^2a^2}{8mN^2}=-\frac{me^4}{32\pi^2\epsilon_0^2\hbar^2N^2},\qquad N=1,2,\ldots.}
$$

For $N=1$, the normalized example is $\psi(r)=\sqrt{b^3/\pi}\,e^{-br}$. For $N=2$, $v(r)$ is proportional to $1-br$. These illustrate the polynomial-times-exponential [Coulomb bound states](../../../../../coulomb-bound-state.md) produced for every required energy. The radial derivative at the origin is generally nonzero, a Coulomb cusp consistent with the requested [continuity](../../../../../continuous-function.md).

## ↑ Ancestors (10)

1. [16B](../16b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
