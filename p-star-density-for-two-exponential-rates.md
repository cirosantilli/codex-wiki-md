# P-star density for two exponential rates

↑ **Parent:** [P-star approximation](p-star-approximation.md)

For independent samples of size $n$ from [exponential distributions](exponential-distribution.md) with rates $\lambda$ and $\psi\lambda$, the [maximum-likelihood estimators](maximum-likelihood-estimator.md) are $\widehat\lambda=n/S$ and $\widehat\psi=S/T$, where $S$ and $T$ are the respective sample sums. Their normalized [P-star approximation](p-star-approximation.md) is exact:

$$
p(\widehat\psi,\widehat\lambda;\psi,\lambda)=\frac{n^{2n}\psi^n\lambda^{2n}}{\Gamma(n)^2\widehat\psi^{n+1}\widehat\lambda^{2n+1}}\exp\left\{-\frac{n\lambda}{\widehat\lambda}\left(1+\frac\psi{\widehat\psi}\right)\right\},\qquad \widehat\psi,\widehat\lambda>0.
$$

Indeed, $S$ and $T$ have independent [gamma distributions](gamma-distribution.md) with shapes $n$ and respective rates $\lambda,\psi\lambda$. The [Jacobian determinant](jacobian-determinant.md) of their inverse transformation is $n^2/(\widehat\psi^2\widehat\lambda^3)$, giving the displayed [density](density.md). Alternatively the square root of the determinant of the fitted [observed information](observed-fisher-information.md) is $n/(\widehat\psi\widehat\lambda)$; multiplying by the exponential of the fitted [log-likelihood](log-likelihood.md) difference gives the same shape. Its normalizing constant in the [P-star approximation](p-star-approximation.md) is $c_n=n^{2n-1}e^{-2n}/\Gamma(n)^2$. Integrating over $\widehat\lambda$ gives

$$
p(\widehat\psi;\psi)=\frac{\Gamma(2n)}{\Gamma(n)^2\psi}\left(\frac{\widehat\psi}\psi\right)^{n-1}\left(1+\frac{\widehat\psi}\psi\right)^{-2n},
$$

so $\widehat\psi/\psi$ has the [F-distribution](f-distribution.md) with degrees of freedom $(2n,2n)$.

## ↑ Ancestors (10)

1. [P-star approximation](p-star-approximation.md)
2. [Saddlepoint density approximation](saddlepoint-density-approximation.md)
3. [Cumulant-generating function](cumulant-generating-function.md)
4. [Moment-generating function](moment-generating-function.md)
5. [Probability distribution](probability-distribution.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-38/1/solution.md)
