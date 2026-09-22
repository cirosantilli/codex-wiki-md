<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

For a [central potential](../../../../../central-potential.md), [angular momentum](../../../../../angular-momentum.md) is conserved and the motion lies in a plane. With $L=mr^2\dot\theta$, radial [energy](../../../../../energy-split.md) conservation becomes

$$
\mathcal E=\frac12m\dot r^2+V_{\rm eff}(r),\qquad V_{\rm eff}(r)=V(r)+\frac{L^2}{2mr^2}.
$$

Allowed radii have $\mathcal E\ge V_{\rm eff}$; equality gives radial [turning points](../../../../../turning-point.md). A well with two finite [turning points](../../../../../turning-point.md) gives regular radially bound motion. Access to arbitrarily large radii gives an unbound branch, while access to the origin can lead to collision in a singular potential. Stationary points are circular-orbit candidates; a strict local minimum gives radial [stability](../../../../../stability-of-a-numerical-method.md). For a potential tending to zero at infinity, [energy](../../../../../energy-split.md) relative to that asymptote is useful, but a singular inner potential and centrifugal barrier must still be examined.

Integrating the angular-momentum relation with the origin of [angle](../../../../../angle.md) at $t=0$ gives

$$
\boxed{\theta(t)=\frac Lm\int_0^t\frac{dt'}{r(t')^2}.}
$$

For $V=-A/r+B/r^2$ at $L=L_0$, the [effective potential](../../../../../effective-potential.md) is $-A/r+(L_0^2+2mB_0)/(2mr^2)$. It is exactly the Kepler [effective potential](../../../../../effective-potential.md) with $L_{\rm K}=\sqrt{L_0^2+2mB_0}$, provided that expression is real. Equal radial [energy](../../../../../energy-split.md) and initial radial phase therefore give identical $r(t)$, although the angular motion differs. Writing $\psi$ for the Kepler [angle](../../../../../angle.md), $\dot\theta/\dot\psi=L_0/L_{\rm K}=k$. With matched periapsis origins,

$$
\theta=k\psi,\qquad \boxed{r(\theta)=\frac{r_0}{1+e\cos(\theta/k)},\quad k=\frac{L_0}{\sqrt{L_0^2+2mB_0}}.}
$$

Here $r_0=L_{\rm K}^2/(mA)$ and the [eccentricity](../../../../../eccentricity-of-a-conic.md) is fixed by radial [energy](../../../../../energy-split.md). For $B_0>0$, $k<1$ and successive periapses are separated by $2\pi k$, so there is retrograde apsidal motion relative to a closed Kepler ellipse. The radial equivalence is the relevant content of the [Newton's theorem of revolving orbits](../../../../../newton-s-theorem-of-revolving-orbits.md).

For the pure [inverse-cube central force](../../../../../inverse-cube-central-force.md) set $A=0$. The free-particle reference orbit at $B=0$ is a straight line, $r=d/\cos(\psi-\psi_0)$, not a finite-$A$ conic with its old $r_0$ held fixed. To cover attractive as well as repulsive cases completely, put

$$
u=1/r,\qquad \lambda=1+\frac{2mB}{L^2},\qquad u''+\lambda u=0,\qquad \mathcal E=\frac{L^2}{2m}(u'^2+\lambda u^2),
$$

where primes denote [angle](../../../../../angle.md) derivatives and $L\ne0$. The [inverse-cube central orbit classification](../../../../../inverse-cube-central-orbit-classification.md) gives the following physically positive-radius branches.

For **$\lambda>0$**, write $u=C\cos[\sqrt\lambda(\theta-\theta_0)]$ with $C>0$, so $r=C^{-1}\sec[\sqrt\lambda(\theta-\theta_0)]$. These are scattering orbits with positive [energy](../../../../../energy-split.md) and an inner turning radius $1/C$; the angular interval between the two infinite-radius ends is $\pi/\sqrt\lambda$. Repulsion ($B>0$) gives an interval smaller than $\pi$; weak attraction ($-L^2/(2m)<B<0$) gives a larger interval and can cause winding. The $B=0$ limit is the straight line.

For **$\lambda=0$**, $u=C+D(\theta-\theta_0)$. If $D\ne0$, reciprocal-linear spirals connect an infinite-radius end to collision at infinite accumulated [angle](../../../../../angle.md). If $D=0$ and $C>0$, every radius admits a circular solution at zero [energy](../../../../../energy-split.md): attraction exactly balances centrifugal acceleration. Each is a [marginal circular orbit under an inverse-cube force](../../../../../marginal-circular-orbit-under-an-inverse-cube-force.md), with no radial restoring [force](../../../../../force-split.md).

For **$\lambda<0$**, put $\beta=\sqrt{-\lambda}$ and $u=C_+e^{\beta\theta}+C_-e^{-\beta\theta}$. Up to [angle](../../../../../angle.md) shifts and reversal, the three [energy](../../../../../energy-split.md) classes are

$$
\begin{array}{c|c|c}
\mathcal E>0&r=d\,\operatorname{csch}[\beta(\theta-\theta_0)]&\text{infinity to collision}\\
\mathcal E=0&r=d e^{-\beta(\theta-\theta_0)}&\text{logarithmic collision/escape spiral}\\
\mathcal E<0&r=d\,\operatorname{sech}[\beta(\theta-\theta_0)]&\text{outer turning radius }d
\end{array}
$$

with positive-radius domains understood. The negative-energy branch is radially bounded but reaches the singular centre on either side of its outer [turning point](../../../../../turning-point.md); it is not a regular closed orbit. Collision requires additional physics to continue through $r=0$. Zero [angular momentum](../../../../../angular-momentum.md) gives radial trajectories and is excluded from the angular parametrization above.

<a id="section-c/c10/image-original-representative-inverse-cube-orbit-branches-with-force-sign-and-critical-attraction-distinguished"></a>
![](../../../../../past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-1-inverse-cube-orbits.png)

**[Figure 4](#section-c/c10/image-original-representative-inverse-cube-orbit-branches-with-force-sign-and-critical-attraction-distinguished). Original representative inverse-cube orbit branches, with force sign and critical attraction distinguished**.

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
