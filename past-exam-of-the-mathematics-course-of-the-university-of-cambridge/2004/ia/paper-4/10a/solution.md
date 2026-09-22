<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

Write $k=GM$ and $r=|\mathbf r|$. The gravitational [central force](../../../../../central-force.md) has zero [torque](../../../../../torque.md), so the specific [angular momentum](../../../../../angular-momentum.md)

$$
\mathbf h=\mathbf r\times\dot{\mathbf r},\qquad
\dot{\mathbf h}=\mathbf r\times\ddot{\mathbf r}=0
$$

is constant. For a nonradial orbit $h=|\mathbf h|>0$, motion lies in the plane normal to $\mathbf h$, and plane polar coordinates give $r^2\dot\theta=h$. With $u=1/r$ and primes denoting $\theta$ derivatives,

$$
\dot r=-hu',\qquad \ddot r=-h^2u^2u'',\qquad r\dot\theta^2=h^2u^3.
$$

The radial equation $\ddot r-r\dot\theta^2=-k/r^2$ is therefore the [Binet equation](../../../../../binet-equation.md)

$$
u''+u=\frac{k}{h^2}.
$$

Its general solution, after choosing the polar origin of angle, is

$$
u=\frac{k}{h^2}(1+e\cos\theta),\qquad
\boxed{r=\frac{p}{1+e\cos\theta},\quad p=\frac{h^2}{GM}.}
$$

The origin is a focus of this [conic section](../../../../../conic-section.md). To identify which [conic section](../../../../../conic-section.md) occurs, use the conserved specific [energy](../../../../../energy.md)

$$
\varepsilon=\frac12(\dot r^2+r^2\dot\theta^2)-\frac{k}{r}
=\frac{h^2}{2}\left[(u')^2+u^2\right]-ku
=\frac{k^2}{2h^2}(e^2-1).
$$

A bound, nonradial orbit has $\varepsilon<0$, hence $0\leq e<1$ and is an [ellipse](../../../../../ellipse.md). For example, putting $x=r\cos\theta$, $y=r\sin\theta$ in $r+ex=p$ gives

$$
(1-e^2)\left(x+\frac{ep}{1-e^2}\right)^2+y^2=\frac{p^2}{1-e^2},
$$

an explicit [ellipse](../../../../../ellipse.md) equation. This is the intended low, bound [Kepler orbit](../../../../../kepler-orbit.md). The inverse-square equation alone does not imply an [ellipse](../../../../../ellipse.md): an initially tangential [speed](../../../../../speed.md) larger than $\sqrt{2GM/r}$ gives $\varepsilon>0$, $e>1$ and a [hyperbolic Kepler orbit](../../../../../hyperbolic-kepler-orbit.md). Zero [angular momentum](../../../../../angular-momentum.md) instead gives radial motion. Those qualifications are necessary for the elliptic conclusion.

In a circular orbit, centripetal [acceleration](../../../../../acceleration.md) balances the gravitational [acceleration](../../../../../acceleration.md):

$$
r_0\Omega^2=\frac{GM}{r_0^2},\qquad
\boxed{T=\frac{2\pi}{\Omega}=2\pi\sqrt{\frac{r_0^3}{GM}}.}
$$

Here $\Omega$ is the positive [angular speed](../../../../../angular-speed.md); either sense of circulation has this [period](../../../../../period-of-a-function.md).

With the stated drag [force](../../../../../force.md), use the full [angular momentum](../../../../../angular-momentum.md) $\mathbf L=m\mathbf r\times\dot{\mathbf r}$. Gravitational [torque](../../../../../torque.md) is still zero, while the drag [torque](../../../../../torque.md) is

$$
\dot{\mathbf L}=\mathbf r\times(-A\dot{\mathbf r})
=-\frac{A}{m}\mathbf L.
$$

Therefore $\boxed{\mathbf L(t)=\mathbf L(0)e^{-At/m}}$ for constant $A>0$. Its direction remains fixed, and its magnitude has [exponential decay](../../../../../exponential-decay.md) with time constant $m/A$; the orbit remains planar although its shape is no longer a fixed [ellipse](../../../../../ellipse.md).

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
