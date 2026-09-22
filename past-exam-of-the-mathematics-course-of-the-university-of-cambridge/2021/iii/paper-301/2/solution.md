<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The interaction-picture Hamiltonian density is $\mathcal H_I=\lambda\phi\Phi^\dagger\Phi$. The first-order [Dyson series](../../../../../dyson-series.md) term cannot connect the four external particles, so the leading contribution is

$$
S^{(2)}
=\frac{(-i\lambda)^2}{2}
\int d^4x\,d^4y\,
\mathcal T\{\phi\Phi^\dagger\Phi(x)\,
\phi\Phi^\dagger\Phi(y)\}.
$$

By the [Wick theorem](../../../../../wick-s-theorem.md), the nonzero terms annihilate the incoming complex particle using the annihilation part of $\Phi$, create the outgoing complex particle using the creation part of $\Phi^\dagger$, annihilate the incoming real particle using the annihilation part of $\phi$, and create the outgoing real particle using its creation part. The remaining $\Phi$ and $\Phi^\dagger$ form an internal [Feynman propagator](../../../../../feynman-propagator.md). Interchanging which vertex absorbs the incoming real scalar gives the two contractions; this factor of two cancels the Dyson factor $1/2$.

There are therefore an $s$-channel internal momentum $p+k$ and a crossed channel internal momentum $p-k'$. With covariantly normalized external states,

$$
\langle p',k'|S|p,k\rangle_{\rm conn}
=i(2\pi)^4\delta^{(4)}(p+k-p'-k')\mathcal M,
$$

where

$$
\boxed{
i\mathcal M=(-i\lambda)^2i
\left[
\frac1{(p+k)^2-M^2+i\epsilon}
+\frac1{(p-k')^2-M^2+i\epsilon}
\right]}.
$$

Equivalently,

$$
\mathcal M=-\lambda^2
\left[
\frac1{s-M^2+i\epsilon}
+\frac1{u-M^2+i\epsilon}
\right],
$$

with $s=(p+k)^2$ and $u=(p-k')^2$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
