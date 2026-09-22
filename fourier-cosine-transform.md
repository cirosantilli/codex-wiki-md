# Fourier cosine transform

↑ **Parent:** [Fourier transform](fourier-transform-split.md)

For sufficiently regular decaying data, this half-line transform has inverse $f(x)=(2/\pi)\int_0^\infty C(k)\cos(kx)dk$. To derive it, extend $f$ evenly to the real line. Its [Fourier transform](fourier-transform-split.md) with negative exponential is $2C(k)$, and its odd sine contribution vanishes. The [Fourier inversion theorem](fourier-inversion-theorem.md) then gives the stated factor $2/\pi$. If the forward transform is instead defined as $\widehat f_c=2C$, the inverse factor is $1/\pi$.

With boundary terms at infinity vanishing, two [integrations by parts](integration-by-parts.md) give the cosine transform of $f''$ as $-k^2C(k)-f'(0)$. Thus a homogeneous [Neumann boundary condition](neumann-boundary-condition.md) makes it a multiplier $-k^2C(k)$, paralleling the [Fourier sine transform](fourier-sine-transform.md) with a homogeneous [Dirichlet boundary condition](dirichlet-boundary-condition.md).

## ↑ Ancestors (5)

1. [Fourier transform](fourier-transform-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-1/3/i/solution.md)
