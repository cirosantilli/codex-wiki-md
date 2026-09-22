<h1 id="neumann-compatibility-condition-for-laplace-s-equation">Neumann compatibility condition for Laplace's equation</h1>

↑ **Parent:** [Neumann boundary-value problem](neumann-boundary-value-problem.md)

For a smooth bounded region $\Omega$, prescribing the outward [normal derivative](normal-derivative.md) $\partial_nu=g$ of a [harmonic function](harmonic-function.md) requires

$$
\int_{\partial\Omega}g\,dS=0.
$$

This follows from the [divergence theorem](divergence-theorem.md) applied to the [gradient](gradient.md):

$$
\int_{\partial\Omega}\partial_nu\,dS
=\int_\Omega\nabla\cdot\nabla u\,dV
=\int_\Omega\Delta u\,dV=0.
$$

On the unit [disk](disk-mathematics.md), the condition becomes $\int_0^{2\pi}g(\theta)\,d\theta=0$. If $g=\sum_{n\geq1}(a_n\cos(n\theta)+b_n\sin(n\theta))$ is sufficiently regular with zero mean, its regular [harmonic expansion on a disk](harmonic-expansion-on-a-disk.md) is

$$
u(r,\theta)=C+\sum_{n\geq1}\frac{r^n}{n}(a_n\cos(n\theta)+b_n\sin(n\theta)).
$$

The factor $1/n$ compensates for the radial [derivative](derivative.md). The arbitrary $C$ reflects the [uniqueness of the Neumann problem](uniqueness-of-the-neumann-problem.md) up to an additive constant on a connected region.

## ↑ Ancestors (8)

1. [Neumann boundary-value problem](neumann-boundary-value-problem.md)
2. [Boundary value problem](boundary-value-problem-split.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2017/prelims/mathematics-v-resit/question-6/c/iii/solution.md)
