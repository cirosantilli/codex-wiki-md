<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $s=Kx$ and assume $s>0$. The scalar [Poisson data fidelity](../../../../../../poisson-data-fidelity.md) integrand has derivative $1-y/s$. Applying the permitted interchange of differentiation and integration in a direction $z$ gives

$$
\left.\frac d{d\varepsilon}E(x+\varepsilon z)\right|_{\varepsilon=0}=\int_\Sigma\left(1-\frac y{Kx}\right)Kz\,dt=\left\langle z,K^*\left(1-\frac y{Kx}\right)\right\rangle.
$$

Thus the ambient-space [Fréchet derivative](../../../../../../frechet-derivative.md), or its [Hilbert space](../../../../../../hilbert-space-split.md) gradient when the pairing is an inner product, is

$$
\boxed{E'(x)=K^*\left(1-\frac y{Kx}\right).}
$$

The quotient is pointwise, and the [adjoint operator](../../../../../../adjoint-operator.md) transports it back from the data domain to the source domain. The chosen spaces must ensure the integrals and derivative pairing are finite; an output bounded away from zero is a useful sufficient condition.

The printed set of [probability density functions](../../../../../../probability-density-function.md) and positive cone are not vector spaces, so the notation for a bounded linear map between them is understood as a positive [bounded linear operator](../../../../../../continuous-linear-operator.md) on ambient function spaces, restricted to admissible inputs. If unit mass is a constraint, admissible directions satisfy $\int_\Omega z=0$. The displayed gradient is then a representative modulo an additive constant; optimization with that constraint additionally includes its [normal cone](../../../../../../normal-cone.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
