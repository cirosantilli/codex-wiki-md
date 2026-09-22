<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The shell feels only radial gravity and the radial force due to the [cosmological constant](../../../../../../cosmological-constant.md), so its torque vanishes and its [specific angular momentum](../../../../../../specific-angular-momentum.md) $L=r^2\dot\theta$ is conserved. Multiplying

$$
\ddot r=\frac{L^2}{r^3}-\frac{GM}{r^2}+\frac\Lambda3r
$$

by $\dot r$ and integrating gives the conserved [specific orbital energy](../../../../../../specific-orbital-energy.md)

$$
\boxed{E=\frac12\dot r^2+\frac{L^2}{2r^2}-\frac{GM}{r}-\frac\Lambda6r^2.}
$$

For a uniform sphere, assembling concentric shells gives its gravitational [potential energy](../../../../../../potential-energy.md)

$$
W_{G,{\rm ta}}=-\int_0^{r_{\rm ta}}\frac{GM(r)}r\,dM
=-\frac{3GM^2}{5r_{\rm ta}}.
$$

The cosmological-constant potential per unit mass is $-\Lambda r^2/6$. Since $\langle r^2\rangle=3r_{\rm ta}^2/5$ in a uniform sphere,

$$
W_{\Lambda,{\rm ta}}=-\frac\Lambda6M\langle r^2\rangle
=-\frac1{10}\Lambda Mr_{\rm ta}^2.
$$

The scalar [virial theorem](../../../../../../virial-theorem.md) weights a potential homogeneous of degree $n$ by $-nW$. Gravity has degree $-1$ and the $\Lambda$ potential degree $2$, so the final state obeys

$$
\boxed{2T_f+W_{G,f}=2W_{\Lambda,f}.}
$$

At turnaround $T=0$, while the virial relation gives $E_f=W_{G,f}/2+2W_{\Lambda,f}$. Conservation of energy, together with $M=4\pi\rho_{\rm ta}r_{\rm ta}^3/3$, then gives, for $x=r_f/r_{\rm ta}$ and $\eta=\Lambda/(4\pi G\rho_{\rm ta})$,

$$
\boxed{2\eta x^3-(2+\eta)x+1=0.}
$$

The root connected continuously to the $\Lambda=0$ solution has $x=1/2-\eta/8+O(\eta^2)$, equivalently

$$
\boxed{\frac{r_f}{r_{\rm ta}}\simeq
\frac{1-\eta/2}{2-\eta/2}}
$$

to first order in $\eta$. With $\Lambda=0$, virialization occurs at half the [turnaround radius](../../../../../../turnaround-radius.md). At fixed turnaround state, positive $\Lambda$ makes this equilibrium root slightly smaller because its repulsive quadratic potential enters both energy conservation and the virial relation; sufficiently strong repulsion instead prevents a bound virialized state. Negative $\Lambda$ shifts the root in the opposite direction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 346](../../../paper-346-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
