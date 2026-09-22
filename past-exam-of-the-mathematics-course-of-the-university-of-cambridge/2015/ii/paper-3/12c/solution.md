<h1 id="12c/solution">Solution</h1>

↑ **Parent:** [12C](../12c.md)

The terms in the [Boltzmann equation](../../../../../boltzmann-equation.md) respectively describe dilution by expansion, pair annihilation, and pair production from the thermal bath. The annihilation rate per volume is $\langle\sigma v\rangle n\bar n$; $P(t)$ is the corresponding production rate. Antiparticles satisfy the same equation with $n$ replaced by $\bar n$. Subtracting gives

$$
\frac{d(n-\bar n)}{dt}=-3H(n-\bar n),\qquad \boxed{(n-\bar n)a^3=\hbox{constant}.}
$$

Initial particle-antiparticle symmetry therefore persists. [Detailed balance](../../../../../detailed-balance.md) in the thermal bath gives $P=\langle\sigma v\rangle n_{\rm eq}^2$, so

$$
\frac{d(na^3)}{dt}=\langle\sigma v\rangle(n_{\rm eq}^2-n^2)a^3.
$$

During [radiation domination](../../../../../radiation-domination.md), with fixed effective relativistic degrees of freedom, $T\propto a^{-1}$ and $H=H_m/x^2$. Thus $\dot x=Hx$ and the dilution terms cancel in $Y=n/T^3$:

$$
\dot Y=-\langle\sigma v\rangle T^3(Y^2-Y_{\rm eq}^2),\qquad \boxed{\frac{dY}{dx}=-\frac{m^3\langle\sigma v\rangle}{H_mx^2}(Y^2-Y_{\rm eq}^2).}
$$

After [cosmological particle freeze-out](../../../../../cosmological-particle-freeze-out.md), neglect $Y_{\rm eq}$. For constant $\lambda$ the exact reduced solution is

$$
\frac1{Y(x)}=\frac1{Y_f}+\lambda\left(\frac1{x_f}-\frac1x\right),\qquad \boxed{Y_\infty=\left(\frac1{Y_f}+\frac\lambda{x_f}\right)^{-1}.}
$$

For the [post-freeze-out relic abundance](../../../../../post-freeze-out-relic-abundance.md), the familiar answer $Y_\infty\simeq x_f/\lambda$ additionally neglects $1/Y_f$ compared with $\lambda/x_f$. **It is an approximation, not an exact consequence of the post-freeze-out equation without initial data.** A smaller annihilation cross-section means smaller $\lambda$, earlier decoupling and less depletion, so weakly interacting particles normally have a larger relic abundance.

## ↑ Ancestors (10)

1. [12C](../12c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
