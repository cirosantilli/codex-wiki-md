<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The holomorphic part of the [free-boson worldsheet propagator](../../../../../free-boson-worldsheet-propagator.md) gives

$$
\partial X^\mu(z)\partial X^\nu(w)\sim-\frac{\alpha'}2\frac{\eta^{\mu\nu}}{(z-w)^2}.
$$

Apply [Wick theorem](../../../../../wick-s-theorem.md) to $T(z)T(w)$. The two double contractions give $D/[2(z-w)^4]$, while the single contractions reconstruct $T$ and its derivative. Thus the [stress-tensor operator-product expansion](../../../../../stress-tensor-operator-product-expansion.md) is

$$
\boxed{
T(z)T(w)\sim\frac{D/2}{(z-w)^4}+\frac{2T(w)}{(z-w)^2}+\frac{\partial T(w)}{z-w}
}
$$

and the $D$ embedding coordinates have [central charge](../../../../../central-charge.md) $\boxed{c=D}$.

The [holomorphic stress-energy tensor](../../../../../holomorphic-stress-energy-tensor.md) generates an infinitesimal conformal transformation through

$$
\delta_vT(z)=\frac1{2\pi i}\oint_zdw\,v(w)T(w)T(z).
$$

Taking the three residues gives

$$
\boxed{\delta_vT=\frac{c}{12}\partial^3v+2(\partial v)T+v\partial T}.
$$

The third derivative is the anomalous term that prevents $T$ from transforming as an ordinary weight-two [Virasoro primary operator](../../../../../primary-field.md).

With [Virasoro algebra](../../../../../virasoro-algebra.md) modes $L_n=(2\pi i)^{-1}\oint dz\,z^{n+1}T(z)$, a second contour calculation gives

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}+\frac{c}{12}m(m^2-1)\delta_{m+n,0}},
$$

so $A(m)=c(m^3-m)/12=D(m^3-m)/12$. This [Virasoro central extension](../../../../../virasoro-central-extension.md) is the quantum conformal anomaly. In string theory the matter and ghost contributions must cancel; $c_{\rm matter}+c_{\rm ghost}=D-26=0$ gives the [critical dimension of string theory](../../../../../critical-dimension-of-string-theory.md) $D=26$ and makes the [BRST operator](../../../../../brst-operator.md) nilpotent.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 306](../../paper-306-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
