# Poisson summation formula for a Euclidean lattice

↑ **Parent:** [Poisson summation formula](poisson-summation-formula.md)

Let $\Lambda=B\mathbb Z^d$ be a full-rank [Euclidean lattice](euclidean-lattice.md), with [covolume](covolume.md) $m(\Lambda)=|\det B|$ and [dual lattice](dual-lattice.md) $\Lambda^\vee=B^{-\mathsf T}\mathbb Z^d$. For a [Schwartz function](schwartz-function.md) $f\in\mathcal S(\mathbb R^d)$ use the [Fourier transform](fourier-transform-split.md) convention

$$
\widehat f(y)=\int_{\mathbb R^d}f(x)e^{-2\pi i\langle x,y\rangle}\,dx.
$$

Then the [Poisson summation formula](poisson-summation-formula.md) becomes

$$
\boxed{\sum_{\lambda\in\Lambda}f(\lambda)
=\frac1{m(\Lambda)}\sum_{\mu\in\Lambda^\vee}\widehat f(\mu).}
$$

Both [series](series-mathematics.md) have [absolute convergence](absolute-convergence.md). To see the normalization, apply integer-lattice [Poisson summation](poisson-summation-formula.md) to $g(u)=f(Bu)$. The [change of variables formula](change-of-variables-formula.md) gives $\widehat g(k)=|\det B|^{-1}\widehat f(B^{-\mathsf T}k)$, yielding both the reciprocal [covolume](covolume.md) factor and the [dual lattice](dual-lattice.md) argument. The factor is the physical lattice-point density. In particular, for spacing $h>0$,

$$
\sum_{n\in\mathbb Z}f(hn)=\frac1h\sum_{k\in\mathbb Z}\widehat f(k/h).
$$

For the [Gaussian function](gaussian-function.md) $f(x)=e^{-\pi a\|x\|^2}$ with $a>0$, the product of the one-dimensional [Gaussian Fourier transforms](fourier-transform-of-a-gaussian.md) gives

$$
\sum_{\lambda\in\Lambda}e^{-\pi a\|\lambda\|^2}
=\frac{a^{-d/2}}{m(\Lambda)}\sum_{\mu\in\Lambda^\vee}e^{-\pi\|\mu\|^2/a}.
$$

Here $\|\cdot\|$ is the [Euclidean norm](euclidean-norm.md). As a normalization check, take $\Lambda=\operatorname{diag}(2,3)\mathbb Z^2$. Its [covolume](covolume.md) is $6$, and its [dual lattice](dual-lattice.md) is $\operatorname{diag}(1/2,1/3)\mathbb Z^2$, so

$$
\sum_{m,n\in\mathbb Z}e^{-\pi a(4m^2+9n^2)}
=\frac1{6a}\sum_{p,q\in\mathbb Z}e^{-\pi(p^2/4+q^2/9)/a}.
$$

This also follows by multiplying two [Gaussian Poisson summation identities](gaussian-poisson-summation-identity.md) with parameters $4a$ and $9a$. If one instead uses an angular [Fourier transform](fourier-transform-split.md) kernel $e^{-i\langle x,\omega\rangle}$, the reciprocal [frequencies](frequency.md) are $2\pi\Lambda^\vee$, while the prefactor remains $m(\Lambda)^{-1}$.

## ↑ Ancestors (6)

1. [Poisson summation formula](poisson-summation-formula.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Anisotropic theta functional equation](anisotropic-theta-functional-equation.md)
- [Gaussian theta sum](gaussian-theta-sum.md)
- [Lattice theta functional equation](lattice-theta-functional-equation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-28/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-137/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-137/4/c/solution.md)
- [Poisson summation formula](poisson-summation-formula.md)
