<h1 id="4d/solution">Solution</h1>

↑ **Parent:** [4D](../4d.md)

[Gauss's law](../../../../../gauss-s-law.md) in electrostatics states

$$
\oint_{\partial V}E\mathbin{\cdot}dS
=\frac{Q_{\rm enclosed}}{\varepsilon_0}.
$$

Cylindrical symmetry and a coaxial Gaussian cylinder give

$$
E(r)=
\begin{cases}
0,&0<r<a,\\[2pt]
\dfrac{Q}{2\pi\varepsilon_0r}\,e_r,&a<r<b,\\[6pt]
0,&r>b.
\end{cases}
$$

The field vanishes inside each perfect conductor, and outside the cable because the total enclosed charge per unit length is zero.

Choose the outer conductor's potential to be zero. Since $E=-\nabla V$,

$$
V(r)=
\begin{cases}
\dfrac{Q}{2\pi\varepsilon_0}\log(b/a),&0<r\leq a,\\[6pt]
\dfrac{Q}{2\pi\varepsilon_0}\log(b/r),&a<r<b,\\[6pt]
0,&r\geq b.
\end{cases}
$$

The [capacitance per unit length](../../../../../capacitance-per-unit-length.md) is therefore

$$
\boxed{C=\frac{Q}{V(a)-V(b)}
=\frac{2\pi\varepsilon_0}{\log(b/a)}}.
$$

The [electrostatic energy](../../../../../electrostatic-energy.md) per unit length is

$$
U=\frac{\varepsilon_0}{2}
\int_a^b|E|^2\,2\pi r\,dr
=\boxed{\frac{Q^2}{4\pi\varepsilon_0}\log\frac ba}.
$$

Substitution of $C$ verifies $U=Q^2/(2C)$.

## ↑ Ancestors (10)

1. [4D](../4d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
