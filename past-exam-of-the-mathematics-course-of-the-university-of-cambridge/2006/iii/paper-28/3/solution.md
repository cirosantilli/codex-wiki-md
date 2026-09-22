<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the meromorphic completion

$$
Z(s)=\pi^{-s/2}\Gamma(s/2)\zeta(s).
$$

The [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) is

$$
\boxed{Z(s)=Z(1-s).}
$$

Its entire version is $\xi(s)=\tfrac12s(s-1)Z(s)$ with $\xi(s)=\xi(1-s)$. The completion $Z$ itself has [poles](../../../../../pole.md) at zero and one; it should not be confused with the entire [Riemann xi function](../../../../../riemann-xi-function.md).

We prove the equation by a theta integral. Set

$$
\Theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}\qquad(t>0).
$$

The Gaussian [Fourier transform](../../../../../fourier-transform.md), with kernel $e^{-2\pi i x y}$, is

$$
\int_{\mathbb R}e^{-\pi t x^2}e^{-2\pi i xy}\,dx=t^{-1/2}e^{-\pi y^2/t}.
$$

For example, differentiation in $y$ and [integration by parts](../../../../../integration-by-parts.md) give the differential equation $I'(y)=-(2\pi y/t)I(y)$; the [Gaussian integral](../../../../../gaussian-integral.md) gives $I(0)=t^{-1/2}$. Periodize the Gaussian by summing $e^{-\pi t(x+n)^2}$ over integers $n$. Its $k$th Fourier coefficient is the displayed transform at $k$. Both the periodized function and its [Fourier series](../../../../../fourier-series-split.md) converge absolutely, so evaluation at $x=0$ gives the [Poisson summation formula](../../../../../poisson-summation-formula.md) in this case:

$$
\Theta(t)=t^{-1/2}\Theta(1/t).
$$

For $\operatorname{Re}s>1$, integration term by term in the [Gamma function](../../../../../gamma-function.md) integral gives

$$
Z(s)=\frac12\int_0^\infty(\Theta(t)-1)t^{s/2}\frac{dt}{t}.
$$

Indeed, the two terms for $n$ and $-n$ cancel the factor $1/2$, and substitution $v=\pi n^2t$ gives $\pi^{-s/2}\Gamma(s/2)n^{-s}$. Split at one, and use the transformation above in the integral from zero to one. The elementary contribution is

$$
\frac12\int_0^1(t^{-1/2}-1)t^{s/2}\frac{dt}{t}=\frac1{s-1}-\frac1s.
$$

Substitution $t=1/u$ in the remaining term therefore gives

$$
\boxed{Z(s)=\frac1{s-1}-\frac1s+\frac12\int_1^\infty(\Theta(t)-1)\left(t^{s/2}+t^{(1-s)/2}\right)\frac{dt}{t}.}
$$

The theta tail decays exponentially. The integral is consequently an [entire function](../../../../../entire-function.md) of $s$, with [uniform convergence](../../../../../uniform-convergence.md) and termwise differentiation on compact subsets. The formula continues $Z$ meromorphically to the whole plane. Both its rational part and its integral are unchanged by $s\mapsto1-s$, proving the equation and the entire xi formulation. Using the reflection and duplication identities of the [Gamma function](../../../../../gamma-function.md), one may equivalently write

$$
\boxed{\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s),}
$$

understood as an identity of meromorphic functions, including points where individual factors need continuation.

Now let $N(T)$ count the [Nontrivial zeros of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) $\rho=\beta+i\gamma$ with $0<\gamma\le T$, including [multiplicity](../../../../../multiplicity-mathematics.md). The [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md) is

$$
\boxed{N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}-\frac{T}{2\pi}+O(\log(T+2)).}
$$

For $T$ not a zero ordinate, the more precise usual form is

$$
N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}-\frac{T}{2\pi}+\frac78+S(T)+O(T^{-1}),\qquad S(T)=\frac1\pi\arg\zeta(\tfrac12+iT)=O(\log T).
$$

Here the argument is continued from $\zeta(2)>0$ along the path $2\to2+iT\to\tfrac12+iT$. The first formula remains valid at zero ordinates with the stated endpoint convention. Only its leading asymptotic is needed below.

List the positive ordinates as $\gamma_1\le\gamma_2\le\cdots$, with [multiplicity](../../../../../multiplicity-mathematics.md), consistent with this counting function. Put $b_n=2\pi n/\log n$. For every fixed $\varepsilon\in(0,1)$,

$$
\log((1\pm\varepsilon)b_n)=\log n-\log\log n+O_\varepsilon(1),\qquad
N((1\pm\varepsilon)b_n)\sim(1\pm\varepsilon)n.
$$

For all sufficiently large $n$, the lower count is less than $n$ and the upper count is greater than $n$. Consequently $(1-\varepsilon)b_n<\gamma_n\le(1+\varepsilon)b_n$. Letting $\varepsilon\downarrow0$ proves the [asymptotic inversion of the zeta zero count](../../../../../asymptotic-inversion-of-the-zeta-zero-count.md)

$$
\boxed{\gamma_n\sim\frac{2\pi n}{\log n}.}
$$

This argument works even when several zeros have the same ordinate; “increasing” is interpreted in the standard nondecreasing, multiplicity-counted sense. A count listing only distinct ordinates is a different object and is not determined by this formula alone.

In this notation the [Riemann hypothesis](../../../../../riemann-hypothesis.md) says that every [Nontrivial zero of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) has real part one-half:

$$
\boxed{\rho=\tfrac12+i\gamma\quad\text{for every nontrivial zero}.}
$$

It concerns their horizontal location, not merely the growth of the ordinates, and does not assert that the zeros are simple. The functional equation and [complex conjugation](../../../../../complex-conjugation.md) make the zero set symmetric about both the real axis and the [critical line](../../../../../critical-line.md); the hypothesis puts all the [Nontrivial zeros of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) on that line.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
