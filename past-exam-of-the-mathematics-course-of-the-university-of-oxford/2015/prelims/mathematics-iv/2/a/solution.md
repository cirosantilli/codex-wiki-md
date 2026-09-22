<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By [Newton's second law](../../../../../../newton-s-second-law.md), the [central force](../../../../../../central-force.md) obeys

$$
m\ddot{\mathbf r}=-\Phi'(r)\frac{\mathbf r}{r}.
$$

Differentiating the [cross product](../../../../../../cross-product.md) gives

$$
\dot{\mathbf n}=\dot{\mathbf r}\wedge\dot{\mathbf r}+\mathbf r\wedge\ddot{\mathbf r}=\mathbf0,
$$

since the [acceleration](../../../../../../acceleration.md) is parallel to $\mathbf r$. Hence $\mathbf n=\mathbf n(0)$ is constant. Since $\mathbf r\cdot\mathbf n=0$, the entire motion lies in the fixed [plane](../../../../../../plane.md) through the origin with nonzero [normal vector](../../../../../../normal-vector.md) $\mathbf n(0)$.

Choose [polar coordinates](../../../../../../polar-coordinates.md) in that [plane](../../../../../../plane.md), orienting $\theta$ so that its positive [normal vector](../../../../../../normal-vector.md) points along $\mathbf n(0)$. The [velocity](../../../../../../velocity.md) is

$$
\dot{\mathbf r}=\dot r\,\mathbf e_r+r\dot\theta\,\mathbf e_\theta,
\qquad
\mathbf r\wedge\dot{\mathbf r}=r^2\dot\theta\,\mathbf e_z.
$$

Therefore

$$
\boxed{r^2\dot\theta=h=|\mathbf n(0)|>0.}
$$

Multiplication by $m$ identifies this with [conservation of angular momentum](../../../../../../conservation-of-angular-momentum.md); geometrically, the swept [area](../../../../../../surface-area.md) per unit time is $h/2$.

Taking the [dot product](../../../../../../dot-product.md) of [Newton's second law](../../../../../../newton-s-second-law.md) with the [velocity](../../../../../../velocity.md) gives

$$
\frac{d}{dt}\left(\frac m2|\dot{\mathbf r}|^2+\Phi(r)\right)
=m\dot{\mathbf r}\cdot\ddot{\mathbf r}+\Phi'(r)\dot r=0.
$$

Thus

$$
\boxed{\frac m2\left(\dot r^2+r^2\dot\theta^2\right)+\Phi(r)=E.}
$$

This expresses [conservation of mechanical energy](../../../../../../conservation-of-mechanical-energy.md), the sum of [kinetic energy](../../../../../../kinetic-energy.md) and [potential energy](../../../../../../potential-energy.md).

Finally, for $u=1/r$ and a prime denoting a [derivative](../../../../../../derivative.md) with respect to $\theta$, the [chain rule](../../../../../../chain-rule.md) gives

$$
\dot\theta=hu^2,\qquad
\dot r=-u^{-2}u'\dot\theta=-hu',\qquad
r\dot\theta=hu.
$$

Substitution into the conserved [energy](../../../../../../energy-split.md) yields

$$
\boxed{\frac{mh^2}{2}\left[\left(\frac{du}{d\theta}\right)^2+u^2\right]+\Phi(1/u)=E.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Mathematics IV](../../../mathematics-iv-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
