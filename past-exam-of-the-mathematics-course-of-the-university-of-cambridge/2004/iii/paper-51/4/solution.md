<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Interpret triviality as [holomorphic](../../../../../complex-differentiability-at-a-point.md) triviality. Choose a global [holomorphic](../../../../../complex-differentiability-at-a-point.md) [bundle frame](../../../../../frame-of-a-vector-bundle.md) $s_1,\ldots,s_k$ for $E$. Let $H_\alpha$ have as its columns the coordinates of these sections in the prescribed local frame over $U_\alpha$, with the convention that a fiber coordinate vector transforms as $s_\beta=F_{\alpha\beta}s_\alpha$. Then

$$
H_\beta=F_{\alpha\beta}H_\alpha,\qquad
\boxed{F_{\alpha\beta}=H_\beta H_\alpha^{-1}.}
$$

Each $H_\alpha$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) and invertible because its columns form a basis in every fiber. This proves the requested [holomorphic splitting of transition functions on a trivial bundle](../../../../../holomorphic-splitting-of-transition-functions-on-a-trivial-bundle.md). Smooth or topological triviality alone would not justify [holomorphic](../../../../../complex-differentiability-at-a-point.md) splitting.

For the [line bundle](../../../../../line-bundle.md) on [projective twistor space](../../../../../projective-twistor-space.md), pull its patching function back to the [twistor line](../../../../../twistor-line.md) $L_x$ using the incidence convention of this problem, $\omega^A=x^{AA'}\pi_{A'}$, without an extra factor of $i$. Triviality on each line gives nonvanishing linewise [holomorphic](../../../../../complex-differentiability-at-a-point.md) functions $H_0,H_1$ with $F_{01}=H_1H_0^{-1}$. The factors can be chosen as [holomorphic](../../../../../complex-differentiability-at-a-point.md) functions of $x$ locally: a degree-zero scalar transition function has zero winding on the overlap annulus, hence admits a logarithm there; splitting its positive and negative [Laurent series](../../../../../laurent-series.md) parts gives factors whose coefficients are [Cauchy integrals](../../../../../cauchy-transform.md) that are [holomorphic](../../../../../complex-differentiability-at-a-point.md) functions of $x$. The explicit splitting is worked out below. Their only common linewise ambiguity is multiplication by a nonzero function $g(x)$: the ratio is a global [holomorphic](../../../../../complex-differentiability-at-a-point.md) function on the compact [complex projective line](../../../../../complex-projective-line.md), hence constant on that line.

Take $\epsilon_{0'1'}=1$, $\epsilon^{0'1'}=-1$ and raise a [two-component spinor](../../../../../two-component-spinor.md) by left multiplication with $\epsilon^{A'B'}$. The derivative along an [alpha-plane](../../../../../alpha-plane.md) is $\ell_A=\pi^{A'}\partial_{AA'}$. It annihilates the unsplit twistor function, because

$$
\ell_A\omega^B=\delta_A^B\pi^{A'}\pi_{A'}=0,\qquad\ell_A F_{01}=0.
$$

Thus

$$
G_A=H_0^{-1}\ell_AH_0=H_1^{-1}\ell_AH_1
$$

is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on the whole line and has projective weight one. A section of $\mathcal O(1)$ is linear in the homogeneous coordinates: in an affine coordinate, [holomorphic](../../../../../complex-differentiability-at-a-point.md) regularity at infinity bounds its growth to at most first order, so the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) excludes all higher powers. Therefore

$$
G_A=\pi^{A'}A_{AA'}(x).
$$

The inverse splitting functions obey $(\ell_A+G_A)H_\alpha^{-1}=0$. Commuting these two equations proves

$$
\pi^{A'}\pi^{B'}F_{AA'BB'}=0.
$$

The [spinor decomposition of gauge curvature](../../../../../spinor-decomposition-of-gauge-curvature.md) is

$$
F_{AA'BB'}=\epsilon_{AB}\varphi_{A'B'}+\epsilon_{A'B'}\varphi_{AB},
$$

where both $\varphi$ [two-component spinors](../../../../../two-component-spinor.md) are symmetric. Vanishing of the contraction for every $\pi$ forces $\varphi_{A'B'}=0$. This is exactly the [anti-self-dual Maxwell equations](../../../../../anti-self-dual-maxwell-equations.md). Since the [Abelian](../../../../../abelian-group.md) [gauge curvature](../../../../../gauge-field-strength.md) is $dA$, it is closed; its duality condition also makes it co-closed, giving the source-free [Maxwell equations](../../../../../maxwell-equations.md). Changing both splitting factors by $g(x)$ changes $A$ by $d\log g$, the expected [Abelian](../../../../../abelian-group.md) [gauge transformation](../../../../../gauge-transformation.md). This derives the rank-one [Penrose-Ward correspondence](../../../../../penrose-ward-correspondence.md) in the needed local form.

For the exponential patching function, choose a representative $f$ of the [Čech cohomology](../../../../../cech-cohomology.md) class, of homogeneous degree zero. On the overlap of the two line patches write $f_x(\zeta)=f(x\pi,\pi)=\sum_{n\in\mathbb Z}f_n(x)\zeta^n$. To compute the [gauge potential](../../../../../gauge-field.md) explicitly, use a constant [two-component spinor](../../../../../two-component-spinor.md) basis in which $\iota_{A'}=(1,0)$ and the finite patch $\pi_{0'}=\zeta,\pi_{1'}=1$. Then $\pi^{0'}=-1$, $\pi^{1'}=\zeta$ and

$$
\iota_{C'}\pi^{C'}=-1,\qquad \pi_{D'}d\pi^{D'}=d\zeta,\qquad
\omega^B=x^{B0'}\zeta+x^{B1'}.
$$

For a positively oriented contour in the overlap annulus, split its [Laurent series](../../../../../laurent-series.md) as

$$
h_0=-\sum_{n\ge0}f_n\zeta^n,\qquad
h_1=\sum_{n<0}f_n\zeta^n,\qquad f_x=h_1-h_0.
$$

The first is [holomorphic](../../../../../complex-differentiability-at-a-point.md) inside the contour, the second outside including infinity; $H_\alpha=e^{h_\alpha}$ split $e^f$. Since $(-\partial_{B0'}+\zeta\partial_{B1'})f_x=0$, coefficient comparison gives $\partial_{B0'}f_n=\partial_{B1'}f_{n-1}$. Applying that operator separately to $h_0,h_1$ cancels all nonconstant terms and leaves

$$
G_B=\partial_{B1'}f_{-1}.
$$

Thus $-A_{B0'}+\zeta A_{B1'}=G_B$ yields $A_{B1'}=0$ and $A_{B0'}=-\partial_{B1'}f_{-1}$. Moreover

$$
f_{-1}=\frac1{2\pi i}\oint_\Gamma f_x\,d\zeta,\qquad
\partial_{B1'}f_x=f_{,B}:=\frac{\partial f}{\partial\omega^B}.
$$

Substitution gives $A_{B0'}=-(2\pi i)^{-1}\oint f_{,B}\,d\zeta$, which in homogeneous form is precisely

$$
\boxed{A_{BB'}=\frac1{2\pi i}\oint_\Gamma
\frac{\iota_{B'}}{\iota_{C'}\pi^{C'}}\,f_{,B}(x\pi,\pi)\,\pi_{D'}d\pi^{D'}.}
$$

This is the [Abelian Ward splitting by Laurent series](../../../../../abelian-ward-splitting-by-laurent-series.md). The factors have weights $-1,-1,2$, respectively, so the integrand is invariant under a change of homogeneous representative. The contour avoids $\iota_{C'}\pi^{C'}=0$; the basis chosen above places that point at infinity. One can keep the contour fixed for $x$ in a sufficiently small domain, allowing differentiation under the integral.

Finally differentiate the [contour potential for an anti-self-dual Maxwell field](../../../../../contour-potential-for-an-anti-self-dual-maxwell-field.md). By the [twistor incidence relation](../../../../../twistor-incidence-relation.md), $\partial_{AA'} f_{,B}=\pi_{A'}f_{,AB}$. Consequently

$$
\begin{aligned}
F_{AA'BB'}&=\frac1{2\pi i}\oint_\Gamma
\frac{\pi_{A'}\iota_{B'}-\pi_{B'}\iota_{A'}}{\iota_{C'}\pi^{C'}}\,
 f_{,AB}\,\pi_{D'}d\pi^{D'}\\
&=\epsilon_{A'B'}\,\frac1{2\pi i}\oint_\Gamma f_{,AB}\,\pi_{D'}d\pi^{D'}.
\end{aligned}
$$

The second equality uses the elementary two-spinor identity $\pi_{A'}\iota_{B'}-\pi_{B'}\iota_{A'}=\epsilon_{A'B'}(\iota_{C'}\pi^{C'})$ in the declared convention. The remaining [two-component spinor](../../../../../two-component-spinor.md) is symmetric in $A,B$, and no primed symmetric [gauge curvature](../../../../../gauge-field-strength.md) part survives. This directly verifies **$dA$ is anti-self-dual**. In complexified Lorentzian signature duality has [Hodge star](../../../../../hodge-star-operator.md) [eigenvalues](../../../../../eigenvalue.md) $\pm i$; here the vanishing primed [two-component spinor](../../../../../two-component-spinor.md) fixes the stated ASD convention rather than incorrectly imposing the Euclidean equation $*F=-F$ on that signature.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
