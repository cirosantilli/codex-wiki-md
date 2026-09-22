<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [polar molecular field](../../../../../../polar-molecular-field.md) is

$$
h_i=(a+b|\mathbf p|^2)p_i-\kappa\nabla^2p_i.
$$

For a spatially uniform [polar order parameter](../../../../../../polar-order-parameter.md), $\mathbf h=(a+bp^2)\mathbf p$, so it is colinear with $\mathbf p$ and its magnitude is $|\mathbf h|=|a+bp^2|p$. The scalar factor can be negative; colinearity does not necessarily mean parallel orientation.

For the [simple shear flow](../../../../../../simple-shear-flow.md), the paper's [velocity gradient](../../../../../../velocity-gradient.md) convention gives

$$
\Omega=\frac g2\begin{pmatrix}0&-1\\1&0\end{pmatrix},
\qquad D=\frac g2\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Substitute these matrices into $\dot{\mathbf p}=-\Omega\mathbf p+\xi D\mathbf p-\Gamma\mathbf h$. Projection along and perpendicular to the [polar order parameter](../../../../../../polar-order-parameter.md) yields

$$
\frac{\dot p}{p}=\frac{\xi g}{2}\sin2\theta-\Gamma(a+bp^2),
\qquad \dot\theta=\frac g2(\xi\cos2\theta-1).
$$

Assume $g\ne0$, $\Gamma>0$, $b>0$ and $p>0$. The [flow-alignment angle in planar shear](../../../../../../flow-alignment-angle-in-planar-shear.md) must satisfy

$$
\boxed{\cos2\theta=\frac1\xi,
\quad |\xi|\ge1,
\quad \tan^2\theta=\frac{\xi-1}{\xi+1}}.
$$

For $\xi=-1$, use the cosine equation: $\theta=\pi/2$ modulo $\pi$, and the displayed tangent is infinite. The radial equation gives

$$
\boxed{p^2=\frac{-a+\xi g\sin2\theta/(2\Gamma)}b
=\frac{-a\ \pm\ g\sqrt{\xi^2-1}/(2\Gamma)}b},
$$

where the sign distinguishes the angular branches, and only positive right-hand sides are ordered solutions. Linearizing the angular equation gives $\delta\dot\theta=-g\xi\sin2\theta\,\delta\theta$. For $|\xi|>1$, the stable angular branch therefore has

$$
\boxed{p_{\rm stable}^2=\frac{-a+|g|\sqrt{\xi^2-1}/(2\Gamma)}b>0}.
$$

Its radial relaxation eigenvalue is $-2\Gamma bp^2<0$. At $|\xi|=1$ the angular linearization is marginal and $p^2=-a/b$ requires $a<0$. If $g=0$, the shear restriction disappears and any orientation is allowed for $p^2=-a/b>0$. The printed request for dependence only on $a,b,\Gamma,g$ omits $\xi$: in general the magnitude necessarily depends on it.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
