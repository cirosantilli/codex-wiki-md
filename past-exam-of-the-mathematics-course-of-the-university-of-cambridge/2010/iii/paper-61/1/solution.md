<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $\mathcal G=G(M_\star+M_{\rm pl})$, $h=\sqrt{\mathcal G a(1-e^2)}$, $\theta=\omega+f$ and $L=n_{\rm pl}t$. Here $h$ is the [specific angular momentum](../../../../../specific-angular-momentum.md), $f$ is the [true anomaly](../../../../../true-anomaly.md) and $\omega$ is the planar [longitude of periapsis](../../../../../longitude-of-periapsis.md). Differentiating the [Kepler orbit](../../../../../kepler-orbit.md) equation with $\dot f=h/r^2$ gives

$$
\dot r=\frac{\mathcal G}{h}e\sin f=Ae\sin f,\qquad r\dot f=A(1+e\cos f).
$$

Resolve the [velocity](../../../../../velocity.md) along the radial and tangential [unit vectors](../../../../../unit-vector.md), $\widehat{\boldsymbol r}=(\cos\theta,\sin\theta)$ and $\widehat{\boldsymbol\theta}=(-\sin\theta,\cos\theta)$. The identities $\sin f\cos\theta-\cos f\sin\theta=-\sin\omega$ and $\sin f\sin\theta+\cos f\cos\theta=\cos\omega$ yield

$$
\boxed{\dot x=-A(\sin\theta+e\sin\omega),\qquad \dot y=A(\cos\theta+e\cos\omega).}
$$

This is the [Kepler velocity hodograph](../../../../../kepler-velocity-hodograph.md): the [velocity](../../../../../velocity.md) runs around a circle whose centre is displaced by the [orbital eccentricity](../../../../../orbital-eccentricity.md).

The [centre of mass](../../../../../center-of-mass.md) condition gives the star's barycentric position $\boldsymbol r_\star=-\mu a_{\rm pl}(\cos L,\sin L)$. Translating to the star without rotating the axes gives $\boldsymbol r'=\boldsymbol r-\boldsymbol r_\star$ and $\boldsymbol v'=\boldsymbol v-\dot{\boldsymbol r}_\star$. From [Kepler's third law](../../../../../kepler-s-third-law.md), $n_{\rm pl}^2a_{\rm pl}^3=\mathcal G$, so

$$
\mu a_{\rm pl}n_{\rm pl}=A\kappa,\qquad \kappa=\mu\alpha^{-1/2}\sqrt{1-e^2}.
$$

Consequently

$$
\boxed{\dot x'=\dot x-A\kappa\sin L,\qquad \dot y'=\dot y+A\kappa\cos L.}
$$

The small displacement and the larger reflex [velocity](../../../../../velocity.md) have different orders: $|\boldsymbol r'-\boldsymbol r|/a=\mu\alpha$, but the reflex speed divided by the circular speed is $\mu\alpha^{-1/2}$. These are the source of the [astrocentric osculating-element oscillations](../../../../../astrocentric-osculating-element-oscillations.md).

For the coordinate ratio, the exact result is

$$
\frac{x'-x}{x}=\frac{\mu\alpha\cos L}{(r/a)\cos\theta}.
$$

For fixed $e<1$, $r/a\ge1-e$, so this is $O(\mu\alpha)$ on any angular region with $|\cos\theta|$ bounded away from zero. The printed coordinate claim is not uniform over a full orbit: at $x=0$ its ratio is undefined. The nonsingular statement is $|\boldsymbol r'-\boldsymbol r|/r\le\mu\alpha/(1-e)$, assuming the [pericentre distance](../../../../../pericentre-distance.md) remains much larger than the binary separation.

Squaring the two components of the [velocity](../../../../../velocity.md) gives

$$
\boxed{v'^2=A^2\left[1+e^2+2e\cos f+\kappa^2+2\kappa\{\cos(L-\theta)+e\cos(L-\omega)\}\right].}
$$

At $\mu=0$, $\kappa=0$ and $\mathcal G=GM_\star$. Since

$$
\frac{1+e^2+2e\cos f}{a(1-e^2)}=\frac2r-\frac1a,
$$

this reduces to the [vis-viva equation](../../../../../vis-viva-equation.md), $v'^2=GM_\star(2/r-1/a)$.

Now let the barycentric [Kepler orbit](../../../../../kepler-orbit.md) be circular, write $\Delta=L-\theta$ and $\varepsilon=\mu\alpha^{-1/2}\ll1$, and put $v_0=\sqrt{\mathcal G/a}$. The [osculating orbital elements](../../../../../osculating-orbital-element.md) about the star use the gravitational parameter $GM_\star=(1-\mu)\mathcal G$. To the required order, $r'=a[1+O(\mu\alpha)]$ and $v'^2=v_0^2[1+2\varepsilon\cos\Delta+O(\varepsilon^2)]$. The [specific orbital energy](../../../../../specific-orbital-energy.md) therefore implies

$$
\frac a{a'}=\frac{2a}{r'}-\frac{av'^2}{GM_\star}=1-2\varepsilon\cos\Delta+O(\mu+\varepsilon^2),
\qquad \boxed{\frac{a'}a-1=2\mu\alpha^{-1/2}\cos\Delta+O(\mu+\varepsilon^2).}
$$

Here $\mu=o(\varepsilon)$ and $\varepsilon^2=o(\varepsilon)$ under the stated hierarchy. Even at a phase where the leading cosine vanishes, the absolute error bound remains valid.

Finally, use the [eccentricity vector](../../../../../eccentricity-vector.md) $\boldsymbol e'=(\boldsymbol v'\times\boldsymbol h')/(GM_\star)-\widehat{\boldsymbol r}'$. In radial and tangential components it is

$$
e'_r=\frac{r'v_\theta'^2}{GM_\star}-1,\qquad e'_\theta=-\frac{r'v'_rv'_\theta}{GM_\star}.
$$

The translation changes the radial basis only by $O(\mu\alpha)$, whereas $v'_r=-v_0\varepsilon\sin\Delta+O(v_0\mu\alpha)$ and $v'_\theta=v_0(1+\varepsilon\cos\Delta)+O(v_0\mu\alpha)$. Thus

$$
\boxed{e'\cos(\omega'-\omega-f)=2\mu\alpha^{-1/2}\cos\Delta+O(\mu+\varepsilon^2),\qquad e'\sin(\omega'-\omega-f)=\mu\alpha^{-1/2}\sin\Delta+O(\mu+\varepsilon^2).}
$$

For the original circular [Kepler orbit](../../../../../kepler-orbit.md), $\omega$ and $f$ are separately arbitrary; their sum $\theta$ is well defined. Using the [eccentricity vector](../../../../../eccentricity-vector.md) avoids introducing an undefined [pericentre](../../../../../periapsis.md) for that circular [Kepler orbit](../../../../../kepler-orbit.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
