# Probability concentration of a circular Coulomb eigenstate

↑ **Parent:** [Hydrogen atom](hydrogen-atom.md)

For a nonnegative integer $\ell$, this [Coulomb potential](coulomb-potential-energy.md) [energy eigenstate](energy-eigenstate.md) has principal quantum number $\ell+1$ and maximal magnetic quantum number. Put $b=(\ell+1)a$. Including the spherical [volume element](volume-element.md), its radial [probability density](probability-density.md) is a [gamma distribution](gamma-distribution.md) proportional to $r^{2\ell+2}e^{-2r/b}$; its polar density is proportional to $\sin^{2\ell+1}\theta$, while its azimuth is uniform. Radial and polar variables are independent. Their moments satisfy

$$
\mu=\mathbb E[r]=\frac{2\ell+3}{2}b,\qquad\frac{\operatorname{Var}(r)}{\mu^2}=\frac1{2\ell+3},\qquad\mathbb E[\cos^2\theta]=\frac1{2\ell+3}.
$$

The radial identities follow by successive [integration by parts](integration-by-parts.md); the angular identity follows from $\int_0^\pi\sin^{j+2}\theta\,d\theta=(j+1)\int_0^\pi\sin^j\theta\,d\theta/(j+2)$.

Set $h=(2\ell+3)^{-1/3}$. [Chebyshev's inequality](chebyshev-s-inequality.md) and [Markov's inequality](markov-s-inequality.md) give $\mathbb P(|r/\mu-1|>h)\leq h$ and $\mathbb P(|\cos\theta|>h)\leq h$. By the [union bound](boole-s-inequality.md), outside an event of probability at most $2h$, the point lies at distance $O(\mu h)$ from the equatorial circle of radius $\mu$. The [quantum state](quantum-state.md) therefore concentrates near a classical circular orbit in relative units as $\ell$ grows. The absolute orbit radius and absolute transverse width both grow; this statement does not assert localization in a fixed narrow tube.

## ↑ Ancestors (4)

1. [Hydrogen atom](hydrogen-atom.md)
2. [Mathematical physics](mathematical-physics-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford/2008/a/3/solution.md)
