<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

There is a sign inconsistency in the printed model. For the ordinary [cross product](../../../../../cross-product.md) let $J(a)z=a\times z$. The vector triple-product identity gives $[J(a),J(b)]=J(a\times b)$. Consequently the printed $D_\mu=\partial_\mu+eJ(A_\mu)$ has [gauge curvature](../../../../../gauge-field-strength.md)

$$
[D_\mu,D_\nu]\Phi=eF^+_{\mu\nu}\times\Phi,\qquad
F^+_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu+eA_\mu\times A_\nu.
$$

Its [gauge curvature](../../../../../gauge-field-strength.md) cannot instead contain the printed negative quadratic term. For a noncommuting [pure gauge potential](../../../../../pure-gauge-potential.md) for this [gauge covariant derivative](../../../../../gauge-covariant-derivative.md), $F^+=0$ whereas $F^-=-2eA_\mu\times A_\nu\ne0$. Thus the printed gauge [kinetic term](../../../../../kinetic-term.md) assigns a nonzero value to a connection obtained by applying the [gauge-field transformation law](../../../../../gauge-field-transformation-law.md) to the zero connection. Literally the printed action has global rotations but not the requested local triplet [gauge symmetry](../../../../../gauge-invariance.md). The [cross-product convention for an adjoint covariant derivative](../../../../../cross-product-convention-for-an-adjoint-covariant-derivative.md) makes the minimal repair explicit: change the [gauge field strength](../../../../../gauge-field-strength.md) quadratic term to a plus sign, retaining the printed [gauge covariant derivative](../../../../../gauge-covariant-derivative.md). Changing the sign in the [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) instead would be another consistent convention. The remaining calculation uses the first repair.

The corrected theory has local [SO(3)](../../../../../so-3-group.md) [gauge symmetry](../../../../../gauge-invariance.md), equivalently the adjoint-field realization of the [SU(2)](../../../../../su-2-group.md) [Lie algebra](../../../../../lie-algebra-split.md); its [adjoint scalar fields](../../../../../adjoint-scalar-field.md) and [gauge fields](../../../../../gauge-field.md) are insensitive to the [center of a group](../../../../../center-of-a-group.md) of [SU(2)](../../../../../su-2-group.md). Explicitly, $\Phi\mapsto R(x)\Phi$ and

$$
eJ(A_\mu)\mapsto R\,eJ(A_\mu)R^{-1}-(\partial_\mu R)R^{-1}.
$$

Both $D_\mu\Phi$ and $F_{\mu\nu}$ transform as triplets, so their [dot products](../../../../../dot-product.md) and the [scalar potential](../../../../../scalar-potential.md) are invariant. Assume $\lambda>0$, $e\ne0$ and take $v\ge0$ without loss of generality. For $v>0$ the minima have $\Phi^2=v^2$. Choose the [scalar-field vacuum](../../../../../scalar-field-vacuum.md) $\Phi_0=v(0,0,1)$, whose [stabilizer](../../../../../stabilizer-subgroup.md) consists of rotations around the third axis: **the residual [gauge symmetry](../../../../../gauge-invariance.md) is SO(2), locally [U(1)](../../../../../circle-group.md).**

In [unitary gauge](../../../../../unitary-gauge.md) write $\Phi=(0,0,v+h)$, $A_\mu=A^3_\mu$ and $W^\pm_\mu=(A^1_\mu\mp iA^2_\mu)/\sqrt2$. These are the neutral massless [gauge field](../../../../../gauge-field.md), two charged massive [gauge fields](../../../../../gauge-field.md) and a real radial [scalar field](../../../../../scalar-field.md). Define

$$
f_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu,\qquad
C_{\mu\nu}=W^+_\mu W^-_\nu-W^+_\nu W^-_\mu,
$$



$$
G^\pm_{\mu\nu}=(\partial_\mu\mp ieA_\mu)W^\pm_\nu-(\partial_\nu\mp ieA_\nu)W^\pm_\mu.
$$

Substitution gives $F^3_{\mu\nu}=f_{\mu\nu}-ieC_{\mu\nu}$ and $(F^1_{\mu\nu}\mp iF^2_{\mu\nu})/\sqrt2=G^\pm_{\mu\nu}$. The entire physical-field [Lagrangian density](../../../../../lagrangian-density.md) is therefore

$$
\mathcal L=-\frac14(f_{\mu\nu}-ieC_{\mu\nu})(f^{\mu\nu}-ieC^{\mu\nu})
-\frac12G^+_{\mu\nu}G^{-\mu\nu}
+\frac12\partial_\mu h\partial^\mu h+e^2(v+h)^2W^+_\mu W^{-\mu}
-\frac\lambda8[(v+h)^2-v^2]^2.
$$

In particular $D_\mu\Phi=(e(v+h)A^2_\mu,-e(v+h)A^1_\mu,\partial_\mu h)$; this directly verifies the [scalar field](../../../../../scalar-field.md) kinetic and vector [mass terms](../../../../../mass-term.md). Expanding the [scalar potential](../../../../../scalar-potential.md) gives $\lambda v^2h^2/2+\lambda vh^3/2+\lambda h^4/8$. Comparing the quadratic terms with standard [real scalar field](../../../../../real-scalar-field.md) and charged-vector [mass terms](../../../../../mass-term.md) yields the [adjoint triplet Higgs spectrum](../../../../../adjoint-triplet-higgs-spectrum.md),

$$
\boxed{m_{W^\pm}^2=e^2v^2,\qquad m_A=0,\qquad m_h^2=\lambda v^2}.
$$

This also rewrites the purely vector interactions, which are already contained in the displayed [gauge field strengths](../../../../../gauge-field-strength.md) rather than omitted from the theory.

The original symmetry remains unbroken **at $v=0$**. The unique minimum is then $\Phi=0$, with three massless [gauge fields](../../../../../gauge-field.md) and three massless [real scalar field](../../../../../real-scalar-field.md) components; the quartic [scalar field](../../../../../scalar-field.md) interaction remains. The physical [degrees of freedom](../../../../../degree-of-freedom.md) number $3\times2+3=9$. At $v>0$ the two broken generators supply two [Goldstone bosons](../../../../../goldstone-boson.md), eaten to give [longitudinal gauge-boson polarizations](../../../../../longitudinal-polarization-of-a-massive-vector-boson.md) of the charged vectors. The physical count is $2\times3+2+1=9$: two massive vectors, one massless vector and one radial [scalar field](../../../../../scalar-field.md). The scalar components eaten in [unitary gauge](../../../../../unitary-gauge.md) are not additional physical particles.

For the broken phase all interactions containing the physical [scalar field](../../../../../scalar-field.md) are

$$
\mathcal L_{\rm scalar,int}=-\frac{\lambda v}{2}h^3-\frac\lambda8h^4
+2e^2vhW^+_\mu W^{-\mu}+e^2h^2W^+_\mu W^{-\mu}.
$$

Multiplying interaction coefficients by $i$ and differentiating with respect to the external fields includes the identical-field [factorials](../../../../../factorial.md). The [scalar vertices of an adjoint triplet Higgs model](../../../../../scalar-vertices-of-an-adjoint-triplet-higgs-model.md) are

$$
\boxed{hhh:\ -3i\lambda v,\quad hhhh:\ -3i\lambda,\quad
hW^+_\mu W^-_\nu:\ 2ie^2v g_{\mu\nu},\quad
hhW^+_\mu W^-_\nu:\ 2ie^2g_{\mu\nu}}.
$$

For example, the $h^3$ rule contains $3!$, whereas the $hhW^+W^-$ rule contains only $2!$ from its two identical [scalar fields](../../../../../scalar-field.md). There are no $hAA$ or $hhAA$ vertices: the radial [scalar field](../../../../../scalar-field.md) is neutral under the residual [U(1)](../../../../../circle-group.md). There is no derivative scalar-vector vertex in this physical spectrum in [unitary gauge](../../../../../unitary-gauge.md).

<a id="4/image-all-physical-scalar-interaction-vertices-in-the-broken-triplet-higgs-model-with-the-unbroken-phase-scalar-vertices-shown-below-dashed-lines-are-scalars-and-wavy-lines-are-vectors"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-53-scalar-vertices.png)

**[Figure 2](#4/image-all-physical-scalar-interaction-vertices-in-the-broken-triplet-higgs-model-with-the-unbroken-phase-scalar-vertices-shown-below-dashed-lines-are-scalars-and-wavy-lines-are-vectors). All physical-scalar interaction vertices in the broken triplet Higgs model, with the unbroken-phase scalar vertices shown below; dashed lines are scalars and wavy lines are vectors**.

For completeness, if the unbroken phase is chosen, its physical [scalar fields](../../../../../scalar-field.md) are the three components $\phi_a$, not a single radial $h$. Expanding its [gauge-covariant kinetic term](../../../../../gauge-covariant-kinetic-term.md) gives

$$
\mathcal L_{A\phi\phi}=e\epsilon^{iaj}(\partial_\mu\phi_i)A^{a\mu}\phi_j,\qquad
\mathcal L_{AA\phi\phi}=\frac{e^2}{2}[A_\mu^aA^{a\mu}\phi_b\phi_b-A_\mu^a\phi_aA^{b\mu}\phi_b].
$$

With all momenta incoming and [Fourier transform](../../../../../fourier-transform.md) convention $e^{-ipx}$, the three unbroken-phase rules are

$$
A^a_\mu\phi_b(p)\phi_c(q):\quad e\epsilon^{abc}(q-p)_\mu,
$$



$$
A^a_\mu A^b_\nu\phi_c\phi_d:\quad
ie^2(2\delta^{ab}\delta^{cd}-\delta^{ac}\delta^{bd}-\delta^{ad}\delta^{bc})g_{\mu\nu},
$$



$$
\phi_a\phi_b\phi_c\phi_d:\quad
-i\lambda(\delta^{ab}\delta^{cd}+\delta^{ac}\delta^{bd}+\delta^{ad}\delta^{bc}).
$$

The first rule follows by differentiating once on each possible scalar: for $a=3,b=1,c=2$, the interaction is $eA^3_\mu(\phi_1\partial^\mu\phi_2-\phi_2\partial^\mu\phi_1)$, which fixes the momentum sign. The remaining rules follow from the quadratic gauge interaction and $-\lambda(\phi_a\phi_a)^2/8$. There are no unbroken-phase cubic [scalar field](../../../../../scalar-field.md) [Feynman vertices](../../../../../interaction-vertex.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 53](../../paper-53-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
