<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Substitution of the proposed [normal mode](../../../../normal-mode.md) into the [wave equation](../../../../wave-equation-split.md) gives the [ordinary differential equations](../../../../ordinary-differential-equation.md)

$$
f_j''+k^2\left(\frac{c^2}{c_j^2}-1\right)f_j=0.
$$

A nonzero exterior [displacement field](../../../../displacement-field-mechanics.md) has [exponential decay](../../../../exponential-decay.md) at infinity only when $c<c_2$. With

$$
\ell=k\sqrt{1-c^2/c_2^2}>0,
$$

its [wave amplitude](../../../../wave-amplitude.md) is $f_2(y)=D e^{-\ell(y-h)}$. At $c=c_2$ the exterior [wave amplitude](../../../../wave-amplitude.md) is affine and cannot decay; at $c>c_2$ it is oscillatory and cannot decay. Setting the exterior [wave amplitude](../../../../wave-amplitude.md) identically zero would impose both $f_1(h)=0$ and $f_1'(h)=0$, forcing the entire [normal mode](../../../../normal-mode.md) to vanish.

We also need $c>c_1$. Indeed, if $c<c_1$, the rigid [boundary condition](../../../../boundary-condition.md) gives $f_1(y)=A\sinh(qy)$ with $q=k\sqrt{1-c^2/c_1^2}>0$. At the interface,

$$
\frac{f_1'(h)}{f_1(h)}=q\coth(qh)>0,
\qquad
\frac{f_2'(h)}{f_2(h)}=-\ell<0,
$$

which contradicts [continuity](../../../../continuous-function.md) of [traction](../../../../traction.md) because both values of the [shear modulus](../../../../shear-modulus.md) are positive. At $c=c_1$, the layer [wave amplitude](../../../../wave-amplitude.md) is $Ay$ and the same contradiction follows from $f_1'(h)/f_1(h)=1/h>0$.

Therefore $c_1<c<c_2$. Define the positive transverse [wavenumber](../../../../wavenumber.md)

$$
m=k\sqrt{c^2/c_1^2-1}.
$$

The rigid [boundary condition](../../../../boundary-condition.md) now gives $f_1(y)=A\sin(my)$. The interface [boundary conditions](../../../../boundary-condition.md) give

$$
D=A\sin(mh),\qquad
\mu_1mA\cos(mh)=-\mu_2\ell A\sin(mh).
$$

Neither $\sin(mh)$ nor $\cos(mh)$ can vanish for a nontrivial [normal mode](../../../../normal-mode.md) with $m,\ell>0$. Dividing therefore gives the [rigid-backed shear-wave dispersion](../../../../rigid-backed-shear-wave-dispersion.md) relation:

$$
\boxed{\frac{c^2}{c_1^2}=1+\frac{m^2}{k^2},\qquad
\frac{c^2}{c_2^2}=1-\frac{\ell^2}{k^2},\qquad
\tan(mh)=-\frac{\mu_1m}{\mu_2\ell}.}
$$

Conversely, positive $m,\ell$ satisfying these relations generate a nonzero [normal mode](../../../../normal-mode.md) through the [wave amplitudes](../../../../wave-amplitude.md) above. Its physical [displacement field](../../../../displacement-field-mechanics.md) is the real part of the complex expression.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
