<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose a parallel-transported [orthonormal basis](../../../../../../../orthonormal-basis.md) of the screen. In that basis a symmetric trace-free [null shear](../../../../../../../null-shear.md) and antisymmetric [null twist](../../../../../../../null-twist.md) have forms

$$
\widehat\sigma=\begin{pmatrix}s&t\\t&-s\end{pmatrix},\qquad\widehat\omega=\begin{pmatrix}0&w\\-w&0\end{pmatrix}.
$$

Direct multiplication gives

$$
\widehat\sigma^2=(s^2+t^2)I,\qquad\widehat\omega^2=-w^2I,\qquad\widehat\sigma\widehat\omega+\widehat\omega\widehat\sigma=0.
$$

Hence

$$
\widehat B^2=\left(\frac{\theta^2}{4}+s^2+t^2-w^2\right)I+\theta(\widehat\sigma+\widehat\omega).
$$

Since the tidal [matrix](../../../../../../../matrix.md) is symmetric, the antisymmetric part of the [Sachs optical equations](../../../../../../../sachs-optical-equations.md) immediately gives

$$
\boxed{U\cdot\nabla\widehat\omega_{ab}=-\theta\widehat\omega_{ab}.}
$$

Thus an initially [null twist](../../../../../../../null-twist.md)-free [null geodesic congruence](../../../../../../../null-geodesic-congruence.md) remains [null twist](../../../../../../../null-twist.md)-free while its optical description is regular.

To obtain the trace-free symmetric source, use the original PDF's [Weyl tensor](../../../../../../../weyl-tensor.md) formula, with antisymmetrization brackets carrying weight $1/2$. The TeX aid has lost indices and brackets. The correct curvature decomposition is

$$
R_{cedf}=C_{cedf}+g_{c[d}R_{f]e}-g_{e[d}R_{f]c}-\frac R3g_{c[d}g_{f]e}.
$$

Contract with $U^cU^d$ and project $e,f$ onto the screen. Terms containing $U^2$ or a remaining screen-projected $U$ vanish. The only Ricci term left is

$$
\mathcal R_{ab}=P_a{}^eP_b{}^fC_{cedf}U^cU^d+\frac12P_{ab}R_{cd}U^cU^d.
$$

The Weyl term has zero screen trace, by its trace-free property and antisymmetry. Consequently the trace-free symmetric part of the optical equation is the [null-shear propagation equation](../../../../../../../null-shear-propagation-equation.md)

$$
\boxed{U\cdot\nabla\widehat\sigma_{ab}=-\theta\widehat\sigma_{ab}-P_a{}^eP_b{}^fC_{cedf}U^cU^d.}
$$

The two-dimensional [matrix](../../../../../../../matrix.md) identities are essential: in a higher-dimensional screen the [null shear](../../../../../../../null-shear.md) square can have a trace-free part and the [null shear](../../../../../../../null-shear.md)–[null twist](../../../../../../../null-twist.md) [anticommutator](../../../../../../../anticommutator.md) need not vanish. Choosing the parallel-transported auxiliary [null vector](../../../../../../../null-vector.md) makes these tensor transport formulae hold without extra moving-screen terms.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 66](../../../../paper-66-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
