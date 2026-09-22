<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a decaying [bound state](../../../../bound-state.md) take $\alpha>0$. Substituting $F=fe^{-\alpha r}$ gives $F''=e^{-\alpha r}(f''-2\alpha f'+\alpha^2f)$. The term involving the [energy](../../../../energy-split.md) cancels $\alpha^2f$, leaving the displayed equation with

$$
\boxed{A=\frac{2mK}{\hbar^2}.}
$$

At the lowest power of a series from the [Frobenius method](../../../../frobenius-method.md) $f=\sum_{k\geq0}a_kr^{k+c}$, the [indicial equation](../../../../indicial-equation.md) is $c(c-1)-\ell(\ell+1)=0$. Its roots are $\ell+1$ and $-\ell$. The latter makes $F\sim r^{-\ell}$ and the [radial probability density](../../../../radial-probability-density.md) integral $\int|F|^2dr$ diverge for positive integral $\ell$. Hence $\boxed{c=\ell+1}$.

Equating the remaining coefficients gives

$$
\boxed{a_{k+1}=\frac{2\alpha(k+\ell+1)-A}{(k+1)(k+2\ell+2)}a_k.}
$$

Unless the numerator vanishes, the regular confluent-hypergeometric series contains a large-radius growing branch with the exponential factor $e^{2\alpha r}$. Multiplication by the external $e^{-\alpha r}$ then leaves exponential growth, so it cannot be a [normalizable](../../../../normalizable-wavefunction.md) [bound state](../../../../bound-state.md). Equivalently, the recurrence at large $k$ has $a_{k+1}/a_k\sim2\alpha/k$, indicating that growing exponential scale; regularity at the origin has already fixed the combination of solutions, leaving termination as the way to remove it.

If the polynomial ends at degree index $N\geq0$, its last recurrence numerator gives $A=2\alpha(N+\ell+1)$. With $n=N+\ell+1>\ell$,

$$
\boxed{\alpha=\frac A{2n},\qquad E_n=-\frac{\hbar^2A^2}{8mn^2}=-\frac{mK^2}{2\hbar^2n^2}.}
$$

For the separate angle-independent exponential, [normalization](../../../../normalization.md) includes the full [solid angle](../../../../solid-angle.md):

$$
1=4\pi|N|^2\int_0^\infty r^2e^{-2\alpha r}\,dr
=4\pi|N|^2\frac{2}{(2\alpha)^3}=\frac{\pi|N|^2}{\alpha^3}.
$$

Thus one can choose $\boxed{N=\sqrt{\alpha^3/\pi}}$, up to an overall [phase](../../../../phase-waves.md). Angle independence corresponds to the $\ell=0$ extension, distinct from the positive-$\ell$ family used in the indicial discussion.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
