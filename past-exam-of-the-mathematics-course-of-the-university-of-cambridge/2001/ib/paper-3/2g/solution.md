<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Use [separation of variables](../../../../../separation-of-variables.md) in [Laplace's equation](../../../../../laplace-equation.md): writing $\phi=R(r)\Theta(\theta)$ gives

$$
\frac{r^2R''+rR'}R=-\frac{\Theta''}{\Theta}=n^2.
$$

Single-valuedness requires $2\pi$-periodicity, so the nonconstant angular [Fourier modes](../../../../../fourier-mode.md) have integer $n\ge1$ and are $\cos n\theta,\sin n\theta$. Their radial solutions are $r^n,r^{-n}$. The zero angular mode has radial solutions $1,\log r$. These give the [harmonic Fourier expansions in planar concentric domains](../../../../../harmonic-fourier-expansions-in-planar-concentric-domains.md) used below.

For the [annulus](../../../../../annulus-mathematics.md) with $0<a<b$, constant boundary data suggest a radial [harmonic function](../../../../../harmonic-function.md) $A+B\log r$. Enforcing both boundary values gives

$$
\boxed{\phi(r,\theta)=1+\frac{\log(r/a)}{\log(b/a)}.}
$$

This has the required boundary values and satisfies $(r\phi_r)_r=0$. It is unique: the difference of two continuous solutions is [harmonic](../../../../../harmonic-function.md) in the [annulus](../../../../../annulus-mathematics.md) and zero on both boundary circles, so the [maximum principle for harmonic functions](../../../../../maximum-principle-for-harmonic-functions.md), applied to the difference and its negative, makes it zero.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
