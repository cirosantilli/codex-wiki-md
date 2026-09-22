# MRA projection Fourier identity

↑ **Parent:** [Scaling function](scaling-function.md)

Use $\widehat f(\xi)=\int f(x)e^{-ix\xi}\,dx$ and let $P_j$ be the [orthogonal projection](orthogonal-projection.md) onto the closed span of the orthonormal translates and dilates of a [scaling function](scaling-function.md). If $\widehat f$ is supported in $[-R,R]$ and $R<\pi2^j$, then

$$
\|P_jf\|_2^2=\frac1{2\pi}\int|\widehat f(\xi)|^2|\widehat\varphi(2^{-j}\xi)|^2\,d\xi.
$$

Indeed, the [Plancherel theorem](plancherel-theorem.md) writes the coefficient against $\varphi_{j,k}$ as $2^{-j/2}(2\pi)^{-1}\int\widehat f(\xi)\overline{\widehat\varphi(2^{-j}\xi)}e^{ik2^{-j}\xi}\,d\xi$. With $\xi=2^j\theta$, these are $2^{j/2}$ times the [Fourier series](fourier-series-split.md) coefficients of $\widehat f(2^j\theta)\overline{\widehat\varphi(\theta)}$ on $[-\pi,\pi]$. The [Parseval identity](parseval-identity.md) proves the formula. It shows that continuity and unit modulus at zero imply density of the refinement spaces, and conversely that density forces this unit modulus when the [Fourier transform](fourier-transform.md) is continuous at zero.

## ↑ Ancestors (8)

1. [Scaling function](scaling-function.md)
2. [Multiresolution analysis](multiresolution-analysis.md)
3. [Wavelet](wavelet.md)
4. [Fourier analysis](fourier-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/2/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/2/b/solution.md)
- [Scaling function](scaling-function.md)
