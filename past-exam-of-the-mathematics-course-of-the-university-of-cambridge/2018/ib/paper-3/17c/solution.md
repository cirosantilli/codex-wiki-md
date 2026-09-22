<h1 id="17c/solution">Solution</h1>

↑ **Parent:** [17C](../17c.md)

Take the dot product of [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) with $E$ and of [Faraday's law](../../../../../faraday-s-law-of-induction.md) with $B/\mu_0$. The [divergence of a cross product](../../../../../divergence-of-a-cross-product.md) identity

$$
\nabla\mathbin{\cdot}(E\times B)=B\mathbin{\cdot}(\nabla\times E)-E\mathbin{\cdot}(\nabla\times B)
$$

then gives the local [Poynting theorem](../../../../../poynting-theorem.md)

$$
\frac{\partial}{\partial t}\left(\frac{\varepsilon_0E^2}{2}+\frac{B^2}{2\mu_0}\right)+J\mathbin{\cdot}E+\nabla\mathbin{\cdot}\left(\frac1{\mu_0}E\times B\right)=0.
$$

Integration and the [divergence theorem](../../../../../divergence-theorem.md) produce the stated equation. Its terms are the rate of change of [electromagnetic energy](../../../../../electromagnetic-energy.md), the work per unit time done on charges, and the outward flux of the [Poynting vector](../../../../../poynting-vector.md) $S=E\times B/\mu_0$.

Let the plate separation be $d$ and their radius be $R$, so $A=\pi R^2$. Between the plates,

$$
E=\frac{q}{\varepsilon_0A}\,\hat z.
$$

For a circular [Amperian loop](../../../../../amperian-loop.md) of radius $r<R$, the [displacement current](../../../../../displacement-current.md) in the [Ampère-Maxwell equation](../../../../../ampere-s-circuital-law.md) gives

$$
B_\phi(r)=\frac{\mu_0\varepsilon_0r}{2}\dot E
=-\frac{\mu_0\lambda q r}{2A}.
$$

Therefore

$$
\boxed{S=\frac{\lambda q^2r}{2\varepsilon_0A^2}\,\hat r,}
$$

which points radially outward. Its flux through the cylindrical side is $\lambda q^2d/(\varepsilon_0A)$, exactly $-dU/dt$ for the stored [capacitor energy](../../../../../capacitor-energy.md) $U=q^2d/(2\varepsilon_0A)$.

## ↑ Ancestors (10)

1. [17C](../17c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
