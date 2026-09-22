# Spherical Helmholtz matching to a decaying harmonic exterior

↑ **Parent:** [Spherical Bessel function](spherical-bessel-function.md)

A scalar field solving the [Helmholtz equation](helmholtz-equation.md) inside a sphere of radius $R$ and [Laplace's equation](laplace-equation.md) outside has a regular interior mode $b\,j_\ell(\sqrt{s}\,r)P_\ell(\cos\theta)$ and a decaying exterior mode $a r^{-\ell-1}P_\ell(\cos\theta)$. Continuity of the field and its radial derivative gives, for $x=\sqrt{s}R>0$,

$$
xj_\ell'(x)+(\ell+1)j_\ell(x)=0.
$$

The [Spherical Bessel function](spherical-bessel-function.md) recurrence turns this into $j_{\ell-1}(x)=0$, not $j_\ell(x)=0$. This elimination does not require division by a possibly vanishing boundary value.

For $\ell=0$, $j_0(x)=\sin x/x$ and $j_{-1}(x)=\cos x/x$, so the first positive root is $\pi/2$. For $\ell=1$, the matching condition is $j_0(x)=0$, whose first positive root is $\pi$. The distinction matters when a scalar model permits the monopole sector but a physical multipole model excludes it.

To compare angular sectors, put $u=rj_\ell(\sqrt{s}r)$. Its equation and boundary conditions are $-u''+\ell(\ell+1)u/r^2=su$, $u(0)=0$ and $u'(R)+\ell u(R)/R=0$. Its [Rayleigh quotient](rayleigh-quotient.md) is

$$
s=\frac{\int_0^R[|u'|^2+\ell(\ell+1)|u|^2/r^2]dr+\ell|u(R)|^2/R}{\int_0^R|u|^2dr}.
$$

Both added terms are nonnegative and increase with $\ell$. Thus the lowest scalar eigenvalue is $\pi^2/(4R^2)$ in the $\ell=0$ sector; if only $\ell\geq1$ is admitted, the lowest is $\pi^2/R^2$ in the $\ell=1$ sector. Zeros at $x=0$ caused by the vanishing normalization of $j_\ell$ are not additional eigenvalues.

## ↑ Ancestors (6)

1. [Spherical Bessel function](spherical-bessel-function.md)
2. [Bessel function](bessel-function-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/2/iii/solution.md)
