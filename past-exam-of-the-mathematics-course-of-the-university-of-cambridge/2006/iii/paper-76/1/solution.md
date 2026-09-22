<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $F$ be an invertible, orientation-preserving [deformation gradient](../../../../../deformation-gradient.md), with $J=\det F>0$. To prove [Nanson's formula](../../../../../nanson-s-formula.md), take two reference surface [tangent vectors](../../../../../tangent-vector.md) $a,b$. Their current images are $Fa,Fb$, and their oriented area vectors are proportional to $a\times b$ and $(Fa)\times(Fb)$. For every vector $c$, the scalar triple product gives

$$
(Fc)\cdot[(Fa)\times(Fb)]=Jc\cdot(a\times b).
$$

Thus $F^T[(Fa)\times(Fb)]=J(a\times b)$, and

$$
\boxed{dS=JF^{-T}dS_0}.
$$

This proof also identifies the area transformation as the cofactor of $F$, rather than a transformation by $F$ itself.

Use the paper's material-index-first [nominal stress tensor](../../../../../nominal-stress-tensor.md) $P_{Ii}$. Equality of force on the same material surface in its two configurations gives $P_{Ii}\,dS_{0I}=\sigma_{ji}\,dS_j$. Substitute the area transformation to obtain

$$
\boxed{P_{Ii}=J(F^{-1})_{Ij}\sigma_{ji}},\qquad \boxed{\tau_{ji}=J\sigma_{ji}=F_{jI}P_{Ii}}.
$$

Here $\tau$ is the [Kirchhoff stress tensor](../../../../../kirchhoff-stress-tensor.md). With symmetric [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md), the matrix forms are $P=JF^{-1}\sigma$ and $\tau=FP$. This $P$ is the transpose of the [first Piola-Kirchhoff stress tensor](../../../../../first-piola-kirchhoff-stress-tensor.md); keeping the index convention prevents a spurious transpose later.

For the [velocity gradient](../../../../../velocity-gradient.md) $L=\dot FF^{-1}$, let $D=(L+L^T)/2$ be the [rate-of-strain tensor](../../../../../strain-rate-tensor.md). Then the reference-volume mechanical power is

$$
P_{Ii}\dot F_{iI}=\tau_{ji}(F^{-1})_{Ij}\dot F_{iI}=\tau_{ji}L_{ij}=\boxed{\tau_{ji}D_{ij}}.
$$

The last step uses stress symmetry, as supplied by angular-momentum balance in an ordinary continuum without couple stresses: a symmetric tensor has zero contraction with the skew part of $L$.

By [work-conjugate stress and strain](../../../../../work-conjugate-stress-and-strain.md), a pair $(T,E)$ must satisfy $T:\dot E=\tau:D$ for every deformation rate, with both sides measured per reference volume. For the [Green-Lagrange strain tensor](../../../../../green-lagrange-strain-tensor.md), set $C=F^TF$ and calculate

$$
\dot E^{(2)}=\tfrac12(\dot F^TF+F^T\dot F)=F^TDF.
$$

Cyclically rearranging the contraction shows $T^{(2)}:\dot E^{(2)}=(FT^{(2)}F^T):D$. Hence the symmetric conjugate is

$$
\boxed{T^{(2)}=F^{-1}\tau F^{-T}},
$$

the [second Piola-Kirchhoff stress tensor](../../../../../second-piola-kirchhoff-stress-tensor.md).

The [inverse right Cauchy-Green strain](../../../../../inverse-right-cauchy-green-strain.md) is $E^{(-2)}=(I-C^{-1})/2$, because $C^{-1}=F^{-1}F^{-T}$. Differentiating $CC^{-1}=I$ gives

$$
\dot E^{(-2)}=\tfrac12C^{-1}\dot CC^{-1}=F^{-1}DF^{-T}.
$$

Consequently $T^{(-2)}:\dot E^{(-2)}=(F^{-T}T^{(-2)}F^{-1}):D$, and

$$
\boxed{T^{(-2)}=F^T\tau F}.
$$

The two stress measures have a geometric interpretation in the convected coordinate net. Its basis vectors are $g_I=Fe_I$ and its reciprocal basis is $g^I=F^{-T}e_I$. The entries of $T^{(2)}$ are the contravariant components in $\tau=T^{(2)}_{IJ}g_I\otimes g_J$, whereas $T^{(-2)}_{IJ}=g_I\cdot\tau g_J$ are the covariant components, equivalently $\tau=T^{(-2)}_{IJ}g^I\otimes g^J$. They describe the same spatial [Kirchhoff stress tensor](../../../../../kirchhoff-stress-tensor.md) in a deforming, generally nonorthonormal coordinate net.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
