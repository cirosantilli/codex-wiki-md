<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a full-rank [Euclidean lattice](../../../../../euclidean-lattice.md) $\Lambda\subset\mathbb R^n$, its [dual lattice](../../../../../dual-lattice.md) is

$$
\Lambda'=\{u\in\mathbb R^n:\langle u,\lambda\rangle\in\mathbb Z\text{ for all }\lambda\in\Lambda\}.
$$

If $\Lambda=B\mathbb Z^n$, then $\Lambda'=B^{-\mathsf T}\mathbb Z^n$, $m(\Lambda)=|\det B|$ and $m(\Lambda')=m(\Lambda)^{-1}$. The [characters of a real torus](../../../../../characters-of-a-real-torus.md) identify the additive [dual lattice](../../../../../dual-lattice.md) with the multiplicative character group by

$$
\boxed{u\longmapsto\chi_u,\qquad\chi_u(x+\Lambda)=e^{2\pi i\langle u,x\rangle}.}
$$

The map is well defined precisely because $u\in\Lambda'$, and is injective. For surjectivity, a continuous [group homomorphism](../../../../../group-homomorphism.md) from the compact torus into $\mathbb C^\times$ has compact image. Its modulus has logarithm a homomorphism into $(\mathbb R,+)$ with compact image, hence is zero, so the image lies in the unit circle. Pull the character back to $\mathbb R^n$. Its continuous real lift under $t\mapsto e^{2\pi it}$, normalized to zero at the origin, is additive: its additive defect is an integer-valued continuous function and vanishes at the origin. A continuous additive function is $\langle u,x\rangle$ for a unique $u$. Triviality on $\Lambda$ says $u\in\Lambda'$, proving surjectivity.

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(u)=\int_{\mathbb R^n}f(x)e^{-2\pi i\langle u,x\rangle}\,dx$, and take $f$ to be a [Schwartz function](../../../../../schwartz-function.md). The [periodization of a Schwartz function](../../../../../periodization-of-a-schwartz-function.md) $P_f(x)=\sum_{\lambda\in\Lambda}f(x+\lambda)$ is smooth and $\Lambda$-periodic. On a fundamental cell $F$, the coefficient of the torus character $\chi_u$ is

$$
\frac1{m(\Lambda)}\int_F P_f(x)e^{-2\pi i\langle u,x\rangle}\,dx
=\frac1{m(\Lambda)}\widehat f(u),\qquad u\in\Lambda'.
$$

The equality follows by translating each cell and using $e^{2\pi i\langle u,\lambda\rangle}=1$. The rapidly convergent [Fourier series](../../../../../fourier-series-split.md) can be evaluated at zero, yielding the [Poisson summation formula for a Euclidean lattice](../../../../../poisson-summation-formula-for-a-euclidean-lattice.md)

$$
\boxed{\sum_{\lambda\in\Lambda}f(\lambda)=\frac1{m(\Lambda)}\sum_{u\in\Lambda'}\widehat f(u).}
$$

This argument keeps track of the covolume factor rather than tacitly assuming a unit-volume lattice.

For $\tau$ in the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md), let $g_\tau(x)=e^{\pi i\tau|x|^2}$. Scaling the self-dual real [Gaussian function](../../../../../gaussian-function.md) gives its [Fourier transform](../../../../../fourier-transform.md) at $\tau=it$, $t>0$, and holomorphic continuation in $\tau$ gives the [complex Gaussian Fourier transform](../../../../../complex-gaussian-fourier-transform.md)

$$
\widehat g_\tau(u)=(\tau/i)^{-n/2}\exp\left(-\frac{\pi i|u|^2}{\tau}\right).
$$

The branch is $\exp[-(n/2)\operatorname{Log}(-i\tau)]$ with the logarithm on the right half-plane; it is positive for $\tau=it$. Both the integrals and the lattice sums are locally normally convergent on the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md). Applying the [Poisson summation formula](../../../../../poisson-summation-formula.md) proves the [lattice theta functional equation](../../../../../lattice-theta-functional-equation.md)

$$
\boxed{\Theta_\Lambda(\tau)=(\tau/i)^{-n/2}m(\Lambda)^{-1}\Theta_{\Lambda'}(-1/\tau).}
$$

No integrality or self-duality hypothesis on the lattice is needed.

Put $a=n/2$, $m=m(\Lambda)$ and $\theta_\Lambda(t)=\Theta_\Lambda(it)$. The [Epstein zeta function](../../../../../epstein-zeta-function.md) converges absolutely for $\operatorname{Re}s>a$, and its [Mellin transform](../../../../../mellin-transform.md) representation is

$$
\mathcal E_\Lambda(s)=\pi^{-s}\Gamma(s)E_\Lambda(s)
=\int_0^\infty(\theta_\Lambda(t)-1)t^{s-1}\,dt.
$$

At infinity, $\theta_\Lambda(t)-1$ decays exponentially. Define the entire function

$$
A_\Lambda(s)=\int_1^\infty(\theta_\Lambda(t)-1)t^{s-1}\,dt.
$$

On $(0,1)$, substitute $\theta_\Lambda(t)=m^{-1}t^{-a}\theta_{\Lambda'}(1/t)$ and then $u=1/t$. Isolate the two elementary terms before integrating; this gives the [pole-subtracted theta integral for an Epstein zeta function](../../../../../pole-subtracted-theta-integral-for-an-epstein-zeta-function.md)

$$
\boxed{\mathcal E_\Lambda(s)=A_\Lambda(s)+m^{-1}A_{\Lambda'}(a-s)
+\frac{m^{-1}}{s-a}-\frac1s.}
$$

The formula initially holds for $\operatorname{Re}s>a$ and continues the [completed Epstein zeta function](../../../../../completed-epstein-zeta-function.md) meromorphically to all $\mathbb C$. Apply the same formula to the [dual lattice](../../../../../dual-lattice.md) at $a-s$, using $m(\Lambda')=m^{-1}$ and $\Lambda''=\Lambda$. The entire terms and the two rational terms match, proving

$$
\boxed{\mathcal E_\Lambda(s)=m(\Lambda)^{-1}\mathcal E_{\Lambda'}(n/2-s).}
$$

Finally $E_\Lambda(s)=\pi^s\mathcal E_\Lambda(s)/\Gamma(s)$ also continues meromorphically. Its only pole is a simple one at $s=n/2$, with residue $\pi^{n/2}/[m(\Lambda)\Gamma(n/2)]$; the pole of the completed function at zero is cancelled by $1/\Gamma(s)$, and $E_\Lambda(0)=-1$. The residues and this cancellation make explicit why subtracting the constant theta term was necessary.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 126](../../paper-126-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
