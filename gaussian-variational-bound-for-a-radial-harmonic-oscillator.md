# Gaussian variational bound for a radial harmonic oscillator

↑ **Parent:** [Quantum harmonic oscillator](quantum-harmonic-oscillator-split.md)

Consider $-y''-(n-1)y'/x+x^2y=\lambda y$ for a positive [integer](integer-split.md) $n$, with regular radial data at zero and square-integrable decay at infinity in the measure $x^{n-1}dx$. Its [Sturm-Liouville form](sturm-liouville-form.md) has $p=w=x^{n-1}$ and $q=x^{n+1}$. For the Gaussian trial $y=e^{ax^2}$, $a<0$, the [Rayleigh quotient](rayleigh-quotient.md) is

$$
\Lambda(a)=(4a^2+1)\frac{\int_0^\infty x^{n+1}e^{2ax^2}dx}{\int_0^\infty x^{n-1}e^{2ax^2}dx}=-n\left(a+\frac1{4a}\right).
$$

The [Gamma function recurrence](gamma-function-recurrence.md) evaluates the ratio, and the minimum is $n$ at $a=-1/2$. It is the exact lowest [eigenvalue](eigenvalue.md): after the endpoint term $[x^ny^2]_0^\infty$ vanishes, [integration by parts](integration-by-parts.md) gives

$$
\int_0^\infty\left[x^{n-1}(y')^2+x^{n+1}y^2\right]dx-n\int_0^\infty x^{n-1}y^2dx=\int_0^\infty x^{n-1}(y'+xy)^2dx\geq0.
$$

Equality gives the displayed positive Gaussian [eigenfunction](eigenfunction.md). For $n=1$, the radial regularity condition is the [Neumann boundary condition](neumann-boundary-condition.md) at zero, not a vanishing value there. Changing the boundary condition changes the lowest [eigenvalue](eigenvalue.md) and whether this trial is admissible.

## ↑ Ancestors (5)

1. [Quantum harmonic oscillator](quantum-harmonic-oscillator-split.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/10/solution.md)
