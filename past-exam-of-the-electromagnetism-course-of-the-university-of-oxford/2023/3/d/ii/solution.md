<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The leading [electric dipole radiation](../../../../../electric-dipole-radiation.md) fields are

$$
\mathbf E_{\rm rad}=\frac{\mathbf n(\mathbf n\cdot\mathbf p'')-\mathbf p''}{4\pi\epsilon_0c^2r},\qquad
\mathbf B_{\rm rad}=\frac{\mu_0}{4\pi cr}\mathbf p''\times\mathbf n
=\frac1c\mathbf n\times\mathbf E_{\rm rad}.
$$

The radiation [electric field](../../../../../electric-field-split.md) is transverse, $\mathbf n\cdot\mathbf E_{\rm rad}=0$. The [vector triple product](../../../../../vector-triple-product.md) therefore gives the leading [Poynting vector](../../../../../poynting-vector.md)

$$
\boldsymbol{\mathcal P}=\frac1{\mu_0c}\mathbf E_{\rm rad}\times(\mathbf n\times\mathbf E_{\rm rad})+O(r^{-3})
=\frac{|\mathbf E_{\rm rad}|^2}{\mu_0c}\mathbf n+O(r^{-3}).
$$

If $\theta$ is the angle between $\mathbf p''(t-r/c)$ and $\mathbf n$, then

$$
|\mathbf n(\mathbf n\cdot\mathbf p'')-\mathbf p''|^2
=|\mathbf p''|^2-(\mathbf n\cdot\mathbf p'')^2
=|\mathbf p''|^2\sin^2\theta.
$$

Using $\mu_0\epsilon_0c^2=1$, the final result is

$$
\boxed{\boldsymbol{\mathcal P}(\mathbf r,t)=
\frac{|\mathbf p''(t-r/c)|^2\sin^2\theta}{16\pi^2\epsilon_0c^3r^2}\mathbf n+O(r^{-3}),\qquad
|\boldsymbol{\mathcal P}|=\frac{|\mathbf p''(t-r/c)|^2\sin^2\theta}{16\pi^2\epsilon_0c^3r^2}+O(r^{-3}).}
$$

The leading [Poynting flux](../../../../../poynting-flux.md) is outward, vanishes along the instantaneous retarded $\mathbf p''$ axis, and is maximal in its perpendicular plane. If $\mathbf p''=0$, the radiation term is zero and no angle needs to be assigned. The large-$r$ expansion assumes bounded retarded [electric dipole moment](../../../../../electric-dipole-moment.md) and time [derivatives](../../../../../derivative.md); it may also be read at fixed [retarded time](../../../../../retarded-time.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
