<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $C(r)=\langle\boldsymbol u(\boldsymbol x)\cdot\boldsymbol u(\boldsymbol x+\boldsymbol r)\rangle$, with zero mean [velocity](../../../../../../velocity.md), and normalize the [turbulent energy spectrum](../../../../../../turbulent-energy-spectrum.md) by $\int_0^\infty E(k)dk=\langle|\boldsymbol u|^2\rangle/2$. Use the [Fourier transform](../../../../../../fourier-transform.md) pair

$$
C(\boldsymbol r)=\int e^{i\boldsymbol k\cdot\boldsymbol r}\widehat C(\boldsymbol k)d^3k,
\qquad\widehat C(\boldsymbol k)=\frac1{(2\pi)^3}\int e^{-i\boldsymbol k\cdot\boldsymbol r}C(\boldsymbol r)d^3r.
$$

[Isotropic turbulence](../../../../../../isotropic-turbulence.md) makes the transform radial, while the energy normalization gives $E(k)=2\pi k^2\widehat C(k)$. Thus

$$
E(k)=\frac{k^2}{4\pi^2}\int C(r)\frac{\sin(kr)}{kr}d^3r.
$$

Assume, for example, $\int(1+r^4)|C(r)|d^3r<\infty$, sufficient to control the remainder. Expanding the radial kernel gives $\sin(kr)/(kr)=1-k^2r^2/6+O(k^4r^4)$. With the [Saffman integral](../../../../../../saffman-integral.md) $L=\int C(r)d^3r$ and [Loitsyansky integral](../../../../../../loitsyansky-integral.md) $I=-\int r^2C(r)d^3r$, this proves

$$
\boxed{E(k)=\frac{Lk^2}{4\pi^2}+\frac{Ik^4}{24\pi^2}+O(k^6).}
$$

The original PDF defines the two distinct integrals; the TeX aid accidentally repeats the definition of $I$ in place of $L$.

For a growing volume $V$, let $\boldsymbol P_V=\int_V\boldsymbol u\,dV$ be its [momentum](../../../../../../momentum.md) per unit density. [Statistical homogeneity](../../../../../../statistical-homogeneity.md) gives

$$
\langle|\boldsymbol P_V|^2\rangle
=\int C(\boldsymbol r)|V\cap(V-\boldsymbol r)|d^3r.
$$

For volumes whose boundary-to-volume ratio tends to zero and integrable $C$, divide by $|V|$ and use dominated convergence:

$$
\boxed{L=\lim_{|V|\to\infty}\frac{\langle|\boldsymbol P_V|^2\rangle}{|V|}\ge0.}
$$

If the volume contains many weakly dependent eddies with uncompensated random impulses, the [central limit theorem](../../../../../../central-limit-theorem.md) suggests root-mean-square total [momentum](../../../../../../momentum.md) proportional to $|V|^{1/2}$; its [variance](../../../../../../variance-split.md) is extensive and $L$ is nonzero. This is a physical expectation, not a theorem for all turbulent fields: cancellation between cells can eliminate the extensive term.

In particular $L=0$ for an ensemble built from locally momentum-compensated eddies with zero net impulse, or when the complete incompressible [velocity correlation tensor](../../../../../../velocity-correlation-tensor.md) decays rapidly enough to have no longitudinal $r^{-3}$ tail. Merely imposing zero total [momentum](../../../../../../momentum.md) in one finite periodic box is insufficient to prove $L=0$ in an infinite-volume limit: the finite-box constraint fixes one global mode. Rapid decay of the trace $C$ alone is also insufficient; the individual tensor components can retain algebraic tails whose trace cancels.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 87](../../../paper-87-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
