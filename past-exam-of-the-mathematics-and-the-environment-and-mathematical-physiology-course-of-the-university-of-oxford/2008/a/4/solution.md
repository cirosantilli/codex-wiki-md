<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Glacier sliding](../../../../basal-sliding.md) is motion of the [ice](../../../../ice.md) base relative to its bed, distinct from internal [ice](../../../../ice.md) deformation. Near a melting bed, basal water, [pressure](../../../../pressure-split.md)-melting/refreezing around obstacles and [creep](../../../../creep-deformation.md) past bed [roughness](../../../../surface-roughness.md) can permit motion; a cold frozen bed can suppress it. A simple sliding law is increasing in basal traction, for example $u_b\propto\tau_b^m$ on the positive-traction branch, with resistance also affected in richer models by [roughness](../../../../surface-roughness.md) and [basal water pressure](../../../../basal-water-pressure.md).

Slow [ice](../../../../ice.md) motion has negligible inertial acceleration. In a long shallow [glacier](../../../../glacier.md), leading vertical stress is hydrostatic and longitudinal stress gradients are neglected relative to transverse shear gradients. Resolving gravity downslope and normally yields the two stated balances. This approximates a two-dimensional slab/valley centreline; lateral drag, rapidly varying geometry and strong longitudinal-stress regions need additional terms.

With a stress-[free surface](../../../../free-surface.md),

$$
\boxed{p=\rho g\cos\alpha(h-z),\qquad\tau=\rho g\sin\alpha[1-\cot\alpha\,h_x](h-z).}
$$

Put $K=\rho g\sin\alpha$ and $D=1-\cot\alpha h_x$, assuming positive driving shear for the stated power law. Integrating from the bed gives

$$
\boxed{u(z)=u_b+\frac{A(KD)^n}{n+1}[h^{n+1}-(h-z)^{n+1}],\quad
q=hu_b+\frac{A(KD)^n h^{n+2}}{n+2}.}
$$

The surface speed is $u_s=u_b+A(KD)^nh^{n+1}/(n+1)$. [Mass conservation](../../../../mass-conservation.md), with $a$ measured as [ice](../../../../ice.md)-equivalent thickness [accumulation](../../../../ice-accumulation.md), is $\boxed{h_t+q_x=a}$.

Choose $h=H\hat h$, $x=l\hat x$, $u_b=U\hat u_b$ and $t=(l/U)\hat t$, with $U=(KH/R)^m$. Scale [accumulation](../../../../ice-accumulation.md) with $HU/l$. The [dimensionless](../../../../dimensionless-quantity.md) basal law and parameters are

$$
\boxed{u_b=h^m(1-\mu h_x)^m,\qquad\mu=\frac{H\cot\alpha}{l},\qquad\delta=\frac{A K^nH^{n+1}}U=A R^mK^{n-m}H^{n+1-m}.}
$$

The resulting flux is exactly $hu_b+\delta(1-\mu h_x)^nh^{n+2}/(n+2)$.

When internal deformation is small and slope corrections are uniformly small, $u_b\simeq h^m$ and

$$
\boxed{h_t+(h^{m+1})_x=a.}
$$

For a steady [accumulation](../../../../ice-accumulation.md) profile and prescribed upstream flux $q_{\rm in}$, $\boxed{h_*(x)=[q_{\rm in}+\int_0^xa(\xi)\,d\xi]^{1/(m+1)}}$. For constant $a$ and zero upstream flux this is $(ax)^{1/(m+1)}$ on the region of positive flux.

A small thickness disturbance $\zeta$ satisfies $\zeta_t+[c(x)\zeta]_x=0$ with $c=(m+1)h_*^m$. Hence it travels down-[glacier](../../../../glacier.md) along $dx/dt=c>0$, with amplitude changing as $d\zeta/dt=-c'\zeta$. Since surface speed is $u_s\simeq u_b=h_*^m$ in this sliding-dominated limit,

$$
\boxed{c=(m+1)u_s.}
$$

The thickness wave therefore outruns individual [ice](../../../../ice.md) particles. This is the [sliding-dominated glacier kinematic wave](../../../../sliding-dominated-glacier-kinematic-wave.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
