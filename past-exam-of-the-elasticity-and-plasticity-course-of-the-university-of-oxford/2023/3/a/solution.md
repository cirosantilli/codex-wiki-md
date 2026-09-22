<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume homogeneous [Lamé parameters](../../../../lame-parameter.md), with $\mu>0$ and positive [bulk modulus](../../../../bulk-modulus.md) $K=\lambda+2\mu/3$. For [spherical symmetry](../../../../spherical-symmetry.md), write $q=\tau_{rr}$ and $t=\tau_{\theta\theta}=\tau_{\phi\phi}$. Radial [force balance](../../../../force-balance.md) is $q'+2(q-t)/r=0$. The given [linear elasticity](../../../../linear-elasticity.md) relations imply

$$
q-t=2\mu\left(u'-\frac ur\right),\qquad
q'=(\lambda+2\mu)u''+2\lambda\left(\frac{u'}r-\frac{u}{r^2}\right).
$$

Substitution into radial [force balance](../../../../force-balance.md) gives

$$
0=(\lambda+2\mu)\left(u''+\frac{2u'}r-\frac{2u}{r^2}\right)
=\frac{d}{dr}\left[(\lambda+2\mu)\left(u'+\frac{2u}r\right)\right].
$$

Thus

$$
\boxed{\frac{d}{dr}\left[(\lambda+2\mu)\left(u'+\frac{2u}r\right)\right]=0.}
$$

The [volumetric strain](../../../../volumetric-strain.md) is $e=u'+2u/r$, and the [trace](../../../../matrix-trace.md) of the [stress tensor](../../../../cauchy-stress-tensor.md) is

$$
q+2t=(3\lambda+2\mu)e.
$$

Since $\lambda+2\mu=K+4\mu/3>0$ is constant, $e'=0$. The [radial elastic compatibility](../../../../radial-elastic-compatibility.md) condition follows:

$$
\boxed{\frac{d}{dr}(\tau_{rr}+\tau_{\theta\theta}+\tau_{\phi\phi})=0.}
$$

This condition is local to a region governed by homogeneous [linear elasticity](../../../../linear-elasticity.md); it is not a constitutive condition for a plastically deforming region.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
