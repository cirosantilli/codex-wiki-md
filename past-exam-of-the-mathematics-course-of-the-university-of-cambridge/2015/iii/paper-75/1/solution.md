<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Gaussian units](../../../../../gaussian-units.md) convention implicit in the $4\pi$ coefficient. For a uniform dielectric and a counterion-only [electrolyte](../../../../../electrolyte.md), the [Boltzmann distribution](../../../../../boltzmann-distribution.md) and [Poisson-Boltzmann equation](../../../../../poisson-boltzmann-equation.md) are

$$
n(r)=n_0e^{-\beta q\phi(r)},\qquad \rho(r)=qn(r),\qquad \frac1r\frac{d}{dr}\left(r\frac{d\phi}{dr}\right)=-\frac{4\pi qn_0}{\epsilon}e^{-\beta q\phi},\qquad \beta=(k_BT)^{-1}.
$$

The reference [electric potential](../../../../../electric-potential.md) is $\phi(a)=0$, so $n_0=n(a)$; it is not a prescribed nonzero bulk [concentration](../../../../../concentration.md) at infinity. A salt reservoir with additional [ion](../../../../../ion.md) species would require their charge densities as well. With $u=\log(r/a)$, the cylindrical [Laplacian](../../../../../laplacian.md) is $r^{-2}d^2/du^2$. Since $\beta q\phi=\Phi+2u$ and $r^2=a^2e^{2u}$, the factors of $e^{2u}$ cancel:

$$
\boxed{\Phi''=-C e^{-\Phi},\qquad C=\frac{4\pi\beta q^2a^2n_0}{\epsilon}.}
$$

Here primes mean differentiation with respect to $u$, and the surface condition is $\Phi(0)=0$ in this coordinate.

Multiply by $\Phi'$ to obtain a [first integral](../../../../../first-integral.md):

$$
\frac12\Phi'^2=C e^{-\Phi}+K.
$$

The two specified far-field limits set $K=0$. For a solution tending upwards to infinity, take the positive square root. Writing $b=\sqrt{C/2}$ gives $(e^{\Phi/2})'=b$, hence the [cylindrical counterion-only Poisson-Boltzmann profile](../../../../../cylindrical-counterion-only-poisson-boltzmann-profile.md)

$$
\boxed{\Phi(u)=2\log(1+bu),\qquad \beta q\phi(r)=2\log\frac ra+2\log\left(1+b\log\frac ra\right).}
$$

For $b>0$, $\Phi\to\infty$ and $\Phi'=2b/(1+bu)\to0$. The corresponding number density is

$$
\boxed{n(r)=\frac{n_0(a/r)^2}{[1+b\log(r/a)]^2}.}
$$

Apply [Gauss's law](../../../../../gauss-s-law.md) to a coaxial surface per unit cylinder length. Define the positive accumulated [cylindrical screening charge](../../../../../cylindrical-screening-charge.md) by

$$
Q(r)=2\pi\int_a^r s\rho(s)\,ds.
$$

The signed outward [electric field](../../../../../electric-field.md) is $E_r=2[-\lambda+Q(r)]/(\epsilon r)$, so its magnitude is $2|\lambda-Q(r)|/(\epsilon r)$. In the branch here, $Q(r)<\lambda$, the field is inward and

$$
\boxed{E(r)=\phi'(r)=\frac2{\epsilon r}\left[\lambda-2\pi\int_a^r s\rho(s)\,ds\right],\qquad Q_{\rm screening}=2\pi\int_a^\infty r\rho(r)\,dr.}
$$

In this display, $\phi'$ is a radial derivative. The quantities $Q$ are [electric charges](../../../../../electric-charge.md) per unit axial length, not total charges of an infinite cylinder.

At the surface, $a\phi'(a)=2\lambda/\epsilon$. Define the charge-$q$ [Bjerrum length](../../../../../bjerrum-length.md) $\ell_B=\beta q^2/\epsilon$ and the [Manning parameter](../../../../../manning-parameter.md) $\eta=\lambda\ell_B/q$. Matching the derivative of the solution gives

$$
\Phi'(0)=\beta qa\phi'(a)-2=2(\eta-1)=2b,\qquad b=\eta-1.
$$

Thus the condensed branch exists only for $\eta>1$, and its normalization is

$$
\boxed{\lambda_c=\frac q{\ell_B},\qquad n_0=\frac{(\eta-1)^2}{2\pi\ell_B a^2}\quad(\lambda>\lambda_c).}
$$

The sign condition $b>0$ is essential: simply squaring $\eta-1$ would produce a spurious subcritical density. Direct integration using $r\,n(r)\,dr=n_0a^2du/(1+bu)^2$ yields

$$
Q(r)=\lambda_c b\left[1-\frac1{1+b\log(r/a)}\right],\qquad \boxed{Q_{\rm screening}=\lambda_c b=\lambda-\lambda_c.}
$$

Equivalently, $E(r)=2\lambda_c[1+b/(1+b\log(r/a))]/(\epsilon r)$: the remaining far-field line-charge magnitude is $\lambda_c$. The [Manning condensed fraction](../../../../../manning-condensed-fraction.md) is $1-1/\eta$.

Below threshold, no positive-density profile can satisfy those same far-field conditions. Indeed $\Phi''\leq0$, so a negative initial slope $2(\eta-1)$ cannot increase to zero. The physical interpretation is the [infinite-dilution limit of cylindrical counterions](../../../../../infinite-dilution-limit-of-cylindrical-counterions.md): start with a neutral finite cylindrical cell and send its outer radius to infinity. For $\eta\leq1$, [counterions](../../../../../counterion.md) escape to arbitrarily large radii, leaving **$n_0\to0$ and no finite condensed charge**. The bare-cylinder [Boltzmann distribution](../../../../../boltzmann-distribution.md) $n\propto r^{-2\eta}$ also shows why its radial normalization $\int r^{1-2\eta}dr$ diverges in this regime. In the local zero-density limit, $\Phi=2(\eta-1)u$; this does not obey the condensed branch's imposed limits. At $\eta=1$ the branch has zero amplitude and $\Phi=0$, rather than $\Phi\to\infty$.

Consequently the intended [counterion condensation](../../../../../counterion-condensation.md) result, interpreted as a local infinite-dilution density, is

$$
\boxed{n_0=\frac{[\max(\eta-1,0)]^2}{2\pi\ell_Ba^2},\qquad Q_{\rm condensed}=\max(\lambda-\lambda_c,0).}
$$

Every finite neutral cell still contains enough [counterions](../../../../../counterion.md) to neutralize the cylinder; the missing residual charge in the local limiting profile is carried to infinity. Taking the infinite-cell limit before the charge integral differs from integrating the entire finite cell first. In SI units, the same reference-charge [Bjerrum length](../../../../../bjerrum-length.md) is $q^2/(4\pi\epsilon_{\rm abs}k_BT)$; the electrostatic prefactors must be changed consistently.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
