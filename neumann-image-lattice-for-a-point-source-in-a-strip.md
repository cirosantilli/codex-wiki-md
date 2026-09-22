# Neumann image lattice for a point source in a strip

↑ **Parent:** [Method of images](method-of-images.md)

For $b>0$, the [Poisson equation](poisson-s-equation.md) $\Delta V=q\delta^{(2)}(x,y)$ in $-b<x<b$ with homogeneous [Neumann boundary conditions](neumann-boundary-condition.md) on both edges admits the even-in-$y$ [method of images](method-of-images.md) solution in the title, where $r_n^2=(x-2nb)^2+y^2$. All image strengths are $q$. Pairing the images at $\pm2nb$ and subtracting their constant logarithms makes each summand $O(n^{-2})$, giving local [uniform convergence](uniform-convergence.md) away from the source. The unrenormalized sum of logarithms does not converge.

Differentiating gives

$$
\partial_yV=\frac{q}{2\pi}\sum_{n\in\mathbb Z}\frac{y}{(x-2nb)^2+y^2}.
$$

The corresponding $x$-derivatives cancel in reflected pairs on $x=\pm b$. For $y>0$, integration across the strip yields a telescoping [arctangent](inverse-tangent.md) sum:

$$
\int_{-b}^b\partial_yV\,dx=\frac{q}{2\pi}\lim_{N\to\infty}2\arctan\frac{(2N+1)b}{y}=\frac q2.
$$

One closed form, up to an additive constant, is $V=(q/4\pi)\log[\cosh(\pi y/b)-\cos(\pi x/b)]$. Its near-source [logarithmic singularity](logarithmic-singularity.md) has coefficient $q/(2\pi)$. Conditions at large $|y|$ or a symmetry class must be specified for a uniqueness claim; side [Neumann boundary conditions](neumann-boundary-condition.md) alone allow additional homogeneous [harmonic functions](harmonic-function.md).

## ↑ Ancestors (3)

1. [Method of images](method-of-images.md)
2. [Mathematics](mathematics-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/3/solution.md)
