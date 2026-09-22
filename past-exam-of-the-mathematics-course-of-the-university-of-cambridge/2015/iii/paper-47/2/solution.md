<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Spectrum and symmetry.** Choose a [vacuum expectation value](../../../../../vacuum-expectation-value.md) $\phi_0=(0,v/\sqrt2)^T$. In [unitary gauge](../../../../../unitary-gauge.md) the scalar field is $\phi=(0,(v+h)/\sqrt2)^T$, with real $h$. The [Pauli matrix multiplication law](../../../../../pauli-matrix-multiplication-law.md) gives $\{\tau^a,\tau^b\}=\delta^{ab}I/2$. Since $A^aA^b$ is symmetric in gauge indices, only this symmetric product contributes. The kinetic and potential terms therefore become

$$
(D_\mu\phi)^\dagger D^\mu\phi
=\frac12(\partial_\mu h)^2+\frac{g^2}{8}(v+h)^2A_\mu^aA^{a\mu},
$$



$$
V(h)=\frac{\lambda v^2}{2}h^2+\frac{\lambda v}{2}h^3+\frac{\lambda}{8}h^4.
$$

Comparison with $\frac12m_A^2A_\mu^aA^{a\mu}$ and $\frac12m_h^2h^2$ gives

$$
\boxed{m_{A^1}=m_{A^2}=m_{A^3}=\frac{gv}{2},\qquad m_h=\sqrt{\lambda}\,v.}
$$

These are the [scalar interactions after complete SU2 breaking](../../../../../scalar-interactions-after-complete-su2-breaking.md). The scalar mass uses the specified potential normalization: the prefactor $\lambda/2$ is important.

A nonzero complex doublet has trivial stabilizer in $SU(2)$: a matrix fixing $(0,v)^T$ must have second column $(0,1)^T$, and unitarity and determinant one then fix the first column too. Thus all three gauge generators are broken. Three scalar angular directions are absorbed by the [Higgs mechanism](../../../../../higgs-mechanism.md), giving each [gauge boson](../../../../../gauge-boson.md) a longitudinal polarization. The physical degrees of freedom count is

$$
\boxed{3\times2+4=3\times3+1=10,\qquad\text{no massless physical fields}.}
$$

There is no surviving electromagnetic $U(1)$ in this theory: it contains only the gauged $SU(2)$, not the electroweak product group. The would-be [Goldstone bosons](../../../../../goldstone-boson.md) are not additional physical massless particles. This is [complete breaking by an SU2 scalar doublet](../../../../../complete-breaking-by-an-su2-scalar-doublet.md).

**Scalar interactions.** In [unitary gauge](../../../../../unitary-gauge.md), all interaction terms containing the physical scalar are

$$
\boxed{\mathcal L_{\mathrm{scalar,int}}
=\frac{g^2v}{4}hA_\mu^aA^{a\mu}
+\frac{g^2}{8}h^2A_\mu^aA^{a\mu}
-\frac{\lambda v}{2}h^3-\frac{\lambda}{8}h^4.}
$$

These give $hAA$, $hhAA$, $hhh$, and $hhhh$ [Feynman vertices](../../../../../interaction-vertex.md). Their factors are respectively $ig^2v\,\delta^{ab}g_{\mu\nu}/2$, $ig^2\delta^{ab}g_{\mu\nu}/2$, $-3i\lambda v$, and $-3i\lambda$, including the identical-leg multiplicities. Gauge-dependent descriptions also contain the absorbed scalar modes; the above are all physical-scalar interactions in the chosen gauge.

**Gauge self-interactions.** Write $f_{\mu\nu}^a=\partial_\mu A_\nu^a-\partial_\nu A_\mu^a$. Expanding the field-strength square gives the cubic and quartic pieces

$$
\boxed{\mathcal L_3
=\frac g2\epsilon^{abc}f_{\mu\nu}^aA^{b\mu}A^{c\nu}
=g\epsilon^{abc}(\partial_\mu A_\nu^a)A^{b\mu}A^{c\nu},}
$$



$$
\boxed{\mathcal L_4
=-\frac{g^2}{4}\epsilon^{abc}\epsilon^{ade}
A_\mu^bA_\nu^cA^{d\mu}A^{e\nu}.}
$$

The sign of the cubic term follows from the minus sign in the given nonlinear field strength. The quartic term can also be written using $\epsilon^{abc}\epsilon^{ade}=\delta^{bd}\delta^{ce}-\delta^{be}\delta^{cd}$. The cubic [Feynman vertex](../../../../../interaction-vertex.md) joins three wavy gauge lines, has one momentum factor, and is proportional to $g\epsilon^{abc}$. The quartic [Feynman vertex](../../../../../interaction-vertex.md) joins four wavy lines, is proportional to $g^2$, and has products of structure constants with metric contractions. There are no higher pure-gauge vertices in this Lagrangian. These are the [SU2 gauge self-interaction vertices](../../../../../su2-gauge-self-interaction-vertices.md).

<a id="2/image-cubic-and-quartic-gauge-boson-vertices-from-the-su2-field-strength-square"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-47-gauge-vertices.png)

**[Figure 1](#2/image-cubic-and-quartic-gauge-boson-vertices-from-the-su2-field-strength-square). Cubic and quartic gauge-boson vertices from the SU2 field-strength square**.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
