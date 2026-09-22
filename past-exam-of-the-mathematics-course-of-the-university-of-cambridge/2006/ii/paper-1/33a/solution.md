<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

For unit incident plane-wave amplitude, define the [scattering amplitude](../../../../../scattering-amplitude.md) by $\psi\sim e^{ikz}+f(\theta)e^{ikr}/r$ at large $r$. Comparing outgoing radial flux with incident flux gives $d\sigma/d\Omega=|f(\theta)|^2$. Outside the potential, a real regular radial solution is proportional to $j_\ell(kr)\cos\delta_\ell-n_\ell(kr)\sin\delta_\ell$, with asymptotic phase $\sin(kr-\ell\pi/2+\delta_\ell)/(kr)$. This defines the [scattering phase shift](../../../../../scattering-phase-shift.md) modulo $\pi$.

The incident plane-wave expansion supplies coefficient $(2\ell+1)i^\ell$ for $j_\ell P_\ell$. To preserve its incoming part, replace $j_\ell$ by $e^{i\delta_\ell}(j_\ell\cos\delta_\ell-n_\ell\sin\delta_\ell)$. Writing the asymptotic sine in exponentials shows that its incoming coefficient is unchanged and its outgoing coefficient is multiplied by $e^{2i\delta_\ell}$. The outgoing difference from the plane wave therefore gives

$$
\boxed{f(\theta)=\frac1{2ik}\sum_{\ell\geq0}(2\ell+1)(e^{2i\delta_\ell}-1)P_\ell(\cos\theta)=\frac1k\sum_{\ell\geq0}(2\ell+1)e^{i\delta_\ell}\sin\delta_\ell P_\ell(\cos\theta).}
$$

Put $\rho=ka$, $t=\tan\delta_\ell$, and abbreviate $j=j_\ell(\rho)$, $n=n_\ell(\rho)$. Logarithmic-derivative matching gives $aR_\ell'(a)/R_\ell(a)=\rho(j'-tn')/(j-tn)$. The supplied asymptotics determine the constant [Wronskian](../../../../../wronskian.md): $\rho^2(jn'-j'n)=1$. Consequently

$$
Q_\ell=\rho\left(\frac{j'-tn'}{j-tn}-\frac{j'}j\right)=\frac{-t}{\rho j(j-tn)}.
$$

Solving for $t$ gives

$$
\boxed{\tan\delta_\ell=\frac{Q_\ell j_\ell(ka)^2ka}{Q_\ell n_\ell(ka)j_\ell(ka)ka-1}.}
$$

At zeros of denominators it is interpreted by limits; the logarithmic-derivative definition itself presumes its stated denominators nonzero.

Near a dominant resonant [partial wave](../../../../../partial-wave.md), $\sin^2\delta_\ell\approx\gamma^2/[(k-k_0)^2+\gamma^2]$. Neglecting the small other [partial waves](../../../../../partial-wave.md) yields

$$
\boxed{\frac{d\sigma}{d\Omega}\approx\frac{(2\ell+1)^2}{k^2}\frac{\gamma^2}{(k-k_0)^2+\gamma^2}P_\ell(\cos\theta)^2.}
$$

This is a resonant peak of width $2|\gamma|$ in $k$, with the partial-wave angular pattern and maximum allowed $\sin^2\delta_\ell=1$ at [resonance](../../../../../resonance.md). Integrating gives $\sigma\approx4\pi(2\ell+1)\gamma^2/[k^2((k-k_0)^2+\gamma^2)]$. A small background may matter at angular zeros of the dominant wave.

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
